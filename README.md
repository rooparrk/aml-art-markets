# Graph Analytics & Entity Resolution: Art Markets, PEPs, & Corporate Shells

[![Portfolio](https://img.shields.io/badge/Portfolio-Roo's%20Observatory-amber?style=flat-square)](https://roo-s-observatory.vercel.app)
[![Pipeline Status](https://img.shields.io/badge/Pipeline-Phase%201%20In%20Progress-vibrantgreen?style=flat-square)]()
[![Domain](https://img.shields.io/badge/Domain-Financial%20Systems%20Intelligence-blue?style=flat-square)]()

---

## I. Strategic Context & Workspace Topology

This repository houses the automated entity resolution and relational network graph engine designed to surface hidden transaction pathways within structurally opaque asset environments. By cross-referencing messy public auction data, offshore leaked corporate nodes, and international risk registries, this pipeline transitions asset-layering investigations from manual, text-heavy oversight into deterministic string alignment and network topology modeling.

```text
    [ Raw Data Vault: ICIJ / Auction / PEP ] 
                       │
                       ▼
         [ Deterministic Text Cleaner ] ──> ( Strip Suffixes, Inversions, Whitespace )
                       │
                       ▼
        [ RapidFuzz Token Sort Engine ] ──> ( Calculates Matrix Intersections )
                       │
                       ▼
          [ Structural Graph Build ]   ──> ( NetworkX / igraph Node Topology )
                       │
                       ▼
     [ Compliance Mapping Matrix (MAS) ] ──> High-Betweenness Centrality Flags
```

### Repository Blueprints
* [cite_start]`notebooks/`: Active workspace containing data parsing, algorithmic string matching, and network generation loops[cite: 810].
* [cite_start]`data/`: Protected infrastructure split into `raw/` ingestion dumps and `processed/` master intersection ledgers[cite: 811].
* [cite_start]`outputs/`: Container reserved for compiled directed network visualizations and centrality vector mappings[cite: 812].
* [cite_start]`docs/`: Regulatory mapping ledgers aligning surfaced graph clusters to actionable compliance alerts[cite: 813].

---

## II. Pipeline Methodology & String Matching Mathematics

[cite_start]The operational core of this engine relies on a modular ingestion architecture that standardizes unstructured string variants before passing them to a vector-optimized scoring matrix[cite: 814].

### 1. Deterministic Normalization
[cite_start]To prevent corporate suffixes and localized syntax noise from artificially inflating match confidence scores, raw strings undergo strict string preprocessing[cite: 815]:

$$\text{String}_{\text{Normalized}} = \text{Lower}\left(\text{RegexRemove}\left(\text{String}_{\text{Raw}}, \text{Suffixes} \cup \text{Punctuation}\right)\right)$$

### 2. Algorithmic Token Alignment
[cite_start]Standard Levenshtein distance fails when encountering structural name inversions (e.g., `"Vladimir Potanin"` vs. `"Potanin, Vladimir"`)[cite: 816]. [cite_start]To bypass this limitation, the engine enforces a Token Sort Ratio calculation[cite: 817]. [cite_start]Ingested names are tokenized, alphabetized, and reconciled back to a unified string primitive to isolate the fundamental distance metric[cite: 818]:

$$\text{Match Score} = \text{TokenSortRatio}\left(\text{Entity}_{\text{Target}}, \text{Entity}_{\text{Reference}}\right)$$

### 3. Resolution Risk Thresholds
[cite_start]A standard linear baseline is discarded[cite: 819]. [cite_start]To control false-positive tracking spikes while systematically capturing hidden relationships, a hard thresholding matrix is enforced[cite: 820]:

* **Score $\ge$ 90%**: Deterministic Flag. [cite_start]Automatic mapping into the master processed ledger[cite: 820, 821].
* **Score 85% – 89%**: High-Probability Risk. [cite_start]Isolated for secondary structural verification across the network graph layers[cite: 821, 822].
* **Score < 85%**: Administrative Noise. [cite_start]Discarded automatically to minimize pipeline friction[cite: 822, 823].

---

## III. Execution Instructions

### Technical Core
* [cite_start]**Language:** Python 3.11+ [cite: 824]
* [cite_start]**Primary Libraries:** `pandas`, `rapidfuzz`, `networkx`, `matplotlib` [cite: 824]

### Getting Started
[cite_start]To prepare your environment, install the direct C-compiled string optimization engine and required dependencies[cite: 750, 824]:

```bash
pip install rapidfuzz pandas openpyxl networkx
```

---
[cite_start]Part of a digital ecosystem showcasing financial systems intelligence at [Roo's Observatory](https://roo-s-observatory.vercel.app)[cite: 796].
