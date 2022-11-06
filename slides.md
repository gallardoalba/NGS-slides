
####  Introduction to big data analysis in bioinformatics WS 22/23

### **Concepts in sequencing data analysis**

<sub><sub>Cristobal Gallardo Alba</sub></sub>

------

<img src="img/no_phone.jpg" alt="drawing" width="600"/>

---

<span class="menu-title" style="display: none">Table of contents</span>

<div style="text-align: left">

## Table of contents

<br>

- **Sequencing technologies**
- **Information storage**
- **Applications of sequencing**

</div>

------

<div style="text-align: left">

## Table of contents

<br>

- **Sequencing technologies**
    - NGS technologies: Illumina
    - TGS technologies: Nanopore & PacBio
- <span style="color:#B3B3B3">**Information storage**</span>
- <span style="color:#B3B3B3">**Applications of sequencing**</span>

</div>

------

<div style="text-align: left">

## Table of contents

<br>
    
- <span style="color:#B3B3B3">**Sequencing technologies**</span>
- **Information storage**
    - Phred quality score
    - FASTQ format
- <span style="color:#B3B3B3">**Applications of sequencing**</span>

</div>

------

<div style="text-align: left">

## Table of contents

<br>
    
- <span style="color:#B3B3B3">**Sequencing technologies**</span>
- <span style="color:#B3B3B3">**Information storage**</span>
- **Applications of sequencing**
    - Genome assembly
    - Transcriptomics: gene expression analysis
    - Epigenetics

</div>

---

<span class="menu-title" style="display: none">Sequencing technologies</span>

## Sequencing technologies

------

<span class="menu-title" style="display: none">NGS technology: Illumina</span>

### NGS technology: Illumina

<img src="https://www.intechopen.com/media/chapter/49419/media/image2.png" alt="drawing" width="600"/>

<p style="font-size:14px;">Source: https://www.intechopen.com/</p>    

Note:
    
This sequencing method is based on reversible dye-terminators that enable the identification of single nucleotides.
  
With this technology, thousands of places throughout the genome are sequenced at once via massive parallel sequencing.

------

### NGS technology: Illumina
#### Base calling

<div class="r-stack">
  <img class="fragment fade-out" data-fragment-index="0" src="img/base_calling_01.png" alt="drawing" width="800"/>
  <img class="fragment current-visible" data-fragment-index="0" src="img/base_calling_02.png" alt="drawing" width="1000"/>
</div>



------

<span class="menu-title" style="display: none">TGS technology: Oxford Nanopore</span>

### TGS technology: Oxford Nanopore

<img src="https://www.ukaachen.de/fileadmin/files/institute/humangenetik/_processed_/b/1/csm_nanopore_sequenzierung_c643920a66.jpg" alt="drawing" width="900"/>

<p style="font-size:14px;">Source: https://www.ukaachen.de</p>    

------

### TGS technology: Oxford Nanopore
#### Base calling

<img src="img/nanopore_basecalling.jpg" alt="drawing" width="1000"/>

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

------

### Information storage: Phred quality score

<img src="img/per_base_quality.png" alt="drawing"  width="600"/>

------

<span class="menu-title" style="display: none">Information storage: SAM/BAM datatype</span>

### Information storage: SAM/BAM datatypes

<br>

<img src="img/sam.png" alt="drawing"/>

---

<span class="menu-title" style="display: none">Applications of sequencing technologies</span>

## Applications of sequencing technologies

------

<span class="menu-title" style="display: none">Genome assembly</span>

### Genome assembly
    
<img src="img/genome_assembly.png" alt="drawing" width="1000"/>

------

### Genome assembly
#### VGP assembly workflow
    
<img src="img/VGP_workflow.png" alt="drawing" width="1000"/>

------

### Genome assembly
#### VGP assembly workflow in Galaxy

<div style="text-align:left; font-size:28px">

- The VGP-Galaxy project has assembled 26 genomes in the last 6 months
- Largest: 4Gbp *Gastrophryne carolinensis*

</div>

<img src="img/gastrophryne.png" alt="drawing" width="500"/>

------

<span class="menu-title" style="display: none">Transcriptomics: expression analysis</span>

### Transcriptomics: RNA-seq

<img src="img/transcription.jpg" alt="drawing" width="1000"/>

differential_expression.png

------

### Transcriptomics: RNA-seq
#### Differential expression analysis pipeline

<img src="img/differential_expression.png" alt="drawing" width="500"/>

------

### Transcriptomics: RNA-seq
#### Differential expression analysis

<img src="img/DE_plots.png" alt="drawing" width="1000"/>

------

<span class="menu-title" style="display: none">Epigenetics</span>

### Epigenetics

<a href="https://imgflip.com/i/6zn61x" ><img src="https://i.imgflip.com/6zn61x.jpg"  width="600"/></a>

------

<span class="menu-title" style="display: none">DNA/RNA methylation</span>

### Epigenetics
#### Heritable marks: DNA/RNA methylation

<img src="img/methylation.jpg" alt="drawing" width="1000"/>

<small>DNA/RNA methylation **regulates gene expression** by recruiting proteins involved in gene repression or by inhibiting the binding of transcription factor(s) to DNA.</small>

------

### Epigenetics
#### Heritable marks: DNA/RNA methylation

<img src="img/paper_methylation.png" alt="drawing"/>

------

<span class="menu-title" style="display: none">Cancer molecular markers</span>

### Epigenetics
#### Cancer molecular markers

<img src="img/cancer_methylation.png" alt="drawing" width="700"/>

------

### Epigenetics
#### Cancer molecular markers

<img src="img/cancer_genes.png" alt="drawing" width="900"/>

------

<span class="menu-title" style="display: none">Plant resistance to extreme conditions</span>

### Epigenetics
#### Plant resistance to extreme conditions

<img src="img/plants_methylation.png" alt="drawing" width="700"/>

<small><small>Plant stress memory and their capacity to influence plant tolerance to a changing environment and crop productivity is considered to play an important role in the adaptation and evolution of plants.</small></small>

------

### Epigenetics
#### Plant resistance to extreme conditions

<img src="img/lysenko.png" alt="drawing" width="1000"/>

<small><small>"Environment-induced changes are the primary mechanism of heritability." -- Trofim Denisovich Lysenko (1898-1976)</small></small>

------

<span class="menu-title" style="display: none">Neurodegenerative disorders</span>

### Epigenetics
#### Neurodegenerative disorders

