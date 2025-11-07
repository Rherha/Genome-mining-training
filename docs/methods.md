# Detailed Methodology

## Genome Source
- **Organism:** *Streptomyces coelicolor* A3(2)
- **NCBI Accession:** AL645882.2
- **Size:** 8,667,507 bp (8.67 Mb)
- **Download:** https://www.ncbi.nlm.nih.gov/nuccore/AL645882.2

## Analysis Pipeline

### Step 1: Genome Download
Downloaded complete genome in GenBank format from NCBI.

### Step 2: antiSMASH Analysis
- **Tool:** antiSMASH 7.0
- **Platform:** Galaxy (usegalaxy.eu)
- **Date:** November 2025

**Parameters:**
```
Taxon: Bacteria
All detection modules enabled:
- KnownClusterBlast ✓
- ClusterBlast ✓
- SubClusterBlast ✓
- ActiveSiteFinder ✓
- RREFinder ✓
- CompaRiPPson ✓
```

### Step 3: Data Extraction
- Downloaded HTML output
- Manually extracted BGC information
- Created structured data table

### Step 4: Prioritization
Scoring system based on:
1. BGC type (polyene, lipopeptide, NRPS = high priority)
2. Novelty (<50% similarity = novel)
3. Known antifungal activity

### Step 5: Literature Validation
Cross-referenced findings with:
- MIBiG database
- Published literature
- Known antifungal compounds

## Tools Used
- antiSMASH 7.0
- Galaxy platform
- LibreOffice Calc
- Reference managers
```

4. Commit

---

#### **File: data/genome_info.txt**

1. Navigate to `data/`
2. Create: `genome_info.txt`
3. Paste:
```
Genome Information
==================

Organism: Streptomyces coelicolor A3(2)
NCBI Accession: AL645882.2
RefSeq: NC_003888.3

Assembly Details:
- Type: Complete genome
- Length: 8,667,507 bp (8.67 Mb)
- GC Content: 72.12%
- Topology: Linear chromosome
- Plasmids: SCP1 (356 kb), SCP2 (31 kb)
- Protein-coding genes: 7,825

Source:
- Isolation: Soil, United Kingdom
- First sequenced: 2002 (Bentley et al., Nature)
- Model organism for Streptomyces biology

Download:
https://www.ncbi.nlm.nih.gov/nuccore/AL645882.2

Analysis Date: November 2025
```
