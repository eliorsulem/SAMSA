# SAMSA
SAMSA Evaluation Metric and Human Evaluation Benchmark for Text Simplification

If you use the metric or the benchmark, please cite the following paper:

      Semantic Structural Evaluation for Text Simplification
      Elior Sulem, Omri Abend and Ari Rappoport
      Proc. of NAACL 2018
## Dataset
**./human_evaluation_benchmark.ods**

Human evaluation scores given by 5 annotators for the 4 elicitation questions described in the paper.
Each annotator scored the same 700 (input,output) pairs.

The source sentences and the system outputs can be found at http://homepages.inf.ed.ac.uk/snaraya2/data/simplification-2016.tgz.

## Code
### Requirements:
Python NLTK, [UCCA toolkit](https://github.com/danielhers/ucca), [Monolingual word aligner](https://github.com/ma-sultan/monolingual-word-aligner)

[TUPA parser](https://github.com/danielhers/tupa) for parsing the source side.

**./scene_sentence_extraction.py**

**./scene_sentence_alignment.py** 

**./SAMSA_score.py**: The SAMSA metric

**./SAMSA_abl_score.py**: The SAMSA metric without the non-splitting penalty
