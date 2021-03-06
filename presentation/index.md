---
title       : Dermatology Branch Journal Club
subtitle    : 2013-06-28
author      : Kenneth Daily
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
url         : {lib: libraries}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax, bootstrap, quiz]
mode        : selfcontained # {standalone, draft}

---

## 

<img src="./assets/img/encode-header.jpg" alt="ENCODE" height=75>

### The ENcyclopedia Of DNA Elements Pilot Project (2003-2007)

- Following release of human genome sequence, April 2003

> - Identify and characterize sequence-based functional elements
  - Experimentally and computationally
> - 35 research groups, 200 data sets
> - Targeted analysis of 30Mb (1% of genome)

---

## Highlights (Nature, Vol 447, 14 June 2007)
### Identification and analysis of functional elements in 1% of the human genome by the ENCODE pilot project
- More transcription than previously identified
- Symmetric distribution of regulatory sequences around TSS's
- Characteristic histone modification patterns
- 5% of genome is under (mammalian) evolutionary constraint
- Many "functional", non-constrained sites (a pool of neutral elements)

---

## ENCODE as a data generation project
### From the 2007 ENCODE pilot project (doi:10.1038/nature05874)
> "In describing the major results and initial conclusions, we seek to distinguish ‘biochemical function’ from ‘biological role’. Biochemical function reflects the direct behaviour of a molecule(s), whereas biological role is used to describe the consequence(s) of this function for the organism.

> Genome-analysis techniques nearly always focus on biochemical function but not necessarily on biological role. This is because the former is more amenable to large scale data-generation methods, whereas the latter is more difficult to assay on a large scale."

---

## 
<center>
<img src="./assets/img/ENCODE_nature_cover.png" alt="ENCODE cover" width="45%">
</center>

---

## 

<img src="./assets/img/17448.png" alt="ENCODE" width=900>

PLoS Biol. 2011 Apr;9(4):e1001046. doi: 10.1371/journal.pbio.1001046

---

## 

<img src="./assets/img/encode-feature-graphic.jpg" alt="ENCODE" width=825>

Nature 489, 46–48 (06 September 2012) doi:10.1038/489046a

---

## Histone modifications predict expression

<img src="./assets/img/fig2b.png" alt="Figure 2b: Histone modifications and expression" width=825>

---

## Transcription factor co-association

<img src="./assets/img/fig4.png" alt="Figure 4: Transcription factor co-association" width="95%">

---

## Data integration and segmentation

<img src="./assets/img/fig5a.png" alt="Figure 5a: Data integration and segmentation" width="100%">

---

## Machine learning - self organizing map

<img src="./assets/img/fig7a.png" alt="Figure 7a: Machine learning on integrated data" width="80%">

---

## ENCODE results - self organizing map application

<img src="./assets/img/fig7c.png" alt="Figure 7c: Machine learning on integrated data" width=825>

---

## (Some of) ENCODE's strong statements

> Operationally, we define a __functional element__ as a discrete genome segment that encodes a defined product (for example, protein or non-coding RNA) or displays a reproducible biochemical signature (for example, protein binding, or specific chromatin structure).

> The vast majority (80.4%) of the human genome participates in at least one biochemical RNA- and/or chromatin-associated event in at least one cell type.

> 95% of the genome lies within 8Kb of a DNA-protein interaction.

> 99% is within 1.7Kb of at least one of the biochemical events measured by ENCODE.

> These estimates represent a lower bound, but reinforce the observation that there is __more non-coding functional DNA__ than either coding sequence or mammalian evolutionary conserved bases.

> change the way a lot of [genomics] concepts are written about and presented in textbooks

> I don't think anyone would have anticipated even close to the amount of sequence that ENCODE has uncovered that looks like it has functional importance

---

## 

<img src="./assets/img/graur_title.png" alt="Graur et al, title page" width=825>

--- &twocol

## A rebuttal of ENCODE

*** left

<img src="./assets/img/dan_graur_twitter.jpeg" alt="Dan Graur" width=350>

Molecular evolutionary biologist
https://twitter.com/DanGraur

*** right

### Starting off:
> The ENCODE Project Consortium assigns function to 80.4% of the genome. We disagree with this estimate.


- Definition of function is questionable
- Function is maintained in the absence of selection
- Methods favor sensitivity over specificity

---

## Selected effect vs. causal role

