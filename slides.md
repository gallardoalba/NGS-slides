
####  Introduction to big data analysis in bioinformatics WS 22/23

### **Concepts in sequencing data analysis**

<sub><sub>Cristobal Gallardo Alba</sub></sub>

------

<img src="img/no_phone.jpg" alt="drawing" width="600"/>

---

<span class="menu-title" style="display: none">Table of contents</span>

<div style="text-align: left">

### Table of contents

- <span class="fragment highlight-current-red" style="font-size:40px">**Sequencing technologies**</span>
    - <span class="fragment highlight-current-red" style="font-size:30px">NGS technologies: Illumina</span>
    - <span class="fragment highlight-current-red" style="font-size:30px">TGS technologies: Nanopore & PacBio</span>
- <span class="fragment highlight-current-red" style="font-size:40px">**Information storage**</span>
    - <span class="fragment highlight-current-red" style="font-size:30px">FASTQ datatype</span>
    - <span class="fragment highlight-current-red" style="font-size:30px">Phred quality score</span>
    - <span class="fragment highlight-current-red" style="font-size:30px">SAM/BAM datatype</span>
- <span class="fragment highlight-current-red" style="font-size:40px">**Applications of sequencing**</span>
    - <span class="fragment highlight-current-red" style="font-size:30px">Genome assembly</span>
    - <span class="fragment highlight-current-red" style="font-size:30px">Transcriptomics: gene expression analysis</span>
    - <span class="fragment highlight-current-red" style="font-size:30px">Epigenetics</span>

</div>

---

<span class="menu-title" style="display: none">Sequencing technologies</span>

## Sequencing technologies

------

<span class="menu-title" style="display: none">NGS technology: Illumina</span>

### NGS technology: Illumina

<div class="r-stack">
<span class="fragment fade-out" data-fragment-index="0">
<img src="https://www.intechopen.com/media/chapter/49419/media/image2.png" alt="drawing" width="600"/>
<p style="font-size:14px;">Source: https://www.intechopen.com/</p>    
</span>
<span class="fragment" data-fragment-index="0">

#### Base calling

<div class="r-stack">
<img class="fragment fade-out" data-fragment-index="1" src="img/base_calling_01.png" alt="drawing" width="800"/>
<img class="fragment current-visible" data-fragment-index="1" src="img/base_calling_02.png" alt="drawing" width="1000"/>
</div>
</span>
</div>

Note:
    
This sequencing method is based on reversible dye-terminators that enable the identification of single nucleotides.
  
With this technology, thousands of places throughout the genome are sequenced at once via massive parallel sequencing.

------

<span class="menu-title" style="display: none">TGS technology: Oxford Nanopore</span>

### TGS technology: Oxford Nanopore

<div class="r-stack">
<span class="fragment fade-out" data-fragment-index="0">
<img src="img/oxford_nanopore.jpg" alt="drawing" width="1000"/>
<p style="font-size:14px;">Source: https://www.ukaachen.de</p>    
</span>
<span class="fragment" data-fragment-index="0">

#### Base calling

<img src="img/nanopore_basecalling.jpg" alt="drawing" width="1000"/>

</span>
</div>

------

<span class="menu-title" style="display: none">TGS technologies: PacBio</span>

### TGS technologies: PacBio

<img src="img/pacbio.png" alt="drawing" width="800"/>

---

<span class="menu-title" style="display: none">Information storage</span>

## Information storage

------

<span class="menu-title" style="display: none">File formats: FASTQ</span>

### Information storage: FASTQ datatype

<img src="img/FASTQ_format.png" alt="drawing"/>

------

<span class="menu-title" style="display: none">File formats: Phred score</span>

### Information storage: Phred quality score

<div class="r-stack">
<span class="fragment fade-out" data-fragment-index="0">

<pre><code data-trim data-noescape >
@ERR4760040.1 MN00415:74:FREIBURG:1
TATAGCTCGCAAATCGTATCAGCAGATGTAATCAGGTAATGAAGTAGTTCTAGTTCTAGTTCTA
+
&%%)'/5516:;-,*&,)+1.-3(+-)%&+623196366-+-')*029==*029==*029==*0
</code></pre>

<div style="text-align: left">

Phred quality score is used to indicate the measure of base quality in DNA/RNA sequencing.<br>

</div>

$$
Q = -10\log_{10}p \rightarrow p = 10^{\frac{-Q}{10}}
$$

<br><small>*p: error probability associated with any given basecall*</small><br>
<small>*Q: quality score, encoded in ASCII characters*</small>

</span>
<span class="fragment current-visible" data-fragment-index="0">

<img src="img/per_base_quality_02.png" alt="drawing"  width="700"/>

</span>
<span class="fragment">

<img src="img/per_base_quality.png" alt="drawing"  width="700"/>

</span>
</div>

------

<span class="menu-title" style="display: none">Information storage: SAM/BAM datatype</span>

### Information storage
#### SAM/BAM datatype

<br>

<img src="img/sam.png" alt="drawing"/>

---

<span class="menu-title" style="display: none">Applications of sequencing technologies</span>

## Applications of sequencing technologies

------

<span class="menu-title" style="display: none">Genome assembly</span>

### Genome assembly

<div class="r-stack">
<span class="fragment fade-out" data-fragment-index="0">
<img src="img/dna_structure.jpg" alt="drawing" width="1000"/>
<p style="font-size:14px;">Source: https://www.genome.gov</p>    
</span>
<span class="fragment" data-fragment-index="0">
<img src="img/genome_assembly.png" alt="drawing" width="1000"/>
</span>
</div>

