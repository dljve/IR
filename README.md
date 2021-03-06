# Information Retrieval

#### Indexes

Converting ```ms-marco.trec.gz``` to lucene index:
```
python -m pyserini.index -collection CleanTrecCollection -generator DefaultLuceneDocumentGenerator -threads 1 -input C:/msmarco-docs.trec -index C:/msmarco-doc/lucene-index.msmarco-doc.pos+docvectors+rawdocs -storePositions -storeDocvectors -storeRaw
```

where ```-input``` specifies the folder with the file ```ms-marco.trec.gz``` and ```-index``` specifies the output folder. Pyserini needs to be installed.

#### Evaluation

To use ```trec_eval.exe```, cygwin must be installed and ```C:/cygwin64/bin``` must be added to the system and environment ```PATH``` variable.

#### Links
- [Glove 300d word embeddings](https://drive.google.com/file/d/1Y6022PHZp8PhRicet5qGyMg2tbmV8i31/view?usp=sharing)
- [MSMARCO docs lucene index](https://drive.google.com/file/d/13rQQbZndcqRNZ2oHSG_WKVlcYCDUHYUX/view)
- [MSMARCO docs trec gz](https://drive.google.com/file/d/145-oX04S0TFKPEP5TwGCAlXfsiAs7MnP/view?usp=sharing)
