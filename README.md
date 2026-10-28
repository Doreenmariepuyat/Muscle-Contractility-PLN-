# Molecular Mechanisms of Muscle Contractility: PLN p.Arg14del

## 1. Project Information

- **Assignment number:** 32
- **Gene symbol:** PLN
- **Gene name:** Phospholamban
- **Organism:** *Homo sapiens*
- **Reference transcript:** NM_002667.5
- **Reference protein:** NP_002658.1
- **Assigned variant:** NM_002667.5:c.37AGA[1] (p.Arg14del), as listed in the laboratory manual
- **ClinVar Variation ID:** 44580
- **Variant type:** In-frame deletion
- **Programming language:** R
- **Packages:** rentrez and ggplot2

## 3. Methods

### 3.1 Project Setup

A project folder named `Muscle_Contractility_PLN` was created in RStudio. The project was organized into `data/`, `results/`, and `figures/` folders. The R packages `rentrez` and `ggplot2` were used for retrieving NCBI records and generating figures.

### 3.2 Retrieval of the PLN Gene and Protein

The human PLN gene record was retrieved from NCBI Gene using R and the `rentrez` package. The exact gene record was checked, and its Gene ID, official name, chromosome, and biological role were recorded in `results/gene_summary.txt`.

The assigned transcript, NM_002667.5, was retrieved from NCBI Nucleotide. Its GenBank record was used to identify the corresponding RefSeq protein accession, NP_002658.1. The reference protein sequence was retrieved in FASTA format and saved as `data/PLN_protein.fasta`. The accession was recorded in `results/protein_accession.txt`.

### 3.3 Amino-Acid Composition Analysis

The reference protein FASTA sequence was read into R. The protein length and the frequencies of the 20 standard amino acids were calculated. The results were saved in `results/amino_acid_composition.csv`. A bar chart was generated using ggplot2 and saved as `figures/01_amino_acid_composition.png`.

### 3.4 ClinVar Variant Verification

The assigned variant was examined using NCBI ClinVar, Variation ID 44580. The variant description, protein change, variant class, associated conditions, clinical classification, review status, and available supporting evidence were reviewed. The database access date was recorded.

### 3.5 Protein Position Mapping

A linear protein map was generated in R using ggplot2. The figure displayed the full reference PLN protein length and marked amino-acid position 14, the position affected by p.Arg14del. The figure was saved as `figures/02_variant_position.png`.

## Results

### Gene and Reference Protein

- **Gene:** PLN
- **Official name:** Phospholamban
- **NCBI Gene ID:** 5350
- **Reference transcript:** NM_002667.5
- **Reference protein accession:** NP_002658.1
- **Reference protein length:** 52 amino acids

Phospholamban is a regulatory protein involved in calcium handling, particularly in cardiac muscle. It regulates SERCA, a calcium pump that returns calcium to the sarcoplasmic reticulum and helps the muscle relax after contraction.

### Amino-Acid Composition

The reference protein sequence contained 52 amino acids. Based on the generated bar chart, the three most abundant amino acids were:

1. **Leucine (L):** 10 residues
2. **Isoleucine (I):** 8 residues
3. **Glutamine (Q):** 5 residues

Other amino acids were present at lower frequencies, and some standard amino acids had zero counts in the reference sequence.

**Figure 1. Amino-acid composition of the human PLN reference protein.**

The bar chart shows the number of occurrences of each of the 20 standard amino acids in the 52-amino-acid reference phospholamban sequence, NP_002658.1. Leucine was the most frequent amino acid, followed by isoleucine and glutamine. This chart describes the sequence composition but does not independently establish the protein's function or the effect of the assigned variant.

![Figure 1: PLN amino-acid composition](figures/01_amino_acid_composition.png)

### Variant Position

The assigned p.Arg14del variant affects arginine at amino-acid position 14 of the reference PLN protein. It is an in-frame deletion, meaning that the deletion does not shift the downstream reading frame.

**Figure 2. Linear protein map showing the position affected by PLN p.Arg14del.**

The gray line represents the full-length reference PLN protein of 52 amino acids. The red marker identifies position 14, where arginine is deleted in the assigned variant. This map shows the affected position on the reference sequence and does not independently demonstrate a change in protein structure or function.