------

### Genome assembly
#### VGP *de novo* assembly workflow

<div class="r-stack">
<span class="fragment fade-out" data-fragment-index="0">

<img src="img/VGP_workflow.png" alt="drawing"/>

</span>
<span class="fragment current-visible" data-fragment-index="0">

<div style="text-align:left; font-size:28px">

- The VGP-Galaxy project has assembled 26 genomes in the last 6 months
- Largest: 4Gbp *Gastrophryne carolinensis*

</div>

<img src="img/gastrophryne.png" alt="drawing" width="800"/>

</span>
</div>

------

### Genome assembly
#### Within-species variation: resequencing

<div class="r-stack">
<span class="fragment fade-out" data-fragment-index="0">

<img src="img/within_specie_variation.png" alt="drawing" width="1200"/>

<small><small>The butterfly genus *Heliconius* contains some species that are extremely difficult to tell apart.</small></small>

</span>
<span class="fragment current-visible" data-fragment-index="0">

<img src="img/resequencing.jpg" alt="drawing" width="700"/>

<small><small>Source: nature.com</small></small>

</span>
</div>

------

<span class="menu-title" style="display: none">Transcriptomics: expression analysis</span>

### Transcriptomics: RNA-seq

<img src="img/transcription.jpg" alt="drawing" width="800"/>

<small><small>Source: metrics-lab.github.io</small></small>

------

### Transcriptomics: RNA-seq
#### Expression genetics in cancer

<img src="img/transcriptome_cancer.jpg" alt="drawing" width="1000"/>

------

### Transcriptomics: RNA-seq
#### Differential expression analysis pipeline

<div class="r-stack">
<span class="fragment fade-out" data-fragment-index="0">

<img src="img/differential_expression.png" alt="drawing" width="500"/>

</span>
<span class="fragment current-visible" data-fragment-index="0">

<img src="img/DE_plots.png" alt="drawing" width="1000"/>

<small><small>Source: nature.com</small></small>

</span>
</div>

------

### Epigenetics

<a href="https://imgflip.com/i/6zn61x" ><img src="https://i.imgflip.com/6zn61x.jpg"  width="600"/></a>

------

<span class="menu-title" style="display: none">Epigenetics</span>
    
### Epigenetics

<div class="r-stack">
<span class="fragment fade-out" data-fragment-index="0">

Epigenetics is the study of **stable and inheritable phenotypic changes** that do not involve alterations in the DNA sequence.

<div style="text-align: left">
<br>

It involves multiple mechanisms:
    
- Covalent modifications (e.g. DNA/RNA methylation)
- Histone positioing
- Histone variants
- Many more!

</div>
</span>
<span class="fragment current-visible" data-fragment-index="0" style="font-size:40px">
<div style="text-align: left">

Detection requires usually  a three-phase strategy:

<br>

- Conversion of epigenetic into genetic information
    - Usually by biochemical methods
- High-throughput sequencing
- Computational and statisticall analysis

</div>

</span>
</div>

------

<span class="menu-title" style="display: none">DNA/RNA methylation</span>

### Epigenetics
#### Covalent modifications: DNA/RNA methylation

<div class="r-stack">
<span class="fragment fade-out" data-fragment-index="0">

<img src="img/methylation.jpg" alt="drawing" width="1000"/>

<small>DNA/RNA methylation **regulates gene expression** by recruiting proteins involved in gene repression or by inhibiting the binding of transcription factor(s) to DNA.</small>

</span>
<span class="fragment current-visible" data-fragment-index="0">
<img src="img/bisulfite_sequencing.jpg" alt="drawing" width="800"/>
<small><small>Bisulfite sequencing involves the deamination of unmodified cytosines to uracil.</small></small>
</span>
</span>
<span class="fragment">
<img src="img/paper_methylation.png" alt="drawing"/>
</span>
</div>

------

<span class="menu-title" style="display: none">Cancer molecular markers</span>

### Epigenetics
#### Covalent modifications: Cancer molecular markers

<div class="r-stack">
<span class="fragment fade-out" data-fragment-index="0">

<img src="img/cancer_methylation.png" alt="drawing" width="700"/>

</span>
<span class="fragment current-visible" data-fragment-index="0">

<img src="img/cancer_genes.png" alt="drawing" width="900"/>

<small><small>Source: nature.com</small></small>

</span>
</div>

------

<span class="menu-title" style="display: none">Plant resistance to extreme conditions</span>

### Epigenetics
#### Covalent modicitations: Plant resistance to extreme conditions

<div class="r-stack">
<span class="fragment fade-out" data-fragment-index="0">

<img src="img/plants_methylation.png" alt="drawing" width="700"/>

<small><small>Plant stress memory and their capacity to influence plant tolerance to a changing environment and crop productivity is considered to play an important role in the adaptation and evolution of plants.</small></small>
    
</span>
<span class="fragment current-visible" data-fragment-index="0">

<img src="img/lysenko.png" alt="drawing" width="1000"/>

<small><small>"Environment-induced changes are the primary mechanism of heritability." -- Trofim Denisovich Lysenko (1898-1976)</small></small>

</span>
</div>

------

<span class="menu-title" style="display: none">Neurodegenerative disorders</span>

### Epigenetics
#### Covalent modifications: Neurodegenerative disorders

