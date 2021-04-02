## readme.txt

1. System requirements

The "cubicIBD_demo.r" is a user-friendly R code which can be adapted to any R version without any packages dependencies, because we calculate the IBD probabilities based on two customed functions that can be easily loaded into the current R environment.

2. Intallation guide

Our code don't need to install any dependency R packages, two R scripts containing customed functions can be easily and fastly loaded into R environment.

3 and 4. Demo and Intructions for use

We provide three R scripts: cubicIBD_demo.r, pmatrix.r and omatrix.r.
All things need to do is run the "cubicIBD_demo.r", in which, the program will source the functions from "pmatrix.r" and "omatrix.r", and import a sample data "demo_geno_chr10.hmp.txt". This data contains 16636-SNPs genotypes of 24 parents and 1 offspring as a hapmap format. The function from pmatrix.r can generate initial probabilities for 24 parents at all 16636 SNP loci. Then, a "demo_map.txt" file will be imported that provide a SNP-pairwise linkage information referred from any published genetic maps, this information will help to build the function of the transmission probability. Finally, the function from omatrix.r will calculate the posterior probabilities of 24 parents at any SNP loci. Thus, the output will be a probability matrix with 16636 rows and 24 columns, in which, each row indicates a SNP and the sum value for each row is 1, as shown in "posterior_probs_chr10.txt" file.











