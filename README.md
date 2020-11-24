# Information Retrieval


Converting ```ms-marco.trec.gz``` to lucene index:
```
python -m pyserini.index -collection CleanTrecCollection -generator DefaultLuceneDocumentGenerator -threads 1 -input C:/msmarco-docs.trec -index C:/msmarco-doc/lucene-index.msmarco-doc.pos+docvectors+rawdocs -storePositions -storeDocvectors -storeRaw
```

where ```-input``` specifies the folder with the file ```ms-marco.trec.gz``` and ```-index``` specifies the output folder. Pyserini needs to be installed.


To use ```trec_eval.exe```, cygwin must be installed and ```C:/cygwin64/bin``` must be added to the system and environment ```PATH``` variable.
