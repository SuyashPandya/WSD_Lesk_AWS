# WSD_Lesk_AWS
Finding and Explaining ambiguity of English sentence using Simplified Lesk algorithm.

The Lesk algorithm is based on the assumption that words in a given "neighborhood" (section of text) will tend to share a common topic. A simplified version of the Lesk algorithm is to compare the dictionary definition of an ambiguous word with the terms contained in its neighborhood. Versions have been adapted to use WordNet.[2] An implementation might look like this:

1. for every sense of the word being disambiguated one should count the number of words that are in both the neighborhood of that word and in the dictionary definition of that sense
2. the sense that is to be chosen is the sense that has the largest number of this count.

In Simplified Lesk algorithm,[3] the correct meaning of each word in a given context is determined individually by locating the sense that overlaps the most between its dictionary definition and the given context. Rather than simultaneously determining the meanings of all words in a given context, this approach tackles each word individually, independent of the meaning of the other words occurring in the same context.

"A comparative evaluation performed by Vasilescu et al. (2004)[4] has shown that the simplified Lesk algorithm can significantly outperform the original definition of the algorithm, both in terms of precision and efficiency. By evaluating the disambiguation algorithms on the Senseval-2 English all words data, they measure a 58% precision using the simplified Lesk algorithm compared to the only 42% under the original algorithm.
