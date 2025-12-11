# Changelog

All notable changes to the IGSC (International Game Studio Classification) will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) for specification releases.

---

## [Unreleased]

### Planned
- Self-classification rubric tool
- Badge/certification assets
- Case study examples
- Real-world validation of project rating combination methodology
- Meta-grades for studios/publishers (e.g., "AA-producing studio")

---

## [0.4.0] - 2025-12-11

### Major Conceptual Shift: Projects Are Rated, Not Studios

This release represents a fundamental evolution in the IGSC framework, transitioning from studio classification to project-based rating using bond-style nomenclature.

### Added
- **Bond-Style Rating Scale**: Full AAA/AA/A/BBB/BB/B/CCC/CC/C nomenclature with +/- modifiers
  - Section 4.2: Explanation of bond rating origins in financial markets and applicability to games
  - Preserves industry-familiar terminology (AAA/AA/A) while adding formal structure
- **Source Rating Methodology** (Section 4.3):
  - Studios, publishers, and funders are now rated as independent "sources"
  - Sources combine to produce project ratings
  - Same studio can have multiple projects with different ratings
- **Studio Source Tier Definitions** (Section 6.1):
  - AAA Studio: 200+ staff, multiple departments, proven AAA track record (e.g., Ubisoft Montreal, EA DICE)
  - AA Studio: 80-200 staff, full departmental structure (e.g., Larian pre-BG3, IO Interactive)
  - A Studio: 30-80 staff, emerging departments
  - BBB Studio: 15-30 staff, first commercial title shipped
  - BB Studio: 10-15 staff, mix of FT/contractors
  - B Studio: 5-10 people, mostly part-time
  - CCC/CC/C Studio: 1-4 people, hobbyist/part-time
  - Each tier includes indicators, examples, and modifier guidance (+/-)
- **Publisher/Funder Source Tier Definitions** (Section 6.2):
  - AAA Publisher: $50M+ budgets, global reach (e.g., Sony, Microsoft, EA)
  - AA Publisher: $5M-$30M budgets (e.g., Devolver, Annapurna, Private Division)
  - A Publisher: $1M-$5M budgets (e.g., Raw Fury, Fellow Traveller)
  - BBB/BB/B/C Publisher tiers with financial scale and support services
- **Project Rating Combination Methodology** (Section 7.3):
  - **Recommended Approach**: Weighted Floor-and-Ceiling Model
  - Studio: 50-60% weight (capability foundation)
  - Publisher: 30-40% weight (resources/reach)
  - Other sources: 10-20% weight (supplementary)
  - Transparent explanation of alternative approaches considered
- **New Source Types** (Section 5.3):
  - Platform holder support (ID@Xbox, PlayStation Partners, Epic MegaGrants)
  - Regional/government grants (Film Victoria, Creative Europe, CMF, UK Games Fund)
  - Community funding (Kickstarter, Patreon, Fig)
  - Technology partners (Epic, Unity, middleware licensing deals)
- **source-rating-criteria.md**: Standalone reference document for studio/publisher source ratings
- New use case (Section 8.6): Platform Curation and Discovery

### Changed
- **Document subtitle**: "A Multi-Dimensional Taxonomy for Game Studios and Projects" → "A Bond-Style Rating System for Game Projects"
- **Executive Summary**: Completely rewritten to reflect project-based rating approach
- **Section 4 (The Framework)**: Restructured with four subsections explaining source-based methodology
- **Section 5 (Classification Dimensions)**: Restructured to "Source Rating Dimensions" with studio/publisher/funder sources
- **Section 6 (Tier Definitions)**: Massively expanded with comprehensive studio and publisher source tiers
- **Section 7 (How Classification Works)**: Renamed to "How Project Rating Works", completely rewritten
- **Section 8 (Use Cases)**: All examples updated to use project rating tiers (C/B, BB/BBB, A, AA/AAA)
- **Section 9.4 (HCS Comparison)**: Updated comparison table to include "Bond-style ratings" dimension
- **Section 10 (Design Principles)**: New principle 10.6 "Project-Centric, Not Studio-Centric"
- **Section 12 (Call to Adoption)**: Completely rewritten with project-centric framing for all stakeholder groups
- **Section 13 (References)**: Added new subsection "Financial Rating Systems" with citation flag for S&P/Moody's/Fitch
- **Tier nomenclature throughout**: Micro/Small/Mid/Large replaced with AAA/AA/A/BBB/BB/B/C bond ratings

### Fixed
- Removed duplicate content (lines 557-1110 were duplicate of lines 1-557)

### Design Philosophy
- **Projects receive ratings based on combined sources**: A solo developer (C Studio) with AAA publisher backing produces an A-rated project
- **Cultural alignment**: Bond rating scale (AAA/AA/A/BBB/BB/B/C) leverages existing industry vocabulary while adding formal structure
- **Transparent methodology**: Combination formula presented as recommended approach with clear explanation of alternatives
- **Multi-project flexibility**: Studios can have concurrent projects with different ratings based on resource allocation
- **Financial markets precedent**: Bond ratings provide proven framework for evaluating risk/capacity through letter grades