![Figure 2: PLN p.Arg14del protein-position map](figures/02_variant_position.png)

### ClinVar Findings

- **ClinVar Variation ID:** 44580
- **Variant:** p.Arg14del (R14del)
- **Variant class:** In-frame deletion
- **Aggregate germline classification:** Pathogenic
- **Aggregate review status:** Criteria provided, multiple submitters, no conflicts
- **Associated conditions reported:** Dilated cardiomyopathy and other cardiomyopathy-related conditions
- **Database accessed:** [Enter your access date]

ClinVar includes reports of affected individuals, family segregation, and functional studies supporting a disease association. The exact evidence and classification should be interpreted using the current record and its linked publications.

## Discussion

Phospholamban (PLN) is a small regulatory protein that plays an important role in calcium handling in cardiac muscle. It regulates the sarcoplasmic reticulum calcium ATPase (SERCA), which transports calcium from the cytoplasm back into the sarcoplasmic reticulum. This process helps lower cytoplasmic calcium after contraction and supports cardiac muscle relaxation.

In this project, the human PLN reference transcript NM_002667.5 was used to retrieve the corresponding reference protein, NP_002658.1. Analysis in R showed that the reference protein contains 52 amino acids. The amino-acid composition chart showed that leucine was the most abundant residue, with 10 occurrences, followed by isoleucine with 8 and glutamine with 5. These results describe the sequence composition but cannot independently explain the protein's three-dimensional structure, molecular interactions, or the effect of a variant.

The assigned p.Arg14del variant removes an arginine residue at position 14 without shifting the downstream reading frame. The protein-position map identifies the affected location on the reference sequence. However, the map itself is not experimental evidence of altered protein function.

The current ClinVar record classifies p.Arg14del as pathogenic and summarizes evidence from affected individuals, family segregation, and functional studies. Published functional studies have reported that this variant disrupts phospholamban function and can inhibit SERCA activity. These findings support a mechanism involving abnormal calcium regulation, which may impair normal cardiac muscle function. Clinical observations and laboratory experiments provide different kinds of evidence: association with cardiomyopathy in affected individuals supports clinical relevance, while functional studies investigate the molecular mechanism.

A possible causal chain is: PLN variant → altered phospholamban function → abnormal regulation of SERCA → disturbed calcium handling → possible impairment of cardiac contraction and relaxation. The sequence analysis and figures in this project do not directly test each step of this chain.

A useful follow-up experiment would compare cells expressing wild-type PLN with cells expressing p.Arg14del. Measurements of SERCA activity or calcium reuptake could test whether the variant alters calcium handling. Appropriate controls and biological replicates would be needed. Overall, the project combines sequence analysis, variant mapping, and database evidence while distinguishing computational results from experimentally observed effects.

## References and Database Links

1. **NCBI Gene:** https://www.ncbi.nlm.nih.gov/gene/
2. **NCBI RefSeq transcript NM_002667.5:** https://www.ncbi.nlm.nih.gov/nuccore/NM_002667.5
3. **NCBI RefSeq protein NP_002658.1:** https://www.ncbi.nlm.nih.gov/protein/NP_002658.1
4. **NCBI ClinVar, Variation ID 44580:** https://www.ncbi.nlm.nih.gov/clinvar/variation/44580/
5. Haghighi, K. et al. (2006). A mutation in the human phospholamban gene, deleting arginine 14, results in lethal, hereditary cardiomyopathy. *Proceedings of the National Academy of Sciences*. [Find article via PubMed](https://pubmed.ncbi.nlm.nih.gov/16432188/).

**Database access date:** [October 27, 2026]

<img width="596" height="320" alt="image" src="https://github.com/user-attachments/assets/d90c94ae-d38a-4fcd-9569-ccfa52b36be8" />

<img width="848" height="175" alt="image" src="https://github.com/user-attachments/assets/25964917-3622-42a6-a8a5-6446eaf82b51" />

<img width="770" height="502" alt="image" src="https://github.com/user-attachments/assets/ed0002df-99c0-4e7c-9bea-e23c4ad59b52" />

