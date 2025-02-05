# ENCODE reproducibility, cutandrun & TIP-seq benchmark
Xindong; 

## TIP-seq benchmark
### Updating progress
see updating [slides](https://docs.google.com/presentation/d/1RUutxp24KqfAtOKvWkCQTmH0ZVNXelx9vwVgdoKXpAU/edit?usp=sharing) of the progress
### ENCODE reproducibility 
see [notes](https://docs.google.com/document/d/11hHNdTwsNA4ggAtvPus_hpmdrkUIPJjVDAXd-HnrSdg/edit?usp=sharing) for information from literature 
### R scripts, results metrics and plots
see EpiCompare peak comparison and plotting R scripts at [R_Code](https://github.com/neurogenomics/Benchmark_with_EpiCompare/tree/master/R_Code);
see Plots at [TIP-seq plots](https://github.com/neurogenomics/Benchmark_with_EpiCompare/tree/master/Report_Figure), and [additional plots](https://github.com/neurogenomics/Benchmark_with_EpiCompare/tree/master/plot_TIPseq).


## cutandrun report (data analysis website): 
See [final web report](https://neurogenomics.github.io/Benchmark_with_EpiCompare/DA_Web/Data_Analysis/Data_Analysis_Xindong.html), or at [MSc course server](http://msc.bc.ic.ac.uk/~xs221/DA_Web/Data_Analysis/Data_Analysis_Xindong.html)(with Imperial login)

## Data availability
### ENCODE correlation bewteen experiments and replicates: 
Annotation: H3K4me3_EN4G38_E1_IRpseudo123 <br>
PTM name;<br>
EN 3/4 for ENCODE 3 or 4; G for genome build<br>
E for experiment number <br>
IR for isogenic replicates (pseudo if pseudoreplicates, if I only then it's just the peaks)<br>
For [ENCODE Replication definition](https://www.encodeproject.org/data-standards/terms/)

### Histone modification chromatin annotation:
A brief histone PTM landscape:
![image](https://github.com/neurogenomics/CUTandRUN_EpiCompare/raw/master/Images/PTM_landscape_MIT.PNG) [MIT course ref](https://www.youtube.com/watch?v=ywJep35QnjY&list=PLypiXJdtIca6dEYlNoZJwBaz__CdsaoKJ&index=8)

H3K4me1, preferentially associated with enhancers [1](https://pubmed.ncbi.nlm.nih.gov/17571346/),[6](https://pubmed.ncbi.nlm.nih.gov/17277777/); <br>
H3K4me2, associated with promoters and enhancers [1](https://pubmed.ncbi.nlm.nih.gov/17571346/),[3](https://pubmed.ncbi.nlm.nih.gov/17512414/),[6](https://pubmed.ncbi.nlm.nih.gov/17277777/),[9](https://pubmed.ncbi.nlm.nih.gov/15680324/); <br>
H3K4me3, a modification associated with promoters [4](https://pubmed.ncbi.nlm.nih.gov/17603471/),[5](https://pubmed.ncbi.nlm.nih.gov/17632057/),[9](https://pubmed.ncbi.nlm.nih.gov/15680324/); <br>
H3K9ac and H3K27ac, associated with active regulatory regions [9](https://pubmed.ncbi.nlm.nih.gov/15680324/),[10](https://pubmed.ncbi.nlm.nih.gov/19295514/); <br>
H3K27me3, associated with Polycomb-repressed regions [3](https://pubmed.ncbi.nlm.nih.gov/17512414/),[4](https://pubmed.ncbi.nlm.nih.gov/17603471/); <br>
H3K36me3 and H4K20me1, associated with transcribed regions [3](https://pubmed.ncbi.nlm.nih.gov/17512414/),[4](https://pubmed.ncbi.nlm.nih.gov/17603471/),[5](https://pubmed.ncbi.nlm.nih.gov/17632057/); <br> 
These are [overall conclusion](https://doi.org/10.1038/nature09906) with 9 cell lines including the K562. These consist of embryonic stem cells (H1 ES), erythrocytic leukemia cells (K562), B-lymphoblastoid cells (GM12878), hepatocellular carcinoma cells (HepG2), umbilical vein endothelial cells (HUVEC), skeletal muscle myoblasts (HSMM), normal lung fibroblasts (NHLF), normal epidermal keratinocytes (NHEK), and mammary epithelial cells (HMEC).

#### A549:
[H3K4me3](https://neurogenomics.github.io/CUTandRUN_EpiCompare/ENCODE_correlation/A549_H3K4me3_ExperimentSeries/EpiCompare.html)
[H3K9me3](https://neurogenomics.github.io/CUTandRUN_EpiCompare/ENCODE_correlation/A549_H3K9me3_Experimentseries/EpiCompare.html)

#### K-562:
[H3K4me1](https://neurogenomics.github.io/CUTandRUN_EpiCompare/ENCODE_correlation/K562_H3K4me1/EpiCompare.html)
[H3K4me2](https://neurogenomics.github.io/CUTandRUN_EpiCompare/ENCODE_correlation/K562_H3K4me2/EpiCompare.html)
[H3K4me3](https://neurogenomics.github.io/CUTandRUN_EpiCompare/ENCODE_correlation/K562_H3K4me3/EpiCompare.html)
[H3K9ac](https://neurogenomics.github.io/CUTandRUN_EpiCompare/ENCODE_correlation/K562_H3K9ac/EpiCompare.html)
[H3K9me1](https://neurogenomics.github.io/CUTandRUN_EpiCompare/ENCODE_correlation/K562_H3K9me1/EpiCompare.html)
[H3K27ac](https://neurogenomics.github.io/CUTandRUN_EpiCompare/ENCODE_correlation/K562_H3K27ac/EpiCompare.html)
[H3K27me3](https://neurogenomics.github.io/CUTandRUN_EpiCompare/ENCODE_correlation/K562_H3K27me3/EpiCompare.html)
[H3K36me3](https://neurogenomics.github.io/CUTandRUN_EpiCompare/ENCODE_correlation/K562_H3K36me3/EpiCompare.html)
[H3K79me2](https://neurogenomics.github.io/CUTandRUN_EpiCompare/ENCODE_correlation/K562_H3K79me2/EpiCompare.html)
[H4K20me1](https://neurogenomics.github.io/CUTandRUN_EpiCompare/ENCODE_correlation/K562_H4K20me1/EpiCompare.html)

### CUT&RUN Data information:
Sample collectiona and preparation by Yi Yang; 
CUT&RUN peaks storage: /rds/general/project/neurogenomics-lab/live/Data/cutandrun/cutandrun_EpiCompare/1st_trial/called_peaks<br>
File annotation: <br>
TOP001: peaks with 1% confidence; control: peaks exclude IgG peaks

### The cutandrun EpiCompare report:<br>
K-562 cell line; genome build hg38; stringent SEACR peak calling <br>
TOP001: peaks with 1% confidence; Control: peaks exclude negative control<br>
[H3K4me1](https://neurogenomics.github.io/CUTandRUN_EpiCompare/cutandrun_EpiCompare_hg38/H3K4me1/EpiCompare.html)
[H3K4me2](https://neurogenomics.github.io/CUTandRUN_EpiCompare/cutandrun_EpiCompare_hg38/H3K4me2/EpiCompare.html)
[H3K4me3](https://neurogenomics.github.io/CUTandRUN_EpiCompare/cutandrun_EpiCompare_hg38/H3K4me3/EpiCompare.html)
[H3K9ac](https://neurogenomics.github.io/CUTandRUN_EpiCompare/cutandrun_EpiCompare_hg38/H3K9ac/EpiCompare.html)
[H3K9me1](https://neurogenomics.github.io/CUTandRUN_EpiCompare/cutandrun_EpiCompare_hg38/H3K9me1/EpiCompare.html)
[H3K27ac](https://neurogenomics.github.io/CUTandRUN_EpiCompare/cutandrun_EpiCompare_hg38/H3K27ac/EpiCompare.html)
[H3K27me3](https://neurogenomics.github.io/CUTandRUN_EpiCompare/cutandrun_EpiCompare_hg38/H3K27me3/EpiCompare.html)
[H3K36me3](https://neurogenomics.github.io/CUTandRUN_EpiCompare/cutandrun_EpiCompare_hg38/H3K36me3/EpiCompare.html)
[H3K79me2](https://neurogenomics.github.io/CUTandRUN_EpiCompare/cutandrun_EpiCompare_hg38/H3K79me2/EpiCompare.html)
[H4K20me1](https://neurogenomics.github.io/CUTandRUN_EpiCompare/cutandrun_EpiCompare_hg38/H4K20me1/EpiCompare.html)









