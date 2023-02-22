# ROST_withParts

ROST (ROmanian Stories and other Texts) is a dataset introduced in the paper called "[A comparison of several AI techniques for authorship attribution on Romanian texts](https://www.researchgate.net/publication/365299177_A_comparison_of_several_AI_techniques_for_authorship_attribution_on_Romanian_texts)".

In this paper, several AI techniques were compared for classifying 400 literary texts written by 10 authors by taking into account a limited number of speech parts (prepositions, adverbs, and conjunctions). Next we wanted to use these texts to fine-tune trasnformer-based pretrained models. The initial texts varied in length from 91 to 39195 words. In order to have proper inputs for the BERT pretrained model, they needed to be split into fixed length sizes. Preliminary test run on lengths of 91, 200, and 400 words gave better results for 200 words. We also considered to limit the text fragments to have the minim lentgh of 100 words (tokens). Therefore, the only text that was 91 words was adjusted to the length of 114 words ("[Ziua Apocalipsei](http://www.povesti.org/#ziua_apocalipsei)" written by Mihai Oltean). 

