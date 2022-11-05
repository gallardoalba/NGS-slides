
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

<span class="menu-title" style="display: none">Custom Menu Title</span>

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

<img src="img/base_calling_01.png" alt="drawing" width="800"/>

------

### NGS technology: Illumina
#### Base calling

<img src="img/base_calling_02.png" alt="drawing" width="1000"/>

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

### File formats: FASTQ

<img src="img/FASTQ_format.png" alt="drawing"/>

------

<span class="menu-title" style="display: none">File formats: Phred score</span>

### File formats: Phred quality score

<pre><code data-trim data-noescape >
@ERR4760040.1 MN00415:74:FREIBURG:1
TATAGCTCGCAAATCGTATCAGCAGATGTAATCAGGTAATGAAGTAGTTCTAGTTCTAGTTCTA
+
&%%)'/5516:;-,*&,)+1.-3(+-)%&+623196366-+-')*029==*029==*029==*0
</code></pre>

<div style="text-align: left">

Phred quality score is used to indicate the measure of base quality in DNA sequencing.<br>

</div>

$$
Q = -10\log_{10}p \rightarrow p = 10^{\frac{-Q}{10}}
$$

<br><small>*p: error probability associated with any given basecall*</small><br>
<small>*Q: quality score, encoded in ASCII characters*</small>

------

### File formats: Phred quality score

<img src="img/per_base_quality.png" alt="drawing"  width="600"/>

---

<span class="menu-title" style="display: none">Applications of sequencing technologies</span>

## Applications of sequencing technologies

------

<span class="menu-title" style="display: none">Genome assembly</span>

### Genome assembly
    
<img src="img/genome_assembly.png" alt="drawing" width="1000"/>

------

<span class="menu-title" style="display: none">Genome assembly</span>

### Genome assembly
#### VGP assembly workflow
    
<img src="img/VGP_workflow.png" alt="drawing" width="1000"/>

------

<span class="menu-title" style="display: none">Genome assembly</span>

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

------

<span class="menu-title" style="display: none">Epigenetics</span>

### Epigenetics

<a href="https://imgflip.com/i/6zn61x" ><img src="https://i.imgflip.com/6zn61x.jpg"  width="600" title="made at imgflip.com"/></a>

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

------

<span class="menu-title" style="display: none">Neurodegenerative disorders</span>

### Epigenetics
#### Neurodegenerative disorders

------

<span class="menu-title" style="display: none">Abuse substance</span>

### Epigenetics
#### Molecuar basis of substance abuse
