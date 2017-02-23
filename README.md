# intention-clarification
A dataset of clarification requesets extracted from the AMI Corpus, annotated for whether they target intentionality.

The data is extracted from the AMI corpus [1] using the heuristic detailed in [2]. It is annotated by two expert annotators.

The data contains 338 dialogues, separated by double linebreaks.

Each dialogue contains:
- 10 utterances of prior context.
- the SOURCE of the clarification request (the utterance that is clarified), marked by "->"
- the clarification request (CR) itself, marked by "-->"
- the ANSWER to the CR, marked by "->"
- the FOLLOW UP of the asker of the CR, marked by "->"

The last line of each excerpt is the annotation. There are 5 annotations:
- "not" indicates that the CR is not actually a clarification request (i.e. a false positive of the heuristic).
- "low" indicaes that the CR is a low-level clarification request (channel, parsing, or resolution).
- "int-rec" indicates that the CR is an intention-recognition CR.
- "int-tr" indicates that the CR is an intention-adoption CR.
- "ambig" indicates that the CR is ambiguous between one or more of the above categories.

For example, this is the first dialogue in the dataset:

A: Yeah but y but you have to go through all the channels if you want to go
B: I think you can if you have a scale , so
C: No no , you don't have to y no
C: it's uh when you when you stop t uh
C: when you stop , the the turn ,
A: Mm-hmm .
C: then the angle you stop is the angle you is the channel you
D: Yeah .
D: How d how do you know this angle is th is the correct one ?
-> C: It's it's very easy , because you kn you know how many channel are there in the
--> D: So you you count one degree , two degrees , no .
-> C: Yeah , yeah , yeah . You can do it .
-> D: I don't think so .
int-tr,

"C: It's it's very easy , because you kn you know how many channel are there in the" is the SOURCE.
"D: So you you count one degree , two degrees , no ." is the CR.
"C: Yeah , yeah , yeah . You can do it ." is the  ANSWER.
"D: I don't think so ." is the FOLLOW UP.

The last line indicates that the CR is judged to be an intention-transfer clarification request.


[1] Carletta, J. (2007). Unleashing the killer corpus: experiences in creating the multi-everything AMI meeting corpus. Language Resources and Evaluation 41(2), 181–190.

[2] Julian J. Schlöder and Raquel Fernández (2015). Clarifying Intentions in Dialogue: A Corpus Study, Proceedings of the 11th International Conference on Computational Semantics (IWCS 2015).
