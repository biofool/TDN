# Technical Marketing Summary — TDN (Truthiness Discovery Network)

## One-Line Positioning

A conceptual framework for a decentralized public ledger that tracks media provenance and truthiness ratings, enabling real-time authenticity assessment of digital media.

## Target Users / Personas

- **Media consumers** who need to assess the authenticity of news, videos, and images in real time
- **Fact-checking organizations** (e.g., RD2020 network) seeking a public infrastructure for sharing provenance data
- **Media platform developers** building players that query a truthiness ledger
- **Policy makers and journalists** concerned about deep fakes and misinformation

## Key Features (Grounded in Code)

- **Public ledger concept** — decentralized tracking of media provenance, expert ratings, and commentary (described in `README.md`)
- **Threat model** — OWASP Threat Dragon diagram documenting security considerations (`ThreatDragonModels/Test/Test.json`)
- **Privacy-enhancing proxy reference** — Privoxy 3.0.28 source code included as a reference for the filtering/proxy component of the envisioned architecture (`privoxy-3.0.28-stable/`)
- **GitHub Pages site** — Jekyll-configured site with tactile theme for project documentation (`_config.yml`)

## Technical Differentiators

- **Real-time truthiness** — vision of media players querying a public ledger at presentation time, not after-the-fact fact-checking
- **Decentralized and public** — no single authority controls the provenance data
- **Leverages existing fact-checking infrastructure** — designed to complement, not replace, organizations like RD2020
- **Privacy-first proxy layer** — Privoxy reference suggests a filtering/proxy approach to media consumption

## Use Cases

- A media player that displays a "truthiness score" alongside a video, sourced from the public ledger
- Fact-checkers contributing provenance data and expert commentary to a shared public ledger
- Content platforms integrating ledger queries to flag potentially manipulated media
- Researchers analyzing media provenance patterns

## Benefits / Value Proposition

- Moves fact-checking from reactive to real-time — consumers see truthiness scores as media is presented
- Decentralized design avoids single points of control or censorship
- Complements existing fact-checking infrastructure rather than duplicating it
- Open and public — anyone can query or contribute to the ledger

## Tech Stack

- **Reference proxy**: Privoxy 3.0.28 (C)
- **Threat modeling**: OWASP Threat Dragon
- **Documentation site**: Jekyll (tactile theme) via GitHub Pages
- **Conceptual architecture**: Decentralized public ledger (design phase)

## Known Limitations

- **Conceptual/design phase only** — no runnable application, ledger, or API exists yet
- **No implementation** — the repository contains only the concept description, a threat model, and reference source code
- **Privoxy inclusion is unexplained** — the relationship between Privoxy and the TDN architecture is not documented
- **No API specification** — the ledger query/write protocol is not defined
- **No consensus mechanism** — how the decentralized ledger reaches agreement is unspecified