### Selected effect functions are historical and evolutionary
> The sequence "TATAAA" is maintained by natural selection to bind a transcription factor, resulting in the transcription of a gene.
>
>
> The selected effect function is binding a transcription factor.

<!---
Suggests a clear, conservative method for inference for function in DNA sequences; only sequences under selection can be claimed to be functional
--->


### Causal role functions are ahistorical and nonevolutionary

> Example: The sequence "TATAAT" mutates into "TATAAA" and subsequently bind a transcription factor, but does not result in the transcription of a gene.
> The "causal role function" is binding a transcription factor.

_The heart: a blood pump, or fancy paperweight?_

<!---
Graur, et al. argue that ENCODE takes this definition; thus, if a region is determined to be functional (by the assays) then no deleterious mutations can occur (even in the absence of observed sequence-based evolutionary pressure)
--->

---

## Wrong and inconsistent?
- Function according to ENCODE
  - be transcribed, associated with modified histone, located in an open chromatin area, bind a transcription factor or contain methylated CpG dinucleotide

**Are these functions, or simply genomic locations, features/properties related to nucleotide composition?**

- The ENCODE functional argument (affirming the consequent)
  1. "Functional" DNA segments tend to display a certain property.
  2. A DNA segment displays the same "property."
  3. Therefore, the DNA segment is "functional."

### Inconsistent, arbitrary percentages of amount of functional DNA (80%, 40%, 20%,...)

### 100% of genome replicates (a reproducible biochemical event!); so it's all functional!

---

## Transcription does not equal function
### Claim: 74.7% of the genome is transcribed (via RNA-Seq, CAGE-Seq, PET-Seq)
- Conclusion: every observed transcribed DNA is "functional"

<!---
The broadest element class represents the different RNA types, covering 62% of the genome (although the majority is inside of introns or near genes).
--->

### Problems
- Others estimate 90% of transcription is "noise"
- Cell lines used are transcription permissive (<a href='http://encodeproject.org/encode/cellTypes.html'>Cell types</a>)
  - A hallmark of ESC genome: transcriptionally globally hyperactive<br/>
  (<a href="http://www.ncbi.nlm.nih.gov/pmc/articles/PMC2435228/">doi:10.1016/j.stem.2008.03.021</a>)
  - HeLa cells are not representative of human cells (_Helacyton gartleri_)
- Allows DNA sequences WITHOUT a promoter to be transcribed
- Three major classes of transcribed elements that are not really functional


---

## Transcription does not equal function

### Pseudogenes
- 10% of pseudogenes are transcribed, often translated in tumor cells
- High level of mutations, not under functional constraint (negative selection)
- "Pseudogenes" that have been shown to be functional aren't pseudogenes!

### Introns
- Only 4% of primary transcripts are coding, but ALL transcript bases counted as functional
- 3% introns knocked out with negative growth effect yeast
- Exceptions - splice sites, regulatory elements, mirtrons (small percentage)

<!---
They do concede that introns are counted; though no numbers are given when they are excluded 
--->

### Mobile elements
- LINEs, SINES, retroviruses, transposons
- 2/3 of genome, 1/3 of transcriptome (e.g. Alu elements)
- Only functions are littering and causing frameshifts

---

## Histone modification does not equal function
- The "epigenetic code" - methylation, acetylation, phosporylation of histone tails
- How much variation in gene expression is explained by histone modifications?
  - Karlic et al. - 142 combinations of 3 modifications (out of ~8000)
  - 2% **statistically** significant
- ENCODE assigns function such as "5' end of genes" to H4K20me1

---

## Open chromatin does not equal function
- Defined as genomic DNAase I hypersensitive (DHS), or identified by FAIRE-Seq
  - They are nucleosome depleted
- 2.89 million DHSs (205K/cell type; tier 1, 2)
  - 98.5% of ENCODE ChIP-Seq peaks are in these regions
- 80% of TSSs were in open chromatin regions; two ways to view this:
  1. Most TSSs are in open chromatin regions, or
  2. __Most open chromatin regions are functional TSSs.__

<!--- Song et al - "Over 870,000 DNaseI or FAIRE sites, which correspond tightly to nucleosome-depleted regions, were identified across the seven cell lines, covering nearly 9% of the genome"..."Open chromatin common to all seven cell types tended to be at or near transcription start sites and to be coincident with CTCF binding sites, while open chromatin sites found in only one cell type were typically located away from transcription start sites and contained DNA motifs recognized by regulators of cell-type identity." --->

