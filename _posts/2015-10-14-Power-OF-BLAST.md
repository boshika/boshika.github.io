---
layout: post
title: Power of BLAST
category: article
tags:
 - coding
 - challenges
 - archives
 - datastructures
---

<!-- <!DOCTYPE html> -->
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Power of BLAST</title>
</head>
<body>
	<h4>POWER OF BLAST</h4>
	<p>
	Couple years back at Stanford, doing bench research for me involved running datasets, on heavy Bioinformatics tools, 
	BLAST(Basic Local Alignment Search Tool), was what I used almost on daily basis, from DNA sequence alignment, 
	to protein sequence analysis. In genomic research, these tools become second nature, I used them without 
	really understanding the underlying principles of such computational tools, and this sought a bugged me.
  So when I entered graduate school, the first class I took was an Introductory course in Bioinformatics, and 
  Algorithms, and here is where I learnt the power of the BLAST algorithm.	
</p>
<h4>BLAST is a heuristic algorithm</h4>
<p>
  The BLAST algorithm finds regions of local alignments by breaking the query sequence down into smaller chunks of sequence called words, for amino acids it is 3 letter, while for nucleotides it is 11. These words are then indexed by the computer along with information about where each is found in the intact sequence. The BLAST algorithm then starts by seeding the search with this small subset of letters from the query sequence. 
   For each search that happens against the database a threshold(t) is set, the t determines the accuracy, and the speed at which homologous sequences can be found, higher t is faster, but less reliable.
In query sequence below a k=3 search is conducted(this a protein sequence). The scores are created by comparing the word in the list in step 2 with all the 3-letter words. By using the scoring matrix (substitution matrix) to score the comparison of each residue pair, there are 20^3 possible match scores for a 3-letter word. For example, the score obtained by comparing PQG with PEG and PQA is 15 and 12, respectively.      

</p>
<img src = "https://upload.wikimedia.org/wikipedia/commons/5/56/Query_word.jpg">
<p> 
  The words whose scores are greater than the threshold T will remain in the possible matching words list, while those with lower scores will be discarded. For example, PEG is kept, but PQA is abandoned when T is 13.
Once the initial word hit has been found, the BLAST algorithm attempts to extend the match in the immediate sequence neighborhood. Extension proceeds and the cumulative score is calculated using the scoring matrices discussed above.
Here we I need to mention high-scoring segment pair or HSP.  As long as positive matches and conservative substitutions outweigh the negative scores for gaps and mismatches, the cumulative score will increase. When the cumulative score starts to drops off, the BLAST algorithm measures the rate of decay and, once past a certain point, stops trying to extend the alignment. The result is an extended sequence alignment that was initially seeded by a word hit. So this was the old BLAST, a newer, faster BLAST called BLAST2 has been created. 
BLAST2, uses a lower threshold for sequence identity, this increases the number of 3 letter words in the list. A arbitrary distance can be set in BLAST, this will be used to join all three letter sequences within that distance range. See below

</p>
<img src = "https://upload.wikimedia.org/wikipedia/en/8/84/Neighbor_HSP.jpg">
<p>
Next step would be to take all these HSPs and determine whether this match is significant or not. Two BLAST statistics, the score (S) and the E-value (E) are particularly helpful in making this interpretation. First, the score (S) is a good measure of the quality of an alignment because it is calculated as the sum of substitution and gap scores for each aligned residue. Second, the E-value (E), or expectation value is a good measure of the significance of the alignment. The E-value is the number of different alignments, with scores equivalent to or better than S, that are expected to occur in a database search by chance. The lower the E-value, the more significant the alignment result.
Understanding BLAST statistics helps to effectively interpret BLAST results, but this is a biological interpretation and whenever possible you should apply your knowledge of biology. Many time secondary alignments, need to be conducted to further to zero in specific areas of interest.
I want to touch on the different categories of the BLAST search, and right way to conduct sequence alignments…at this point the post is longer then I intended it to be...so coming soon

</p>


 
</body>
</html>