### Breaking Changes
- Previous tier names (Micro/Small/Mid/Large) fully replaced with bond rating scale
- Classification shifted from entity-centric (studios) to project-centric
- Self-classification process now requires rating sources separately before combining

### Notes
- Combination methodology flagged as "subject to real-world validation"
- Future versions may introduce meta-grades for studios/publishers (e.g., "AA-producing studio")
- Version bumped to 0.4.0 to reflect significant conceptual evolution

---

## [0.3.1] - 2025-11-24

### Added
- Comprehensive citation coverage throughout IGSC-White-Paper.md:
  - **Introduction**: Newzoo 2024 market size ($188B), Video Game History Foundation on AAA/indie/AA term origins (Orland, 2024)
  - **Section 3.1**: Humble Games GDC Vault talk (2022), Dan Pearce/IGN quote
  - **Section 3.4**: Engadget, PC Gamer, Digital Trends coverage of Dave the Diver controversy (2023); director Jaeho Hwang quote via VGC
  - **Section 9.1**: SAG-AFTRA budget tier definitions, AIM/IMPALA independent label criteria, WordsRated Big Five statistics
  - **Section 9.2**: Steam Direct, ID@Xbox, PlayStation Partners, Nintendo Developer Portal details; IGDA DSS definition; The Game Awards and BAFTA eligibility criteria; Newzoo and Gamalytic classification methodologies
  - **Section 9.3**: Garda & Grabarczyk (2016) Game Studies article, Juul *Handmade Pixels* MIT Press (2019), GDC survey methodology, Game Developer magazine quotes
  - **Section 13**: Full References section populated with all citations

### Changed
- Section 9.2 platform programmes description clarified: platforms use unified programmes, not formal tiered systems
- Version bumped to 0.3.1

### Fixed
- All [CITATION NEEDED] markers in document body resolved with scholarly and industry sources

### Known Issues
- Document contains duplicate content (whitepaper text appears twice)—flagged for cleanup

---

## [0.3.0] - 2025-11-24

### Added
- New Section 9.4: HushCrasher Classification System (HCS) comparative analysis
  - Overview of HCS methodology (credits length + disk size clustering)
  - Comparison table: IGSC vs HCS across key dimensions
  - Analysis of complementary approaches
- New Section 11.1: How Standards Gain Authority
  - ESRB and PEGI adoption model analogy
  - Network effects explanation for standard adoption
- Second Core Principle in Section 4: "Classification must be prospective, not just retrospective"
- HCS citations to References section (Mayerowitz & Belzanne, 2025)

### Changed
- Section 4 "Core Principle" renamed to "Core Principles" (now two principles)
- Section 11 subsections renumbered (11.1-11.4 instead of 11.1-11.3)
- Version bumped to 0.3.0

### Notes
- Key differentiator established: IGSC is prospective (any development stage), HCS is retrospective (post-release only)
- HCS acknowledged as complementary market analysis tool, not competing framework

---

## [0.2.0] - 2025-11-23

### Added
- New Introduction/Context section with industry landscape and terminology history
- New Supporting Research & Comparative Analysis section with four subsections:
  - Industry Context (film, music, publishing comparisons)
  - Existing Game Industry Approaches (platforms, trade orgs, awards, market research)
  - Academic and Industry Research
  - Why Existing Approaches Fall Short (comparison table)
- New References section with structured placeholder categories
- 15+ [CITATION NEEDED] flags with guidance on appropriate source types

### Changed
- Table of Contents updated to reflect 13 sections (previously 10)
- All sections renumbered to accommodate new Introduction section
- Replaced 11 em dashes with appropriate punctuation (colons, semicolons, parentheses)
- Document structure now fully aligns with White Paper Construction Guide

### Notes
- Citation flags are placeholders requiring research to populate
- Supporting Research section framework needs expansion with actual findings

---

## [0.1.0] - 2025-11-23

### Added
- Initial IGSC White Paper (v1.0 Draft)
- Two-layer classification model (Structural + Outcome)
- Team size tiers: Micro, Small, Mid, Large
- Ownership types: Independent, Affiliated, Owned
- Funding source categories: Self-funded, Grant, Publisher, Investor
- Production scope tiers: Small, Medium, Large, Massive
- Outcome classification dimensions: Revenue, Player Base, Critical Reception, Growth Signals
- Design principles: Voluntary, No Sensitive Disclosure, Transparent, Neutral, Lifecycle-aware, Global
- Use cases: Awards, Scouting, Grants, Analysis, Self-understanding
- CC BY 4.0 licensing

### Notes
- This is the initial draft release for public feedback
- Tier thresholds may be refined based on community input
- Revenue bands are illustrative and may be adjusted

---

## Version Numbering

- **Major versions (1.0, 2.0)** — Significant changes to classification structure or tiers
- **Minor versions (0.1, 0.2)** — Clarifications, additions, refinements
- **Patch versions (0.1.1)** — Typo fixes, formatting, non-substantive changes
