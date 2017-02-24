# intention-clarification
A dataset of clarification requests extracted from the AMI Corpus, annotated for whether they target intentionality.

The data is extracted from the AMI corpus [1] using the heuristic detailed in [2]. It is annotated by two expert annotators.

The data contains 338 dialogues, separated by double linebreaks.

Each dialogue contains:
- 10 utterances of prior context
- the SOURCE of the clarification request (the utterance that is clarified), marked by "->"
- the clarification request (CR) itself, marked by "-->"
- the ANSWER to the CR, marked by "->"
- the FOLLOW UP of the asker of the CR, marked by "->"; if there is no follow up, the 10 utterances after the answer are displayed.

If the prior or posterior context is less than 10 utterances long, the maximum number is displayed.

The last line of each excerpt is the annotation. There are 5 annotations:
- "not" indicates that the CR is not actually a clarification request (i.e. a false positive of the heuristic).
- "low" indicaes that the CR is a low-level clarification request (channel, parsing, or resolution).
- "int-rec" indicates that the CR is an intention-recognition CR.
- "int-tr" indicates that the CR is an intention-adoption CR.
- "ambig" indicates that the CR is ambiguous between one or more of the above categories.

The data points towards a significant, but understudied, class of clarification questions. Some discussion can be found in [3].

[1] Carletta, J. (2007). Unleashing the killer corpus: experiences in creating the multi-everything AMI meeting corpus. Language Resources and Evaluation 41(2), 181–190.

[2] Julian J. Schlöder and Raquel Fernández (2015). Clarifying Intentions in Dialogue: A Corpus Study, Proceedings of the 11th International Conference on Computational Semantics (IWCS 2015).

[3] Julian J. Schlöder and Raquel Fernández (2014). Clarification Requests on the Level of Uptake, Proceedings of the 18th Workshop on the Semantics and Pragmatics of Dialogue (SemDial 2014, "DialWatt").
