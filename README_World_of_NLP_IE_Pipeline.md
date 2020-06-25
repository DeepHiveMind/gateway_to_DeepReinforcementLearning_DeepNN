# World of NLP IE Pipeline
Please refer to my another repo [NLP Information Extraction Optimized Pipeline - NLP IE Pipeline](https://github.com/DeepHiveMind/nlp-architect/blob/master/README.md) which refers to Intel Nervana (Intel's open source AI/ML Platform) NLP-Architect solution component for state-of-the-art deep learning topologies and techniques for optimizing Natural Language Processing. This repo is very enriching as to the vast landscape of NLP Architectural constructs with extensive detailing.

The repo has reference and implementations of  NLP models that provide best (or near) SOTA class performance:

* [Word chunking](http://nlp_architect.nervanasys.com/tagging/sequence_tagging.html#word-chunker)
* [Named Entity Recognition](http://nlp_architect.nervanasys.com/tagging/sequence_tagging.html#named-entity-recognition)
* [Dependency parsing](http://nlp_architect.nervanasys.com/bist_parser.html)
* [Intent Extraction](http://nlp_architect.nervanasys.com/intent.html)
* [Sentiment classification](http://nlp_architect.nervanasys.com/sentiment.html#supervised-sentiment)
* [Language models](http://nlp_architect.nervanasys.com/lm.html#language-modeling-with-tcn)
* [Transformers](http://nlp_architect.nervanasys.com/transformers.html) (for NLP tasks)

Natural Language Understanding (NLU) models that address semantic understanding:

* [Aspect Based Sentiment Analysis (ABSA)](http://nlp_architect.nervanasys.com/absa.html)
* [Joint intent detection and slot tagging](http://nlp_architect.nervanasys.com/intent.html)
* [Noun phrase embedding representation (NP2Vec)](http://nlp_architect.nervanasys.com/np2vec.html)
* [Most common word sense detection](http://nlp_architect.nervanasys.com/word_sense.html)
* [Relation identification](http://nlp_architect.nervanasys.com/identifying_semantic_relation.html)
* [Cross document coreference](http://nlp_architect.nervanasys.com/cross_doc_coref.html)
* [Noun phrase semantic segmentation](http://nlp_architect.nervanasys.com/np_segmentation.html)

Optimizing NLP/NLU models and misc. optimization techniques:

* [Quantized BERT (8bit)](http://nlp_architect.nervanasys.com/quantized_bert.html)
* [Knowledge Distillation using Transformers](http://nlp_architect.nervanasys.com/transformers_distillation.html)
* [Sparse and Quantized Neural Machine Translation (GNMT)](http://nlp_architect.nervanasys.com/sparse_gnmt.html)

Solutions (End-to-end applications) using one or more models:

* [Term Set expansion](http://nlp_architect.nervanasys.com/term_set_expansion.html) - uses the included word chunker as a noun phrase extractor and NP2Vec to create semantic term sets
* [Topics and trend analysis](http://nlp_architect.nervanasys.com/trend_analysis.html) - analyzing trending phrases in temporal corpora
* [Aspect Based Sentiment Analysis (ABSA)](http://nlp_architect.nervanasys.com/absa_solution.html)


