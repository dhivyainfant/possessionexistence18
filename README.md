# possessionexistence18

Mining Possessions: Existence, Type and Temporal Anchors

Official release, June 6, 2018.

Paper:
-------------------------------------------------------------------------------
Dhivya Chinnappa and Eduardo Blanco. 2016.
Mining Possessions: Existence, Type and Temporal Anchors.
In Proceedings of the 16th Annual Conference of the North American Chapter of the Association for Computational Linguistics (NAACL). New Orleans, LA, USA. 
-------------------------------------------------------------------------------

Dhivya Chinnappa - University of North Texas, Denton, TX
Eduardo Blanco - University of North Texas, Denton, TX

Contact: dhivyainfantchinnappa@my.unt.edu, eduardo.blanco@unt.edu
===============================================================================

The file NAACL2018_annotations.csv provides annotations for 979 instances generated from OntoNotes.

-------------
CORPORA
-------------

Annotations are done on top of OntoNotes 5.0, https://catalog.ldc.upenn.edu/LDC2013T19

Possessor-Possessee pairs are generated deterministically through restrictions detailed in Section 4.1 of the paper.

The annotation layers for generating features can be obtained from CoNLL 2011 shared task release

CoNLL 2011: http://conll.cemantix.org/2011/

In order to use the annotations for learning, both OntoNotes 5.0 from the LDC and the CoNLL-2011 shared task release are required.

CoNLL 2011 Shared Task website provides more instructions on how to generate CoNLL files (both gold and auto).

-------------
ANNOTATION
-------------

Each (Possessor, Possessee) pair has annotations for Possession Existence (Yes/Never/Unknown/Invalid), possession type (Alienable/Control) and three temporal tags Before (Yes/No), During (Yes/No) and  After (Yes/No) as explained in section 4.2.

The file contains the token numbers for the possessor, possessee and verb (refer section 4.1) as they appear in OntoNotes 5.0.

-------------
FORMAT
-------------
The csv file contains the following columns:

sent_file: 		Filename in OntoNotes corpus.
sent_part: 		Part number in OntoNotes corpus.
sent_num: 		The sentence number in OntoNotes corpus (sent_file, sent_part and sent_num together identify a sentence in the OntoNotes corpus).
Possessor_ID:		The starting token number indicating the possessor identified.
Possessee_ID:		The token number idicating the possessee identified.
Verb_ID:		The token number indicating the verb identified.
Possession_existence:	Label indicating possession existence.	
Possession_Type:	Label indicating possession type, if the possession existence is 'Yes'.
Duration_before:	Label indicating temporal anchor before, if the possession existence is 'Yes'.
Duration_during:	Label indicating temporal anchor during, if the possession existence is 'Yes'.
Duration_after:		Label indicating temporal anchor after, if the possession existence is 'Yes'.
