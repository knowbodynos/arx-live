# arX-Live

## An arXiv-trend predictive engine!

Uses:
---

1) The [arXiv API](https://arxiv.org/help/api/index).

2) Natural Language Toolkit (NTLK).

Works by:
---

1) Scraping eprint abstracts from the [arXiv](https://arxiv.org/) servers from any query.

2) Cleaning eacho abstract by removing MathJax/LaTeX tags, extra whitespace, punctuation, and common stopwords, and then by fixing the case of the remaining text.

3) Grouping most common bigram and trigram collocations into monograms for each abstract (preserves most technical phrases).

4) Filtering out non-technical terminology in each of the abstracts (i.e. NTLK's corpus of English-language words).

5) Computing the frequencies of each buzzword in the abstracts over a rolling time window.