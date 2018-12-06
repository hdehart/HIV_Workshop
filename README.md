# HIV Transmission in a Criminal Case

You are a researcher in a forensics laboratory. You are contacted by a lawyer representing a victim who accuses her physician of intentionally infecting her with the Human Immunodeficiency Virus (HIV) after their romantic relationship ended. After receiving a vitamin B-12 injection from this doctor, the victim tested positive for HIV. The lawyer alleges that the shot contained infected blood from other HIV positive patients under the doctor’s care. Using HIV sequences from victim, patients of the doctor, and other people in the area, it is up to you to determine if the victim could have contracted HIV from her doctor’s shot or some other source.
## Goals:
1.	Perform a BLAST search to understand sequence data
2.	Conduct multiple sequence alignment (MSA)
3.	Build a phylogenetic tree
4.	Determine if defendant is guilty or not guilty 
### Part 1 - Looking at Sequence Data
1.	Take a look at the [sequence data](https://github.com/hdehart/HIV_Workshop/blob/master/HIV_subset.fas). Copy the first nucleotide sequence. Each sequence starts with a title to separate it from others in the same file:

\>**AY156858.1**\_*V01*

\>**Accession number**\_*Sample name*

An accession number is a unique ID assigned to sequences uploaded to the [GenBank database](https://www.ncbi.nlm.nih.gov/genbank/). The sample names include information about who the sample came from:

* **V** - Victim
* **P** - Other patient's under the doctor's care
* **LA** - Other HIV positive individuals from the Louisiana area

2.	Go to [BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi) and select the nucleotide BLAST option.
3.	Paste the first sequence underneath the Enter Query Sequence box.
4.	Keep all default options and hit **BLAST**.
5.	Explore the results of the BLAST search. Click on the accession number of the top hit. What do you think this sequence is? Who did it come from? 

### Part 2 - Creating a Multiple Sequence Alignment (MSA)
You have multiple samples from the victim, other patients under the doctor’s care, and other HIV positive individuals. How can you use these sequences to trace the source of the victim’s infection? You need to compare the similarities and differences between the sequences, but how do we do that? 


![alt text](https://github.com/hdehart/HIV_Workshop/blob/master/grapefruit.png) ![alt text](https://github.com/hdehart/HIV_Workshop/blob/master/orange.png)

1.	Look at these 2D pictures of a grapefruit and an orange. 
2.	Are there differences you can see? 
3.	Are there differences you can’t see in this format? 
4.	Would looking at the real fruits in person better inform your ideas about similarities and differences?

This is why we create multiple sequence alignments! Lining up the sequences helps us determine the similarities and differences among sequences. We do this quickly by using alignment software.

1.	Go to the [MAFFT alignment online software](https://mafft.cbrc.jp/alignment/server/). Copy and paste all the sequences into the input box.
2.	Keep all the default settings for now, scroll down and hit **SUBMIT**.
3.	Look at the different ways the sequences were aligned. At the bottom of each alignment, there are symbols to indicate shared and different amino acid bases.

|Symbol|Meaning|
:-------:|-------|
|\* | All the sequences are the same
|\. | There are differences between some or all of the sequences

4.	Can you spot some differences between the different sample sequences? Are there shared similarities between patient (P) samples and victim (V) samples? What about LA samples?

### Part 3 - Creating Phylogenetic Relationships and Trees

Now that the sequences are aligned and we can see all the similarities and differences, we need to determine which ones are more and less alike. How can we do that?

![alt text](https://github.com/hdehart/HIV_Workshop/blob/master/fam_tree.png)

*[source](https://www.ebi.ac.uk/training/online/course/introduction-phylogenetics/what-phylogeny/example-family-tree)*

1.	Think about a family tree. Draw some of your own family tree.
2.	What are some similarities between you, your brother, and your cousin? 
3.	Are you more or less related to your cousin than to your brother? Why is that?

Let’s do the same with the HIV sequences. 

1.	Create a hypothesis. If you believe the doctor infected the victim (V) with blood from one of his patients (P), do you think the sequences will be more or less similar than HIV sequences from other people (LA)?
2.	Go back to the alignment you created. 
3.	Click on **PHYLOGENETIC TREE**
4.	Go to the **BOOTSTRAP** setting. Check the **ON** box. This will create 100 different trees and tell you how many times it made the same choices. Hit **GO!**
5.	Click on **VIEW TREE ON PHYLO.IO**
6.	Look at the tree you made. Do you see any groupings of sequences? Which sequence groups do you think are more or less closely related? Why? What do you think the numbers on the branches represent?

#### Final Conclusions

1.	Was your hypothesis supported? Why or why not? Do you believe the doctor was guilty? Why or why not?
2.	Go back to your original BLAST results. Click on accession number **AY156858.1**. Find the PUBMED reference number **12388776** and click on it to read the scientific abstract of the paper that was published. This abstract will tell you whether or not the doctor was found guilty.

More information on this case:

[ABC News](https://abcnews.go.com/Technology/story?id=97856&page=1)

[The Advocate](https://www.theadvocate.com/acadiana/news/article_4f2c8962-fd3c-5fa7-87cf-048188f626e3.html)
