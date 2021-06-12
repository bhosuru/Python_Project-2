# Python_Project-2

INTRODUCTION:

Scientific Question: How many similar genes are present in the two primate isoform datasets provided by the Daugherty lab?

Background:

One of the projects in the daugherty lab is to map primate isoform clevage data to another data set with the same cleavage data across isoforms with population diversity. This way, the lab can acess what genes have population diversity easily without having to reference two data sets constantly. The data is sourced from two memebers of the lab: Brian Tsu (PhD student) and Bryant Cao (Masters student) who are my labmates in the Daugherty lab.

A little bit of background on viruses. Viruses have proteases that cleave human genes. When human genes are cleaved, some mutatae to avoid further deterioartion and some do not. The first data set has all the clevage site information and the second data set as all the mutataion (diversity) infomration. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7150265/ https://pubmed.ncbi.nlm.nih.gov/3444396/

Hypothesis: If there are clevage sites for a gene, then it must have population diversity.

Description: There are 95,265 genes with clevage site positions in the data set "counts_tog_AGM_ORFeome_mapping" which I will be referring to as data set 1. There 1199 genes with population diversity in the data set "filtered_pascaf_codon_level_data" which I will be referring to as data set 2. There are repititions of some gene in data set 1. First, I imported the data sets as a CSV file. My lab mates taught me how to do that! Next, I found the stop site of the cleavage site by using python to add 7 to the start sites because its an 8-mer using numpy. Next, I did some mini tasks like adding 8 new columns to data set 1 and moving the column order just for cleanliness. Next, I found out the number of similar genes in both datasets. Then I removed the duplicate genes and found the real number of common genes. Lastly, I exported the data to an excel sheet using excel writer. The hypothesis I made was wrong. If every gene with a clevage site had human diversity, then I would not have to do this project! Not all genes evolve after the presence of a clevage site. Which is why we see only 737 genes at the end that have human diversity data.
