# Deutsche - KreuzWÖRTER

This is a scored german wordlist for constructing crosswords. It should be used with any online constructing tool. The drawback is that the scoring was not done manually and as such it's not perfect.

## How was it created?

Transformations:
 - remove any words with numbers
 - remove any words with characters that are not in the latin abc or german umlaute
 - Transform umlaute into their expanded ue, ae etc... form

Filtering:
 - remove any words longer than 21 characters (as they would not fit in any grid)

Scoring:
 - https://www.crossword-compiler.com/en/help/html/aboutwordlistscoring.htm
 - Score root words as 50 and derivatives as 25 (root words meaning singular and plural forms, but not declined)
 - Use the data on word frequency from the uni-leipzig wordlist to slightly boost or reduce the scores of words.

## Sources

I used two main sources for the words in this list:
 - https://wortschatz.uni-leipzig.de/de/download/German 
    - cite http://www.lrec-conf.org/proceedings/lrec2012/pdf/327_Paper.pdf
	D. Goldhahn, T. Eckart & U. Quasthoff: Building Large Monolingual Dictionaries at the Leipzig Corpora Collection: From 100 to 200 Languages.
	In: Proceedings of the 8th International Language Resources and Evaluation (LREC'12), 2012

 - Aspell-de `aspell -d de dump master | aspell -l de expand > my.dict` (https://www.reddit.com/r/FragReddit/comments/8i4e1n/gibt_es_ein_deutsches_w%C3%B6rterbuch_zum_download/)
