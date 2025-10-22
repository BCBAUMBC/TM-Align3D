This repository provides an interactive notebook that compares two protein structures using **TM-score** and **RMSD (Root Mean Square Deviation)**, and visualizes their 3D alignment. It’s ideal for computational biologists, structural bioinformaticians, or anyone working on protein modeling and analysis.

---

## Overview

Protein structure comparison is essential for understanding evolutionary relationships, structural similarity, and function prediction.  
This notebook allows you to:

- Compute **TM-score** to measure **global topological similarity** between two protein structures.
- Compute **RMSD** to quantify **geometric deviation** after structural superposition.
- Visualize the **3D structural alignment** using molecular visualization libraries.

---

## Metrics Explained

### **TM-score**
- A **length-independent** metric that measures the topological similarity between two protein structures.
- Introduced by Yang Zhang & Jeffrey Skolnick (2005).  
  _"TM-align: a protein structure alignment algorithm based on the TM-score."_  
  **Nucleic Acids Research, 33(7), 2302–2309.**
- **Interpretation:**
  - **TM-score > 0.5** → Generally indicates similar folds.
  - **TM-score < 0.3** → Typically indicates unrelated structures.

### **RMSD (Root Mean Square Deviation)**
- Measures the **average atomic deviation** between equivalent atoms after optimal superposition.
- **Lower RMSD values** indicate higher structural similarity.
- Sensitive to local deviations, while TM-score captures global fold similarity.

---

## Features

- Compare any two PDB structures.  
- Compute **TM-score** and **RMSD** in seconds.  
- **3D visualization** of aligned structures using interactive molecular viewers (e.g., `py3Dmol` or `nglview`).
- Copare & visualize in monomer and multimer mode.
- Sequence alignment.
- Easy to extend — integrate with AlphaFold models or local PDB datasets.  

---

## Requirements

Install the required dependencies before running the notebook:
<img width="908" height="702" alt="image" src="https://github.com/user-attachments/assets/5c50c155-651b-4111-9b22-eebfb44e06c8" />
<img width="2151" height="260" alt="image" src="https://github.com/user-attachments/assets/293ddfaf-c248-459a-b4c5-f55147c9c761" />
<img width="912" height="733" alt="image" src="https://github.com/user-attachments/assets/4c1c2bf5-1ccf-43fe-85f6-6361eb7c3380" />
```bash
pip install biopython py3Dmol numpy scipy


