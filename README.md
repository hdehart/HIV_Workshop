# Whodunit? Forensics with DNA & Bioinformatics Workshop

The workshop will analyze DNA sequence data to identify the gene(s) involved and identify the context of the samples by linking to PubMed records. You will analyze DNA sequence data using local alignment, global alignment, multiple sequence alignment tools and then use your multiple sequence alignment to estimation evolutionary (phylogenetic) relationships amongst the sequences.  With the phylogeny in hand, you will then solve the forensic mystery and decide if the accused is innocent or guilty of an alleged crime. You will gain experience using a diversity of open-access tools that are all available online. 
## Goals:
1. Perform BLAST search to identify sequence region (local alignment)
2. Link to study system via PubMed link on GenBank entry
3. Conduct a multiple sequence alignment (global alignment)
4. Estimate a phylogeny
5. Interpret your phylogenetic estimate relative to the forensics case

### Part 0 - Looking at Sequence Data
1.	Take a look at the [sequence data](https://github.com/hdehart/HIV_Workshop/blob/master/data_subset.fas). This dataset contains multiple sequences in [FASTA](https://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=BlastHelp) format. This is a standard format for DNA sequence data developed by [David Lipman](http://www.people.virginia.edu/~wrp/) and [William Pearson](https://www.amia.org/about-amia/leadership/acmi-fellow/david-j-lipman-md-facmi). Copy the first nucleotide sequence. Each sequence starts with a title to separate it from others in the same file:

\>**AY156858.1**\_*V01*

\>**Accession number**\_*Sample name*

An [accession number](https://www.ncbi.nlm.nih.gov/genbank/sequenceids/) is a unique ID assigned to sequences uploaded to the [GenBank database](https://www.ncbi.nlm.nih.gov/genbank/). The sample names include information about who the sample came from:

1. Go to [BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi) What option(s) might you choose given your data?  Why?
2. Run a BLAST - What are the options? What do these mean?  What are your parameter values?  How do those impact your search?
3. Explore the results of the BLAST search. Click on the accession number of the top hit. What do you think this sequence is? Who did it come from? 

### Part 1 - Creating a Multiple Sequence Alignment (MSA)
You have multiple samples from the victim, other patients under the doctor’s care, and other HIV positive individuals. How can you use these sequences to trace the source of the victim’s infection? You need to compare the similarities and differences between the sequences, but how do we do that? 


![alt text](https://github.com/hdehart/HIV_Workshop/blob/master/grapefruit.png) ![alt text](https://github.com/hdehart/HIV_Workshop/blob/master/orange.png)

*[source](https://commons.wikimedia.org/wiki/User:Evan-Amos/Food)*

Look at these 2D pictures of a grapefruit and an orange. Are there differences you can see? Are there differences you can’t see in this format? Would looking at the real fruits in person better inform your ideas about similarities and differences?

This is why we create multiple sequence alignments! Lining up the sequences helps us determine the similarities and differences among sequences. We do this quickly by using alignment software.

1.	Go to the [MAFFT alignment online software](https://mafft.cbrc.jp/alignment/server/) and explore some ways to create a multiple sequence alignment. If you change default settings, compare with others and see if and what parameters make a big difference in the alignments you create.
2.	Look at the different ways the sequences were aligned. At the bottom of each alignment, there are symbols to indicate shared and different amino acid bases.

|Symbol|Meaning|
:-------:|-------|
|\* | All the sequences are the same
|\. | There are differences between some or all of the sequences

3.	Can you spot some differences between the different sample sequences? Are there shared similarities between patient (P) samples and victim (V) samples? What about LA samples?

### Part 2 - Creating Phylogenetic Relationships and Trees

Now that the sequences are [aligned](https://github.com/hdehart/HIV_Workshop/blob/master/data_aligned.fas) and we can see all the similarities and differences, we need to determine which ones are more and less alike. How can we do that? Let's think back to the fruits...



Think about some charactersitics that are shared among different types of fruits. All fruits are more siilar to each other than they are to a avegetable like an onion. Within fruits however, some are more closely related because of shared characteristics. For example, the orange and grapefruit are more similar to each other than either is to an apple, because they are citrus fruits. Peaches and cherries are more similar to each other than either is to the apple, because they only have a single pit. 

Let’s do the same with the HIV sequences. 

1.	Create a hypothesis. If some sequences are more similar to each other, what do you think that means?
2.	Go back to the alignment you created and create a phylogenetic tree out of the alignment you created. What do you think each of the parameters adjusts? Do you think adjusting these parameters will greatly affect your results?
6.	Look at the tree you made. Do you see any groupings of sequences? Which sequence groups do you think are more or less closely related? Why? What do you think the numbers on the branches represent?

#### Final Conclusions

1.	Was your hypothesis supported? Why or why not? Do you believe the doctor was guilty? Why or why not?
2.	Go back to your original BLAST results. Click on accession number **AY156858.1**. Find the PUBMED reference number **12388776** and click on it to read the scientific abstract of the paper that was published. This abstract will tell you whether or not the doctor was found guilty.

More information on this case:

[ABC News](https://abcnews.go.com/Technology/story?id=97856&page=1)

[The Advocate](https://www.theadvocate.com/acadiana/news/article_4f2c8962-fd3c-5fa7-87cf-048188f626e3.html)
