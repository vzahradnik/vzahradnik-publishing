Cloud kills sovereignty - Why modern IoT devices are paperweight without the internet (Lutemi Hentower as a counter-example)

Fragmented IoT ecosystem - Every manufacturer builds their own platform, you as a customer have 10 smart apps to control your smart home. Home Assistant and open API as the 
only proper solution

Aggressive push of AI, customers most affected - Android phones are bloated with AI, deeply integrated into the system. We as users want AI as optional. When I hold the power button to turn off my tablet, Bixby, the AI assistant, pops out

Blynk and the non-sovereign IoT devices - Manufacturers build devices without displays or without any way to control them without apps and the internet. Some allow at least basic control. We can do better.

Open-source with teeth - How I plan to release my software to the people. Always open source, dual license, delayed code push at the release (Android AOSP model, Unreal Engine...). This could be posted also under Remo's channel, given it's Ravenville philosophy.

Rich colorful displays on devices that need simplicity - Why Rich UI is a dead-end on the IoT market most of the time? Set up once and keep using. Text UIs, monochromatic OLEDs as a cheap and durable alternative

Arduino - great as a hobby, very bad for production - Unmaintained libraries, forks of forks,...

Why I want to use Zephyr Project

ESP IDF as a clean way to program Espressif hardware

Why I try to minimize dependencies on Arduino? ESP native libraries, logger, pros and cons, maintainability 

Dependency management with Arduino. PlatformIO and the Arduino IDE

Continuous integration with Github Actions

Unit testing an embedded hardware in Github Actions and QEMU

Why you should virtualize your hardware? Renode as a tool

RISC-V and why I want to switch from ESP32

Building Text UI interfaces with TcMenu

Why developing custom protocols is rarely a good thing? TcMenu post mortem

Small teams should integrate open standards, not reinvent the wheel

How I tweaked a smart home platform (Home Assistant) to control a smart Henhouse

Why Raspberry Pi is not good as a real-time microcontroller? Why dual-chip boards with PLC and a Linux core are the perfect solution?

Localization and internationalization challenges in the embedded world - memory constraints, no standard solution (Arduino), dates, units (metric, imperial)

Why you should have a real RTC clock?

Why we are building robust hardware that doesn't kill hens during Amazon cloud outage?

Embedded needs NuxtJS of the web world

Protobuf and GRPC, not JSON. How to save prescious memory when implementing server communication

Debugging and profiling your board with PlatformIO

Why I think that embedded worlds needs "Home Assistant components" to deliver stable firmware rapidly

How to write and build your documentation using Github Actions

Why you should learn Markdown yesterday

Why you should learn Git without using graphical user interface

GitHub, GitLab and why I use Gitea

What taught me embedded development after spending 6 years architecting a smart henhouse?

Why I would rewrite our Henhouse firmware from scratch? Arduino platform limitations, hidden bugs, worse or lacking support, unmaintained code, hardware evolution introduced code changes as we progressed

Supporting multiple variants of development hardware boards. How I ended up reinventing device trees in Arduino

Async programming with TaskManager (TcMenu framework library)

Abstracting device IO with TcMenu's IoAbstraction

Why betting on an open framework developed by one developer was a mistake and how I ended up maintaining the official project and patching workarounds. TcMenu in Hentower story

Open API or your own cloud? Companies want clouds and mine data, customers want open API but don't know it yet

Firmware flavors, modular firmware and conditional features

Why setting up WiFi via small embedded display is a UX nightmare and how I solved it without an app. Onboarding in embedded world

How I architected device pairing with the cloud? Hint: I got inspired with my Xbox

Why as an Android developer I got fed up with making Android apps. It's often just a fancy frontend UI for the backend

Why I love Compose Multiplatform and why Kotlin is my choice to build open-source ecosystems

Digital course platform providers don't care about security or your content protection. They care about marketing. Sarastro LMS proposal

Hollywood built their closed-source streaming platforms. Why do we need an open alternative?

Don't be evil - Why I decided to adopt Google's abandoned philosophy

Game preservation, language preservation, culture preservation - From an open-source developer to an archivist of our culture

Ravenville Summer of Code

Quarkus and gRPC as the perfect server backend for your embedded devices

ACDU - our hardware made for a client that turned out a versatile boardTcMenu framework and code generation for embedded platforms

Adeon - Embedded device control over SMS, custom protocol format, memory leaks and crashes: Post-mortem

RaceDuino - A prototype we never finished. How I would architect the firmware today?

My minimum requirements for a well designed git repository - License, readme, badges, CI/CD, pull request and issue templates...

Modbus - Master, Slave and why I ended up using custom libraries instead of ESP IDF solution.Why every Android team should have shared components libraries

Why I love modular Android architecture

How I pushed experimental Compose Multiplatform as the solution used for EU Digital Wallet implementation in Slovakia

What stress-testing of a mobile wallet solution taught me

OpenWallet and EUDIW - Two solutions for the same problem. Do we have problem at all or we are just building a solution to a non-existing problem?

How was it like to work for a government as a contractor and how it differs from normal clients

Why I am leaving Windows as a serious platform for workMicrosoft is adapting update installs schedule to save CO2 emissions but they are Ok with e-waste caused by stupid Windows 11 requirements

What needs to happen so that Linux phones are actually usable as daily drivers

We are in another .com bubble, it's called AI

How we assign unique serial numbers without rebuilding the firmware

Firmware updates via SD cardOTA updates using Github infrastructure

Automated firmware builds and flashing scripts... How to hand out binaries, not your source code

SD card loggerCLI interface

RFID reader library - how I implemented an Arduino library that makes a chinese RFID reader work

Using Arduino that is 600 kilometers away - remote agent, pros and issues - remote desktop, camera, lights...

RTC clock

Network manager

SD card logger

ArduinoLog and ANSI color

Arduino/PlatformIO  build processPlatformIO hooks

PlatformIO as a warning - closed PRs because the company doesn't fund the project

Building sovereign infrastructure for early stage startup cheaply. Storage server, emails, VPN, firewall, no SaaS...

Why Founders Should Invest in Technical Architecture Early

Reinventing device tree - How we supported multiple hardware revisions in our firmwareWhy JSON is a terrible idea in the embedded world and what we end up using instead?

Why buying a new phone doesn't make much sense and how I restored my OnePlus with Lineage OS.

Why I switched from Mikrotik and Qnap to open source solutions - compatibility, fixing bugs by myself...

Why I train my employees to learn git and MarkdownWhy you should know how to use git via terminal.

My $0/Month Sovereign Cloud: How I Built a Geo-Redundant Private Infrastructure Across Two Cities”or

“Why I Built My Own Personal Cloud Instead of Paying for Google Drive

Microsoft Windows as anti sovereign operating system. OneDrive turned off reported to users as an error and security risk.

Microsoft literally optimizes Windows updates to lower CO2 emissions but they don't care about electronic junk after Windows 10 end of support. Why Windpws 11 requirements are good only for business but unnecessarily high...

Why proprietary software becomes fragile - (One toggle in Unicode support should never break an accounting suite.)

Why sovereign systems don’t rely on registry-based state - (Windows continues to be the least transparent OS in existence.)

Handling “dark” bug clusters - (How to debug systems that fail for non-obvious reasons.)

Why local business software needs sandboxing - (Kros is the opposite of containerized design.)

Why sovereignty requires controlled friction

How to do backups of accounting data when the software backups at the same drive? People think their data is safe. Kros accounting product suite story.

Fragmented IoT ecosystem, integration, Open API