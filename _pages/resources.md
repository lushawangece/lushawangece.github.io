---
layout: archive
title: "Resources"
permalink: /resources/
author_profile: true
---


<!-- ### DistFileConv {#distfileconv}
Lightweight tool to convert distribution-system files (e.g., CYME ↔ OpenDSS, JSON/CSV) using NREL DiTTo.

<p><a class="btn btn--primary" href="https://github.com/lushawangece/DistFileConv">GitHub</a></p> -->

### DistFileConv {#distfileconv}

A lightweight converter for **distribution-system feeder models**, designed to move real-world utility data into analysis-friendly formats. DistFileConv sits on top of NREL’s DiTTo model so you can standardize inputs and prototype studies quickly.

**What it does**
- Converts **CYME text exports → OpenDSS** (primary focus), with optional **JSON/CSV** tabular outputs for quick inspection.
- Preserves key feeder structure (buses, lines, phases), common load and capacitor attributes, and basic regulator representations.
- Logs unmapped elements and writes a short conversion **summary** so you can spot data gaps fast.
- Works on **single feeders or batches** of folders.

**Why it’s useful**
- Speeds up research workflows where collaborators use different tools (CYME in utility, OpenDSS in academia).
- Produces human-readable artifacts (JSON/CSV) that are easy to diff, validate, and version-control.
- Designed with **reproducibility** in mind—same inputs → same outputs.

**Current status**
- Early research tool; validated on several real feeders with **1ɸ/2ɸ/3ɸ** sections.
- Not intended to be a perfect round-trip translator; advanced device models (protection, detailed regulator controls, GIS layers) may be simplified.
- Roadmap: GridLAB-D import, OpenDSS→JSON improvements, packaged CLI (`pipx`) for one-command use.

**Requirements**
- Python 3.9+; DiTTo backend; common scientific Python stack (e.g., pandas, numpy).
- Cross-platform (Windows/macOS/Linux).

**Get it**
- GitHub: https://github.com/lushawangece/DistFileConv  
  (README includes install notes and examples.)


<!-- <p>
  <a class="btn btn--primary" href="REPO_URL">GitHub</a>
  <a class="btn" href="DOCS_URL">Docs</a>
  <a class="btn" href="REPO_URL/issues">Issues</a>
</p>

**Install**
```bash
# pick one
pip install distfileconv
# conda
# conda install -c conda-forge distfileconv -->