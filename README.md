# rewordQALD9

This is an extended version of the QALD dataset, a well-known benchmark resource used for the task of Question Answering over knowledge graphs (KGQA). 
The purpose of this work is to make available a) high-quality data even for languages other than English, and b) multiple reformulations of the same question, to test systems' robustness. The QALD version we used is the one released for the 9th edition of the challenge of Question Answering over Linked Data [QALD9](https://github.com/ag-sc/QALD/tree/master/9/data), and the languages involved are English and Italian. Besides a revised and improved quality of Italian translations of questions, the resource presented here features a number of alternative rewordings of both English and Italian questions. 
The dataset has been encoded in the QALD-JSON format.

## Dataset overview

The dataset includes, in addition to the approximately 550 original questions, a total of 995 paraphrases for the English section and 1,156 for the Italian section, and an overall amount of 1546 questions for English and 1707 for Italian. 
Few instances of duplicate questions from the original QALD9 were also removed.

| Lang.  | Split |Orig. questions|Paraphrases|Tot. Questions |
|------- |:-----:|:-------------:|:---------:|:-------------:|
|  En    |Train  | 405           |  729      | 1134          |
|        |Test   | 146           |  266      | 412           |
|  It    |Train  | 405           |  843      | 1248          |
|        |Test   | 146           |  313      | 459           |    


## Evaluation

A preliminary baseline evaluation was conducted using [QAnswer](https://content.iospress.com/articles/semantic-web/sw190343) via [GERBIL](www.gerbil-qa.aksw.org/gerbil/config). 

Here are the main results on the rewordQALD9 test set and for the F1-QALD measure only. To see the complete results for Macro/Micro-Precision/Recall/F1, please follow through GERBIL's permanent URIs of the experiments:

|                           | 	EN	 | IT     |
|---------------------------|:------:|:------:|
|rewordQALD9                | [0.3186](http://www.gerbil-qa.aksw.org/gerbil/experiment?id=202206290011) | [0.2603](http://www.gerbil-qa.aksw.org/gerbil/experiment?id=202206280034) |
|rewordQALD9 (paraph.only)  | [0.3113](http://www.gerbil-qa.aksw.org/gerbil/experiment?id=202206290006) | [0.244](http://www.gerbil-qa.aksw.org/gerbil/experiment?id=202206290009)  |






