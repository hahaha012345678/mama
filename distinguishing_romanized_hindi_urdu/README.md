# Supporting Materials for "Distinguishing Romanized Hindi from Romanized Urdu"

This document provides a brief summary of materials released here in support of
the paper "Distinguishing Romanized Hindi from Romanized Urdu", which
appeared in the 
[CAWL workshop at ACL, 2023](https://aclanthology.org/2023.cawl-1.5/). 

**full_list.tsv** contains the set of linguist-derived seed-words used throughout
 the paper to distinguish romanized Hindi and Urdu. It is organized into 5
 columns, including Hindi words in native and roman script, the equivalent
 Urdu word in native and roman script, and their shared gloss.

The included tarball, cawl2023_data.tgz, is split into 65 1M
chunks (suffixed by `-X-of-00065.tgz`) using Unix `split -b1000K`. It can be
concatenated via `cat` to reform a single file, and expanded as normal
using `tar -xvzf`. It contains the following datasets referenced in
the paper. All datasets are in TSV format, with the first column containing a
string, and the second column containing as label - either *"ur"* (Urdu) or
*"hi"* (Hindi).

-   **gen_train.tsv**: Strings generated by mT5 via template filling (see
    section 4.2).
-   **mc4_train.tsv**: Strings drawn from the hi-Latn portion of mc4, according
    to whether they contain Hindi or Urdu seed words (see section 4.1)
-   **topline_train.tsv**: Hand-labeled Wikipedia sentences from the Dakshina
    dataset (see section 4.1).
-   **topline_dev.tsv**: Evaluation set held out from the Dakshina dataset.




[Elizabeth Nielsen, Christo Kirov, and Brian Roark. 2023. Distinguishing romanized Hindi from romanized Urdu. In Proceedings of the Workshop on Computation and Written Language: CAWL 2023, pages 33–42, Toronto, Canada. Association for Computational Linguistics.](https://aclanthology.org/2023.cawl-1.5.pdf)
