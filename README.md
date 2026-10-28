# Molecular Mechanisms of Muscle Contractility: PLN p.Arg14del
**Student:** Puyat, Doreen Marie G.

- **Gene symbol:** PLN
- **Gene name:** Phospholamban
- **Organism:** *Homo sapiens*
- **Reference transcript:** NM_002667.5
- **Reference protein:** NP_002658.1
- **Assigned variant:** NM_002667.5:c.37AGA[1] (p.Arg14del), as listed in the laboratory manual
- **ClinVar Variation ID:** 44580
- **Variant type:** In-frame deletion


## Methods

**Gene Retrieval**. Searched NCBI Gene for human PLN and recorded the gene ID, gene name, chromosome, and normal function.

<img width="596" height="320" alt="image" src="https://github.com/user-attachments/assets/d90c94ae-d38a-4fcd-9569-ccfa52b36be8" />

**Protein retrieval**. Retrieved transcript NM_002667.5 and its corresponding protein reference sequence, NP_002658.1, using R and NCBI resources. Saved the protein FASTA file in data/.

<img width="1335" height="363" alt="image" src="https://github.com/user-attachments/assets/ab87a965-e752-4524-ba8f-23cbe281ee46" />

**Verified protein reference sequence and FASTA sequence with NCBI.**

<img width="848" height="175" alt="image" src="https://github.com/user-attachments/assets/25964917-3622-42a6-a8a5-6446eaf82b51" />



## Results




### Amino-Acid Composition

**Table 1.** Full amino‑acid composition of PLN (NP_002658.1; 52amino acids)

| AminoAcid | Count |
|-----------|------:|
| A         | 3     |
| C         | 3     |
| D         | 0     |
| E         | 2     |
| F         | 2     |
| G         | 0     |
| H         | 0     |
| I         | 8     |
| K         | 2     |
| L         | 10    |
| M         | 3     |
| N         | 2     |
| P         | 1     |
| Q         | 5     |
| R         | 4     |
| S         | 2     |
| T         | 2     |
| V         | 2     |
| W         | 0     |
| Y         | 1     |


![Figure 1: PLN amino-acid composition](figures/01_amino_acid_composition.png)

**Figure 1. Amino-acid composition of the human PLN reference protein.** The bar chart shows the number of occurrences of each of the 20 standard amino acids in the 52-amino-acid reference phospholamban sequence, NP_002658.1. Leucine was the most frequent amino acid, followed by isoleucine and glutamine. 

### Variant Position

The assigned p.Arg14del variant affects arginine at amino-acid position 14 of the reference PLN protein. It is an in-frame deletion, meaning that the deletion does not shift the downstream reading frame.

![Figure 2: PLN p.Arg14del protein-position map](figures/02_variant_position.png)

**Figure 2. Linear protein map showing the position affected by PLN p.Arg14del.** The gray line represents the full-length reference PLN protein of 52 amino acids. The red marker identifies position 14, where arginine is deleted in the assigned variant. 

## Second Biological Visualization

<img width="770" height="502" alt="image" src="https://github.com/user-attachments/assets/ed0002df-99c0-4e7c-9bea-e23c4ad59b52" />

**Figure 3. Linear protein map of human phospholamban (PLN) showing the location of the p.Arg14del variant.** The reference PLN protein (NP_002658.1) contains 52 amino acids. The red marker indicates the in-frame deletion of arginine at position 14.

# Step 7. Molecular Mechanism of the PLN p.Arg14del Variant

## 1. Describe what your normal protein does in skeletal, cardiac, or smooth muscle (as appropriate). Identify whether it drives the actin–myosin cycle, regulates calcium, or maintains musclestructure.

The PLN gene encodes phospholamban, a small protein that regulates calcium movement in cardiac muscle. It controls SERCA2a, a calcium pump that returns calcium to the sarcoplasmic reticulum after contraction. This helps the heart muscle relax before the next heartbeat. Phospholamban regulates calcium; it does not directly drive the actin–myosin cycle.

## 2. Explain what is known about the assigned variant, separating observed experimental evidencefrom computational prediction and clinical

The assigned variant, p.Arg14del (ClinVar Variation ID 44580), deletes arginine at amino-acid position 14 without shifting the reading frame.

- **Experimental evidence:** Studies have reported that this variant can disrupt phospholamban function and affect SERCA calcium-pump regulation.
- **Clinical evidence:** The variant is associated with inherited cardiomyopathy and is classified as Pathogenic in ClinVar.
- **Computational evidence:** The protein map shows the location of the deletion, but it does not prove how the variant affects protein function.

The exact mechanism and why disease severity differs among individuals remain incompletely understood.

## 3. Write a short causal chain: gene → protein → molecular function →assigned variant →possibleeffect on contraction, relaxation, or muscle integrity.

PLN gene → phospholamban protein → regulates SERCA2a and calcium reuptake → p.Arg14del removes arginine 14 → altered calcium handling → possible disruption of normal heart muscle contraction and relaxation → increased risk of cardiomyopathy.

## 4. Propose one experiment that could test your interpretation, such as ATPase measurement, calcium imaging, binding assay, microscopy, or force measurement.

Compare cardiac cells with normal phospholamban to cells with the p.Arg14del variant by measuring calcium levels with a fluorescent indicator. Now if the variant cells show changes in how quickly calcium is removed from the cytoplasm, this would support the idea that the variant affects calcium regulation.

## References

1. NCBI ClinVar. *PLN p.Arg14del, Variation ID 44580.* https://www.ncbi.nlm.nih.gov/clinvar/variation/44580/
2. Haghighi, K., et al. (2006). A mutation in the human phospholamban gene, deleting arginine 14, results in lethal, hereditary cardiomyopathy. *PNAS, 103*(5), 1388–1393. https://doi.org/10.1073/pnas.0510519103


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



