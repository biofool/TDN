# TDN — Truthiness Discovery Network

A conceptual project exploring a decentralized public ledger for media provenance, truthiness ratings, and expert commentary — enabling consumers to assess the authenticity of media in real time.

## Overview

TDN (Truthiness Discovery Network) addresses the challenge of deep fakes, fake news, and misinformation by proposing a public ledger that tracks media provenance, expert ratings, and commentary. The vision is that media players would query this ledger when presenting content, allowing consumers to understand a piece of media's "truthiness" in real time.

The repository currently contains:
- A conceptual README describing the project vision
- A Threat Dragon threat model diagram (`ThreatDragonModels/`)
- The Privoxy 3.0.28 source code (a privacy-enhancing web proxy), included as a reference/dependency for the network architecture

## Prerequisites

- For reviewing the threat model: [OWASP Threat Dragon](https://owasp.org/www-project-threat-dragon/)
- For building Privoxy: standard C build tools (gcc, make, autoconf)
- Ruby and Jekyll (for GitHub Pages site, configured via `_config.yml`)

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/biofool/TDN.git
   cd TDN
   ```

2. To view the threat model, open `ThreatDragonModels/Test/Test.json` in OWASP Threat Dragon.

3. To build Privoxy (included as reference source):
   ```bash
   cd privoxy-3.0.28-stable
   ./configure
   make
   ```

4. To serve the GitHub Pages site locally:
   ```bash
   bundle exec jekyll serve
   ```

## How to Run

This is primarily a conceptual/design-phase project. There is no runnable application yet. The Privoxy source is included as a reference for the proxy/filtering component of the envisioned architecture.

## Project Structure

```
TDN/
├── README.md                          # Project vision and concept description
├── _config.yml                        # Jekyll configuration (tactile theme)
├── ThreatDragonModels/
│   └── Test/
│       └── Test.json                  # OWASP Threat Dragon threat model
└── privoxy-3.0.28-stable/             # Privoxy web proxy source code (reference)
    ├── AUTHORS, ChangeLog, LICENSE
    ├── Makefile, GNUmakefile.in
    ├── actionlist.h, actions.c, actions.h
    ├── cgi.c, cgi.h, cgiedit.c, cgisimple.c
    ├── client-tags.c, client-tags.h
    └── ... (full Privoxy source tree)
```

## Key Features

- Conceptual framework for decentralized media provenance tracking
- Public ledger design for truthiness ratings and expert commentary
- Threat model diagram (OWASP Threat Dragon format)
- Privoxy source included as reference for privacy-enhancing proxy infrastructure
