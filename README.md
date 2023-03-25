# phage-protein-families
Sequence alignments, Hidden Markov Models, and documentation of protein families used in bacteriophage bioinformatics projects of Stephen C. Hardies   

This site is designed to be accessed through https://Stephen-Hardies.github.io

The purpose of this site is to provide public access to protein family alignments, HMM models, and other supplementary information in support of papers published by Stephen C. Hardies. Since I expand my families past the limits of the most commonly used alignment software, other investigators will have trouble confirming or extending my studies without these resources. Some of these models may eventually appear in Pfam. I mention Pfam specifically, because that is the most accessible route for an investigator to incorporate an alignment into a public database. However, others of my alignments do not fit the Pfam specifications concerning specificity and overlap. For example, a key alignment for my purposes is that of all large terminases in tailed phages. In order to broaden the alignment to include all the different phage families, it will also give significant matching to other P-loop ATPases, and other ruvC paralogs. In order to use the HMM as an alignment tool to make timetrees across the breadth of the tailed phage viriome, I need them all in a common alignment. Pfam prefers to maintain multiple large terminase subfamilies. For other phage proteins, I typically try to expand their trees as deeply as the available techniques will allow. Hence, although most phage proteins are not amenable to a fully global alignment, this problem of an expanded alignment versus the typical protein family alignment arises repeatedly in my work. Further I typically expand each family ahead of each use, rather than using a static alignment.

I generally use the UCSC Sequence Alignment and Modeling System (SAM) for creating and expanding family alignments and the associated HMM. This system is not in widespread use. It is still available from https://users.soe.ucsc.edu/~karplus/projects-compbio-html/sam2src/, although it has not been maintained recently and may be difficult to install. I use SAM because in my control experiments in aligning diverged paralogs wherein there are crystal structures as an arbitrer of what is "correct" alignment, it out performs the more common options. At the greatest depths of comparison, I make the subfamily alignents using SAM, and then fuse them by HMM to HMM comparison using the HHsuite3 system. To allow others to remake my alignments and incorporate other sequences into them, I provide the resulting HMM converted to Hmmer3 format. The Hmmer3 HMM can be used to direct alignment with either the hmmer packag hmmalign program or with clustal omega. I also provide the HHpred-formatted HMMs. For most all purposes I use a local installation of HHsuite3 to do HMM to HMM comparons rather than other options because of its greater sensitivity. 
