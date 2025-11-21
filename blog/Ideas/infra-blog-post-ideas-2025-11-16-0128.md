# Infrastructure Blog Post Ideas
**Date:** November 16, 2025  
**Time:** 1:28

This document captures blog post concepts arising from the upcoming Ravenville infrastructure rebuild. These ideas will later be added to the broader list of ~70 content topics and then prioritized.

---

## 1. Rebuilding a Sovereign Private Cloud From Scratch
How I redesigned my entire digital infrastructure using TrueNAS, OPNsense, WireGuard, Gitea, Vaultwarden, and internal DNS. A deep look into building a long-term, maintainable, zero-trust network.

## 2. Designing a Zero-Trust Network for a One-Person Studio
A practical guide to creating a secure, VPN-only access architecture even when you are the only user today — but planning for a future team.

## 3. Why I Removed All My Internal Services From the Public Internet
The reasoning behind moving Nextcloud, Gitea, Vaultwarden, and TrueNAS behind WireGuard. Reduced attack surface, full sovereignty, and a quieter network.

## 4. Building a Password and Secrets Infrastructure for a Small Team
Deploying Vaultwarden, designing organizational vaults, and separating personal vs business identity. Sharing OTP codes, backup keys, and credentials securely.

## 5. My Disaster Recovery Plan: How I Protect Canon and Core Work
A full breakdown of the DR strategy: encrypted USB sticks, Faraday cage, offline PGP, physical copies, and operational instructions for worst-case scenarios.

## 6. The Case for Self-Hosted Git: Why I Migrated to Gitea
A discussion on public vs internal repos, Git LFS for images, separation from GitHub, and why sovereign Git hosting matters for creative studios.

## 7. Migrating from Raspberry Pi to a Real Firewall Appliance
Lessons learned moving from Pi 4 to an N100 mini PC running OPNsense. Realtek NIC considerations, routing performance, and future scalability.

## 8. The Role of WireGuard in a Modern Private Cloud
Always-on VPNs, low overhead, seamless device syncing, and how WireGuard becomes a central pillar of the entire studio network.

## 9. How I Partition My World: Identity Firewalls in a Founder’s Digital Life
A conceptual explanation of separating Personal vs Vladimír vs Remo vs Ravenville vs Client realms — supported by cryptography and system architecture.

## 10. Reinstalling Arch Linux: Why I Periodically Wipe and Rebuild
A philosophy + technical post about why clean environments matter, especially when building long-term projects, and how I configure my workstation.

## 11. Internal DNS: The Hidden Backbone of a Private Studio
Creating a private DNS zone for internal services (`vault.raven.internal`, `git.raven.internal`), separating public identity from internal architecture.

## 12. Infrastructure as Meditation
A more raw, personal reflection about why rebuilding systems is my form of rest, clarity, and sovereignty.

## 13. The TrueNAS Layout I Wish I Built Earlier
A deep-dive into datasets, permissions, snapshots, client partitions, and clean subvolume design.

## 14. Why Consultants Should Build Their Own Infrastructure
A philosophical post on credibility, lived expertise, and why consulting from experience beats theoretical advice every time.

## 15. Lutemi Smart Henhouse: Architecture Lessons From My IoT Project
A standalone post that ties your IoT work (PlatformIO, ESP32, Modbus, async pairing, backend architecture) into a broader theme of practical engineering.

---

**These topics will be merged with the main idea backlog and prioritized based on impact, readiness, and alignment with your March–April focus window.**