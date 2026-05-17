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
* `notebooks/`: Active workspace containing data parsing, algorithmic string matching, and network generation loops.
* `data/`: Protected infrastructure split into `raw/` ingestion dumps and `processed/` master intersection ledgers.
* `outputs/`: Container reserved for compiled directed network visualizations and centrality vector mappings.
* `docs/`: Regulatory mapping ledgers aligning surfaced graph clusters to actionable compliance alerts.

---

## II. Pipeline Methodology & String Matching Mathematics

The operational core of this engine relies on a modular ingestion architecture that standardizes unstructured string variants before passing them to a vector-optimized scoring matrix.

### 1. Deterministic Normalization
To prevent corporate suffixes and localized syntax noise from artificially inflating match confidence scores, raw strings undergo strict string preprocessing:

$$\text{String}_{\text{Normalized}} = \text{Lower}\left(\text{RegexRemove}\left(\text{String}_{\text{Raw}}, \text{Suffixes} \cup \text{Punctuation}\right)\right)$$

### 2. Algorithmic Token Alignment
Standard Levenshtein distance fails when encountering structural name inversions (e.g., `"Vladimir Potanin"` vs. `"Potanin, Vladimir"`)[cite: 816]. [cite_start]To bypass this limitation, the engine enforces a Token Sort Ratio calculation. Ingested names are tokenized, alphabetized, and reconciled back to a unified string primitive to isolate the fundamental distance metric:

$$\text{Match Score} = \text{TokenSortRatio}\left(\text{Entity}_{\text{Target}}, \text{Entity}_{\text{Reference}}\right)$$

### 3. Resolution Risk Thresholds
A standard linear baseline is discarded. To control false-positive tracking spikes while systematically capturing hidden relationships, a hard thresholding matrix is enforced:

* **Score $\ge$ 90%**: Deterministic Flag. Automatic mapping into the master processed ledger.
* **Score 85% – 89%**: High-Probability Risk. Isolated for secondary structural verification across the network graph layers.
* **Score < 85%**: Administrative Noise. Discarded automatically to minimize pipeline friction

---

## III. Execution Instructions

### Technical Core
* **Language:** Python 3.11+ 
* **Primary Libraries:** `pandas`, `rapidfuzz`, `networkx`, `matplotlib` 

### Getting Started
To prepare your environment, install the direct C-compiled string optimization engine and required dependencies:

```bash
pip install rapidfuzz pandas openpyxl networkx
```

---
Part of a digital ecosystem showcasing financial systems intelligence at [Roo's Observatory](https://roo-s-observatory.vercel.app).
