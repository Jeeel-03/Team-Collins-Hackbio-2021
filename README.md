# Team-Collins-Hackbio-2021
#### In Stage 1 of HackBio Internship_2021, our task was to perform analysis on a genomic dataset using various bioinformatic tools of our choice. Malaria is a disease caused by parasitic protozoans in the genus Plasmodium, which are transmitted between vertebrate hosts by female mosquitoes in the genus Anopheles. The predominant malaria parasite species that infect humans are Plasmodium falciparum (Neafsey et al., 2021) and our team agreed to work on Plasmodium falciparum (P. falciparum). The objective of our analysis was to evaluate variations in the genome sequence with the reference by performing a variant call analysis.
![This is an image of the workflow.](https://github.com/Jeeel-03/Team-Collins-Hackbio-2021/blob/main/Workflow%20for%20ppt.png)
### Analysis
###### We started our analysis by performing a quality assessment on the dataset generating a FastQC report and then filtering out poor-quality reads to re-assess the quality to get a consolidated MultiQC report from all the samples. Following this, indexing of the reference genome that we retrieved from the PlamoDB database was done, which enables locating possible alignment sites for query sequences in a genome, rapidly saving time during alignment. Later, reads were mapped to the reference genome, and we got a SAM file. Further, this SAM file output was sorted by various  SAM attributes generating a BAM output file, which was then executed for the AddOrReplaceReadGroups command to align all the reads to a single new read-group. Next was to validate our BAM file to a specific format to ensure that no errors appear later due to improper formatting. Subsequently, any duplicate reads were identified and characterized as being derived from a single piece of DNA. Followed by base recalibration, variant calling was executed using Haplotype caller to obtain a raw VCF file, for our sample. Variant annotation was then performed on the vcf file to annotate the dataset and identify genetic variation from the ‘reference’ genome of P.falciparum. 
### Result and Discussion
###### The aim of our analysis was to observe any genetic variation in the datasets from the reference genome we acquired. After executing the workflow, we were able to generate our final variant annotation report. The coverage for our sample was found to be low. According to the snpEff results, a total of 49,978 variants were present, attributed mainly to Single Nucleotide Polymorphisms, insertion, and deletion mutations. However, we did not observe any known variants in our analysis.
### Conclusion
###### The completion of this analysis is attributed to the dedicated contribution of the majority of our team members. We demonstrated the known variability on the P. falciparum genome using various bioinformatic analyses on pre-existing data and did not find any known variants. We intend to gain more insights into the mutability of the protozoan by including more samples in future.
### Supplementary Material
###### The analytical reports, along with the video presentation can be found in the **[link]**(https://drive.google.com/drive/folders/17c4NujWtEIVH6f0TcPQXa6sY121Vtq6J) 
### Contributors
![This is an image of the Contributors.](https://github.com/Jeeel-03/Team-Collins-Hackbio-2021/blob/main/Contributions.png)
## Thank you!
