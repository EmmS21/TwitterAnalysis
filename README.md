# TwitterAnalysis
Analysing Twitter data to identify interesting trends for Hooros clients
/**********
Latent Dirichlet Allocation

We sought out to use the Latent Dirichlet Allocation model to classify Twitter bio text of thousands of users into easily interpretable topics. The idea was to use these topics to broadly classify the users identified using a few topics as a basis of said classification.

This was a project to help better understand one of our client's potential target market. In carrying out this analysis we made the assumptions that; Twitter users use the bio to outline their professional achievements, professions/what they do in life, their major interests, ideological leanings and what they would like to be identified with (e.g music lover, libertarian, black consciousness).

We chose the Latent Dirichlet Allocation (LDA) model primarily because we thought this was a very useful tool to decompress large texts and extract key underlying topics existing within the text corpus and used these topics to infer a few key attributes of our target audience

- How LDA Works - http://brooksandrew.github.io/simpleblog/articles/latent-dirichlet-allocation-under-the-hood/ 
- LDA explained in greater detail - https://www.youtube.com/watch?v=DWJYZq_fQ2A

One contentious issue in this analysis was choosing the 'appropriate' number of topics. There appears to be numerous views on the best method to find the ideal number of topics including the 'ldatuning' package and the heuristic appproach (which I confess to not understanding). To choose the 'right' number of topics, I ran numerous trials and settled on between 7 and 8 topics. This made the topics more readable and easier to interpret for the purposes outlined
***********/



/*************
#Bigram Analysis

In order to get an understanding of the types of conversation the users we identified are having, which would then presumably give us a better understanding of their interests, things they talk about and themes we can exploit to increase the efficiency of marketing campaigns targeting this audience, we opted to carry out a bigram analysis identifying the top 50 occuring bigrams (in terms of frequency) and using this to better understand the conversations people were having. This analysis was based on over 500 000 tweets observed over a period of a few days (I understand that this could mean the topics identified are simply topics trending at that particular moment and may not give us the ability to accurately infer themes of topics that these users normally have- e.g by evaluating tweets over a longer period, say a few months would, you may be able to get a clearer picture of the types of topics these users are interested in).

Bigrams can be loosely considered two adjacent words from a given text.  Bigrams give a more contextual understanding of the types of topics or conversations people are having. In this scenario we are using bigrams to understand the types of conversations the people we are targeting are having.

- More reading on ngram analysis https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3694275/ 
*******/
