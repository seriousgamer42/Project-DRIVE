# Project-DRIVE
**Disc Ripping for Interactive Video Entertainment**

Project DRIVE is an open-source utility designed to back up legally owned game discs for preservation, archival, and personal use.

The goal of DRIVE is to create a modular, scalable disc dumping tool that supports multiple generations of optical-based consoles while remaining transparent, verifiable, and community-driven.

---

# ⚠ Legal Notice

Project DRIVE does **not** support piracy.

This software is intended strictly for:
- Backing up legally owned discs
- Preservation efforts
- Research and archival purposes

Users are responsible for complying with local laws.

---

# 🎯 Project Goals

- Provide accurate, verified disc dumps
- Support multiple console generations
- Maintain clean, modular architecture
- Offer both CLI and GUI interfaces
- Integrate hash verification (Redump-compatible where possible)
- Be beginner-friendly but powerful

---

# 🗺 Development Roadmap

---

## Phase 0 – Foundation

**Objective:** Build core architecture.

- [ ] Define modular disc I/O abstraction layer
- [ ] Implement raw sector reading engine
- [ ] Logging system
- [ ] Hashing support (MD5, SHA1, CRC32)
- [ ] ISO output formatting
- [ ] Error handling & retry logic
- [ ] Cross-platform compatibility (Windows first)

Deliverable:
- Functional CLI tool capable of reading standard CD/DVD data discs

---

## Phase 1 – Standard Disc Support (Low Barrier)

**Target Consoles:**
- PlayStation (PS1)
- PlayStation 2 (CD/DVD titles)
- PC CD/DVD games

Focus:
- Redump-style verification
- Multi-track CD support
- Cue/Bin handling
- Layer break detection (DVD9)

Deliverable:
- Reliable CD/DVD dumping with verification
- Verified output matching known hashes

---

## Phase 2 – Wii & GameCube Support

**Target Consoles:**
- Nintendo GameCube
- Nintendo Wii

Requirements:
- Compatible optical drives (e.g., specific LG models)
- Scrambled sector handling
- Wii partition parsing
- Decryption research layer (legal-safe modular design)

Deliverable:
- Verified GameCube/Wii ISO extraction
- Partition awareness

---

## Phase 3 – Original Xbox Support

**Target Console:**
- Xbox (2001)

Challenges:
- Non-standard filesystem (XDVDFS)
- Drive firmware constraints
- Potential need for modified hardware interface

Deliverable:
- Full-disc XDVDFS image dump
- Filesystem parser module

---

## Phase 4 – Advanced & Research Tier

**Target Consoles (Research-Based):**
- Xbox 360
- PlayStation 3
- Wii U
- Blu-ray-based systems

Focus:
- Documentation
- Hardware research
- Legal-safe modular plugin architecture
- Preservation tooling

Note:
This phase prioritizes research transparency over guaranteed implementation.

---

## Phase 5 – GUI & Accessibility

- Cross-platform GUI frontend
- Disc auto-detection
- One-click verified dumping
- Metadata scraping (optional)
- Drive capability diagnostics
- Beginner mode vs Advanced mode

---

# 🧠 Architecture Vision

DRIVE will follow a modular plugin structure:

drive/
├── 📁 core
│   ├── 📁 io
│   ├── 📁 hashing
│   └── 📁 logging
│
├── 📁 platforms
│   ├── 📁 ps1
│   ├── 📁 ps2
│   ├── 📁 wii
│   ├── 📁 gamecube
│   └── 📁 xbox
│
└── 📁 frontend
    ├── 📁 cli
    └── 📁 gui

This allows:
- Console-specific modules
- Easier community contributions
- Legal isolation of experimental components

---

# 🔍 Verification Philosophy

Whenever possible, DRIVE will:

- Generate full-disc hashes
- Support Redump-style verification
- Preserve raw sector accuracy
- Avoid altering disc structure

Preservation > Convenience

---

# 🛠 Tech Stack (Proposed)

- Python (Core logic)
- C/C++ modules (optional performance layer)
- PyQt or similar (GUI)
- Native OS optical drive APIs

---

# 🤝 Contributing

Contributions are welcome.

Please:
- Follow clean code practices
- Document research thoroughly
- Avoid distributing copyrighted content
- Focus on preservation and legality

---

# 🚀 Long-Term Vision

Project DRIVE aims to become:

- A preservation-focused alternative to closed-source dumping tools
- A research hub for optical disc archival
- A scalable framework that can expand as technology evolves

---

**Preserve the past. Build the future.**