# 2025-08-Oropouche-virus-strains-brain
Code associated with the analysis in the article: Microcephaly-like phenotype triggered by novel reassortant and prototypic Oropouche Virus strains in brain organoids

**RNA-seq data analysis.**  
Raw FASTQ files quality were checked with FastQC and aligned against the human transcriptome (GENCODE v48)<sup>1</sup> using Salmon<sup>2</sup> with default parameters and Gibbs sampling bootstrap method. Transcript level quant files were imported into R and summarized to gene. Differential expression was performed with DeSeq2<sup>3</sup> and functional enrichment using R package fgsea<sup>4</sup> against the Gene Ontology Biological process database (GOBP). Data wrangling and plotting was performed with Tidyomics<sup>5</sup>.

1 Mudge JM, Carbonell-Sala S, Diekhans M, et al. GENCODE 2025: reference gene annotation for human and mouse. Nucleic Acids Res 2025; 53(D1): D966–D975.  
2 Patro R, Duggal G, Love MI, et al. Salmon provides fast and bias-aware quantification of transcript expression. Nat Methods 2017; 14(4): 417–9.  
3 Love MI, Huber W, Anders S, et al. Moderated estimation of fold change and dispersion for RNA-seq data with DESeq2. Genome Biol 2014; 15: 550.  
4 Korotkevich G, Sukhov V, Budin N, et al. Fast gene set enrichment analysis. bioRxiv 2021; doi: 10.1101/060012.  
5 Hutchison WJ, Keyes TJ, The tidyomics Consortium, et al. The tidyomics ecosystem: enhancing omic data analyses. Nat Methods 2024; 21: 1166–70.  
