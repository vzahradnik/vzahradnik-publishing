# Arduino: Excellent for Teaching, Dangerous for Business

I’ve been inside the Arduino ecosystem for years. What began as a hobby slowly pulled me into professional embedded development — and for a long time, I was one of the rare developers actually being paid to write Arduino firmware.

As my projects grew in scale and complexity, a pattern became impossible to ignore:

> **Arduino is brilliant for learning — but a liability for production.**
> (Framework, not the hardware. The boards themselves are unusable for any serious commercial deployment.)

Below is a distilled list of the biggest issues I’ve encountered over the years.

## 1. Arduino IDE: Built for Teaching, Not for Engineering
The IDE is intentionally simple — great for beginners, limiting for real engineering work. Industrial-grade projects immediately require PlatformIO (or custom build systems) to stay sane.

## 2. Dependency Management Is Primitive
Arduino IDE has no project-scoped dependencies. You install libraries globally and manually — repeatedly. PlatformIO fixes this, but that alone shows how far the ecosystem lags behind modern software standards.

## 3. The Library “Ghost Town” Problem
Yes — Arduino has a library for everything. No — you should not rely on most of them.

The typical pattern:
- original library abandoned
- pull requests ignored
- ecosystem forks proliferate
- each fork contains partial fixes
- nothing becomes canonical

I maintain several of my own forks just to keep projects from breaking. In some cases, I had to write entirely new libraries from scratch (for example: that infamous non-standard RFID reader — code on my GitHub).

## 4. Testing Culture Is Almost Non-Existent
Unit and integration tests are rare. CI/CD pipelines are rarer.

I ended up building a custom GitHub Actions pipeline with QEMU-based firmware execution to simulate the hardware and test everything automatically. Arduino does not help you here — at all.

## 5. Third-Party Arduino Ports Are Risky
If you use a chip vendor’s Arduino “support package,” expect:
- bugs
- lagging behind native SDKs
- unfixable platform issues
- hacks and workarounds

Some vendors do impressive work — but the inconsistency makes serious development fragile.

## 6. Concurrency Is Painful
Anything that needs parallel execution, scheduled tasks, or non-blocking flow quickly becomes a labyrinth.

TaskManager from TcMenu helps (I co-maintain parts of that ecosystem), but even then:
- long-running tasks freeze displays
- tight loops starve updates
- debugging timing issues becomes a sport

There is nothing like async/await or structured concurrency.

## 7. Memory Pressure Is Brutal
It’s 2025 and we still fight for kilobytes. This made me a better engineer, but JSON on Arduino now feels like a personal attack on RAM.

I use Protocol Buffers on microcontrollers for this exact reason.

## 8. Auto-Generated Code: Practically Unheard Of
Anyone used to Android, Java, C#, or modern build chains expects code generation to be trivial.

With Arduino, achieving this requires:
- custom PlatformIO scripts
- opaque documentation
- low-level build manipulation

I made it work — but only because I refused to accept “just do it manually.”

## 9. Tooling Culture Is Behind
VS Code and Arduino IDE are text editors with plugins — not true IDEs.

For serious work I pair VS Code with JetBrains CLion to get real static analysis + refactoring tools.

## 10. Professional Developer Flows Are DIY
CI/CD? Hardware farms? Automated testing? Versioned dependencies? L10n/i18n? Code generation?

All possible — but mostly unsupported. You build everything yourself because most of the community is still hobbyists.

## 11. Lack of Integrated Solutions
Arduino has countless libraries, but almost no cohesive frameworks.

If you want to build, say, a commercial smart henhouse:
- you combine 10+ libraries
- you debug incompatibilities
- you fight firmware size
- you pray nothing exceeds flash memory

There’s no unified path to production.

## 12. Zero Built-In Internationalization
Arduino has no native support for internationalization (i18n) or localization (l10n). TcMenu implements a custom solution using Java-style .properties files that are converted into C header files with #define constants (as in the screenshot). TcMenu handles the code generation internally, so no GitHub Actions are required. It works reliably, but it’s still a workaround built on top of a framework that was never designed with i18n in mind.

I’m considering a gettext-based solution for the future — but it’s telling that such tooling is missing entirely.

---

## So Where Does This Leave Arduino?
Arduino has done more for hobbyists than almost any electronics platform. It got *me* into embedded engineering.

But every design has a trade-off:

> **You can optimize for learning — or for production. Arduino optimizes for learning.**

I still maintain multiple Arduino codebases, but all future work will move toward:
- **native SDKs like ESP-IDF**, or
- **Zephyr**, which implements features (like device trees) that I previously reinvented.

In the meantime, I continuously minimize dependencies and migrate to native APIs even inside Arduino projects. (Example: Espressif’s native logging library — already included, already good.)

---

## If you’ve shipped a commercial product on Arduino… I’m curious.
How did it go for you? What limitations did you hit? What workarounds did you end up creating?

And if your team is stuck maintaining a legacy Arduino codebase, I’m happy to discuss migration paths.

**Thanks for reading.**

— Vladimír Záhradník

---

## Short LinkedIn Post Intro (to promote the article)

**Arduino is great for learning — but dangerous for business.**

After years of building commercial firmware on Arduino (and maintaining multiple large codebases), I wrote a detailed breakdown of the limitations teams should be aware of.

This isn’t a criticism — Arduino is fantastic for teaching. But the moment a prototype becomes a product, the trade-offs become very real.

👉 *Full breakdown here:* **[Insert your Pulse article link]**

