# HMMs-Based-POS-Tagging-using-Modified-Viterbi-algorithm
In this project, we need to modify the Viterbi algorithm to solve the problem of UNKNOWN WORDS using at least two techniques. Though there could be multiple ways to solve this problem, we may use the following hints: 



1. Which tag class do we think most unknown words belong to? Can we identify rules (e.g. based on morphological cues) that can be used to tag unknown words? You may define separate python functions to exploit these rules so that they work in tandem with the original Viterbi algorithm.  


2. Why does the Viterbi algorithm choose a random tag on encountering an unknown word? We have to modify the Viterbi algorithm so that it considers only one of the transition or emission probabilities for unknown words. 


In original Viterbi algorithm there is a loss of accuracy was majorly due to the fact that when the algorithm encountered an unknown word (i.e. not present in the training set, such as 'Twitter'), it assigned an incorrect tag arbitrarily. This is because, for unknown words, the emission probabilities for all candidate tags are 0, so the algorithm arbitrarily chooses (the first) tag.  


For this Project , we’ll use the Treebank dataset of NLTK with the 'universal' tagset. The Universal tagset of NLTK comprises only 12 coarse tag classes as follows: Verb, Noun, Pronouns, Adjectives, Adverbs, Adpositions, Conjunctions, Determiners, Cardinal Numbers, Particles, Other/ Foreign words, Punctuations. 

Note that using only 12 coarse classes (compared to the 46 fine classes such as NNP, VBD etc.) will make the Viterbi algorithm FASTER as well.
