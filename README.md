# disambiguation
Concept Disambiguation between textual languages

Words like "dindon" and "turquie" both mean "turkey" in English, leading to errors in single word query disambiguation. Find all english terms that might cause such issues in some popular languages (fr, es, de).

## Plan of Attack

Utilize MUSE multilingual dictionaries to find all the english terms that might occur multiple times. For example, the concept "turkey" occurs 4 times

```
turquie turkey
dinde turkey
dindons turkeys
```

Utilize fasttext embeddings in the respective language and DBSCAN to run clustering and find ambiguous terms.
