# LEPOR
LEPOR: Automatic Machine Translation Evaluation Metric with tunable parameters and augmented factors

cmd command example:
Perl the-evaluation-code.pl > score-file.txt

Thanks to Paolo Dr. (Awsome) Bolzoni, It generates the sentence-level score and the system-level score as WMT metrics submission format. e.g. 

http://www.statmt.org/wmt18/metrics-task.html 

"METRIC NAME, LANG-PAIR, TEST SET, SYSTEM, SEGMENT NUMBER, SEGMENT SCORE, ENSEMBLE, AVAILABLE"

"METRIC NAME, LANG-PAIR, TEST SET, SYSTEM, SYSTEM, SYSTEM LEVEL SCORE, ENSEMBLE, AVAILABLE"

-------------
For all the files about hLEPOR_baseline in WMT2019, e.g. rerun hLEPOR baseline for comparesion or improvement etc. you can find them all in this drive folder: (https://drive.google.com/open?id=1v6VR4r5U9tH-0jFzAtxTybxCJWUeCWdn)

- achieved best level performace metrics in German-Czech system-level MT evaluation. Pearson correlation score with human judegment: 0.959.

We call it baseline in WMT2019 because we did not tune the parameters in the metric and did not use the linguistic features that we used in WMT2013 either. Instead, just used a set of default parameters and only measure the scores according ot the system output and reference files, no external resources used.

There is a deep statistical analysis about hLEPOR and nLEPOR performance in WMT13, which shows it performed as one of the best metrics "in both the individual language pair assessment for Spanish-to-English and the aggregated set of 9 language pairs.", see the paper (Accurate Evaluation of Segment-level Machine Translation Metrics) "https://www.aclweb.org/anthology/N15-1124" Graham et al. 2015 NAACL(https://github.com/ygraham/segment-mteval)


-------------
Citation:

COLING:

@inproceedings{han2012lepor,
  title={LEPOR: A Robust Evaluation Metric for Machine Translation with Augmented Factors},
  author={Han, Aaron L.-F. and Wong, Derek F. and Chao, Lidia S.},
  booktitle={Proceedings of the 24th International Conference on Computational Linguistics (COLING 2012)},
  pages={441-450},
  year={2012},
  organization={Association for Computational Linguistics}
}

MT SUMMIT:

@inproceedings{han2013language,
  title={Language-independent Model for Machine Translation Evaluation with Reinforced Factors},
  author={Han, Aaron L.-F. and Wong, Derek F. and Chao, Lidia S. and He, Liangye and Lu, Yi and Xing, Junwen and Zeng, Xiaodong},
  booktitle={Machine Translation Summit XIV},
  pages={215--222},
  year={2013},
  organization={International Association for Machine Translation}
}

WMT:

@inproceedings{W13-2253,
    title = "A Description of Tunable Machine Translation Evaluation Systems in {WMT}13 Metrics Task",
    author = "Han, Aaron Li-Feng  and
      Wong, Derek F.  and
      Chao, Lidia S.  and
      Lu, Yi  and
      He, Liangye  and
      Wang, Yiming  and
      Zhou, Jiaji",
    booktitle = "Proceedings of the Eighth Workshop on Statistical Machine Translation",
    month = aug,
    year = "2013",
    address = "Sofia, Bulgaria",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/W13-2253",
    pages = "414--421",
}

Msc. thesis:

@article{DBLP:journals/corr/Han17,
  author    = {Lifeng Han},
  title     = {{LEPOR:} An Augmented Machine Translation Evaluation Metric},
  journal   = {CoRR},
  volume    = {abs/1703.08748},
  year      = {2017},
  url       = {http://arxiv.org/abs/1703.08748},
  archivePrefix = {arXiv},
  eprint    = {1703.08748},
  timestamp = {Mon, 13 Aug 2018 16:48:22 +0200},
  biburl    = {https://dblp.org/rec/bib/journals/corr/Han17},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}

-------------

Paper that used LEPOR (hLEPOR, nLEPOR) for their work:

Marzouk, S. & Hansen-Schirra, S. Machine Translation (2019). https://doi.org/10.1007/s10590-019-09233-w







