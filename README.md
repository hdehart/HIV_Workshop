# HIV Transmission in a Criminal Case

You are a researcher in a forensics laboratory. You are contacted by a lawyer representing a victim who accuses her physician of intentionally infecting her with the Human Immunodeficiency Virus (HIV) after their romantic relationship ended. After receiving a vitamin B-12 injection from this doctor, the victim tested positive for HIV. The lawyer alleges that the shot contained infected blood from other HIV positive patients under the doctor’s care. Using HIV sequences from victim, patients of the doctor, and other people in the area, it is up to you to determine if the victim could have contracted HIV from her doctor’s shot or some other source.
## Goals:
1.	Perform a BLAST search to understand sequence data
2.	Conduct multiple sequence alignment (MSA)
3.	Build a phylogenetic tree
4.	Determine if defendant is guilty or not guilty 
### Part 1 - Looking at Sequence Data
1.	View the [sequence data](https://github.com/hdehart/HIV_Workshop/blob/master/HIV_subset.fas)

2.	Go to [BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi) and select the nucleotide BLAST option
3.	Copy the first nucleotide option (>AY156858.1_V01) and paste it underneath the Enter Query Sequence box
4.	Keep all default options and hit BLAST
5.	Explore the results of the BLAST search. Click on the accession number of the top hit. What do you think this sequence is? Who did it come from? 

### Part 2 - Creating a Multiple Sequence Alignment (MSA)
You have multiple samples from the victim, other patients under the doctor’s care, and other HIV positive individuals. How can you use these sequences to trace the source of the victim’s infection? You need to compare the similarities and differences between the sequences, but how do we do that? 
