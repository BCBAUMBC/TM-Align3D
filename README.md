# TM-Align 3D

[<img width="547" height="440" alt="TM-Align 3D view 1" src="https://github.com/user-attachments/assets/6e00eb6c-9ef0-4d04-a7b5-5d38d3f8d900" />](https://colab.research.google.com/drive/1NDKRAKhoP-4nNgY9BKrkRlqRELzlGVoU#scrollTo=56ba9447)

<img width="2151" height="260" alt="Sequence alignment" src="https://github.com/user-attachments/assets/293ddfaf-c248-459a-b4c5-f55147c9c761" />

## 🔗 Launch Notebook
[<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"/>](https://colab.research.google.com/drive/1NDKRAKhoP-4nNgY9BKrkRlqRELzlGVoU#scrollTo=56ba9447)




## Overview

This notebook has two primary functionalities:

1. **Structure Alignment and Comparison** — Calculate **TM-score** and **RMSD** between two protein structures using **ProDy** and **tmtools**.
2. **3D Visualization** — Display aligned structures interactively with **py3Dmol**, using **biopython** for file handling and sequence parsing.

Our workflow guides users through three stages:  
- loading or fetching structures,  
- computing TM-score and RMSD for quantitative comparison, and  
- visualizing structural overlap in 3D.

We demonstrate the notebook with examples comparing the **Human apo ferritin** and a **Bullfrog M ferritin** to illustrate how TM-score and RMSD reflect global and local similarity between protein folds.

---

## Metrics Explained

### **TM-score**
- A **length-independent** metric that measures the topological similarity between two protein structures.
- Introduced by Yang Zhang & Jeffrey Skolnick (2005).  
  _"TM-align: a protein structure alignment algorithm based on the TM-score."_  
  **Nucleic Acids Research, 33(7), 2302–2309.**
- **Interpretation:**
  - **TM-score > 0.75** → Indicates strong similarity
  - **TM-score > 0.5** → Generally indicates similar folds.
  - **TM-score < 0.3** → Typically indicates unrelated structures.
    
  <img width="668" height="174" alt="image" src="https://github.com/user-attachments/assets/8649e27c-e0e8-45f3-9f44-8d3490222639" />
 


### **RMSD (Root Mean Square Deviation)**
- Measures the **average atomic deviation** between equivalent atoms after optimal superposition.
- **Lower RMSD values** indicate higher structural similarity.
- Sensitive to local deviations, while TM-score captures global fold similarity.
<img width="317" height="131" alt="image" src="https://github.com/user-attachments/assets/bca8b08f-6670-4138-ae92-0e3dfeb34bae" />

---

## Features

- Compare any two PDB structures.  
- Compute **TM-score** and **RMSD** in seconds.  
- **3D visualization** of aligned structures using interactive molecular viewers (e.g., `py3Dmol`.
- Compare & visualize in monomer and multimer mode.
- Sequence alignment.
- Easy to test your own generated structures.
---