<!--- The protocol is based on the fact that the formaldehyde cross-linking is more efficient in nucleosome-bound DNA than it is in nucleosome-depleted regions of the genome. This method then segregates the non cross-linked DNA that is usually found in open chromatin, which is then sequenced. The protocol consists of cross linking, phenol extraction and sequencing the DNA in aqueous phase. --->

---

## TFBS binding does not equal function
- Applied ChIP-Seq for 119 DNA-binding proteins (87 sequence specific TFs)
- 636K (230Mb; 8.1% of genome) bound regions identified (and counted as functional!)
- Disregard evolutionary conservation
- Other study validates 12/14 Stat3 sites; extrapolating leaves 0.024% of the genome as TFBSs
- High inherent false positive rate (6-14nt sites, degenerate)
- Inflated values based on peak detection methods (600bp window; maybe should be 0.14% of genome)

---

## DNA methylation does not equal function
- Previous work suggests DNA methylation of promoters negatively regulates expression
- Identified 96% of 1.2 million sites are methylated (across 82 cell/tissues types)
- Again, just a chemical property, not a function - most CpG sites are able to be methylated
- A more interesting question: which regions lack CpGs?

<!--- information a bit scarce on overlap across cell/tissue types; 1.2mill is avg across 82 types --->
<!--- CpG sites are selected against - oft mutated, and they neg regulate gene exp --->
<!--- Are CpGs important? Yes! (genomic imprinting, aberrant in cancer, etc) --->

---

## Derived allele frequency distribution

<img src="./assets/img/fig1e.png" alt="Figure 1" width="75%">

<!---
Short term evolution as derived allele frequency (DAF), reflecting the amount of drift from the base present in the common ancestor of human and chimpanzee towards a new base in the human lineage. 
--->

---

## Derived allele frequency and negative selection
> - Evidence for negative selection using 205K ENCODE and 85K non-ENCODE SNPs
> - Multiple "technical" errors
  - Modeling genomes as independently derived (probably computational)
  - Choice of regions to identify, manner of sample selection is questionable
> - ENCODE samples had 0.2% lower DAF than control regions (p=4e-37)
  - Distributions overlap by 99.958%
  - Large sample size -> statistically significant result
  - But is the magnitude of the effect biologically meaningful?

<!---
Only selected primate specific regions to test - removing many functionally interesting regions
Only used 1 out of 3 ethnic samples of SNPs; this significantly changes the distribution, since polymorphic sites were defined using all 3
more than 80% of the regions uses were smaller than 100bp; median size of 15bp!
differences between the control and test regions; 
--->

---

## Junk (or garbage?) DNA
> - Number of putative functional genes decreasing (pre-human genome: 212K; now: 20K)
  - nematode: 20K genes!
  - 'streamlined' genomes only possible with large population size, deleterious effects of genome size are significant
> - The semantics of "junk" DNA - junk vs. garbage
  - Potential for function does not equal a function
> - Indifferent DNA - functional, not under constraint w.r.t. sequence composition (spacer sequence)
> - Are species with larger genomes, less phenotypically complex devoid of junk?

---

## Big science, small science
> - 442 researchers; $288,000,000 in funding
> - Concerns over loss of funding of small (focused) scientific projects over large scale fishing expeditions
> - Big Science - generate data; small science - make sense of it
> - ENCODE whittles it down to 2.7 billion nucleotides of importance, assuming a small science role of interpretation
> - High-impact false positives by the truckload
> - Let's rewrite the textbooks - the marketing, mass media hype, and PR textbooks!

---

## Thought experiment

1. Synthesize a random human genome. Do ENCODE again.
2. Repeat.

What would we find?

---

## Not all bad
- Extensive resource/dataset
- All data AND CODE are available; entire paper should be reproducible
- Pushed computational methods forward
  - Does not excuse many data selection oversights (garbage in, garbage out)
- Useful resource for genomics researchers
- Will impact disease research (Chron's)

---

## Increased vocabulary
- linguistic prudery - ?
- apophenia - see patterns in random data
- A methodological "legerdemain" - sleight of hand, hocus-pocus
- "genomic clochards" - vagrant, tramp
- "textual hermeneutics" - method or principle of interpretation


---

## Selection on ENCODE elements

<img src="./assets/img/fig1.png" alt="Figure 1" width="75%">

<!---
The second is long term evolution (GERP) or the extent of divergence of that base across the mammals considered.
--->
