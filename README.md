# omer_gene_tumour_gene_list
Hacking LLM / agentic AI pipelines for OB gene lists

Sketch of planned workflows:

<img width="1134" height="641" alt="image" src="https://github.com/user-attachments/assets/7878bf70-e508-4833-a241-ea055fd9db72" />


### Experiment 1:

Paper: A spatiotemporal cancer cell trajectory underlies glioblastoma heterogeneity https://www.biorxiv.org/content/10.1101/2025.05.13.653495v1 

Aim1: use LLM queries with context to generate predictions of potentially relevant processes/states/interactions from gene lists for 'types' (Table S5):

Malignant | AC-gliosis-like | AC-gliosis-like 1 | ['POSTN',   'JPH1', 'EYA4', 'RTN1', 'LAMA2', 'AC092957.1', 'TNC', 'IGFBP7', 'COL23A1',   'NAMPT']
-- | -- | -- | --
Malignant | AC-gliosis-like | AC-gliosis-like 2 | ['CFAP54', 'IGFBP7',   'VOPP1', 'AQP4', 'LANCL2', 'AC074351.1', 'DTHD1', 'AC012405.1', 'RTN1',   'MTRNR2L12']
Malignant | AC-gliosis-like | AC-gliosis-like 3 | ['LAMA2', 'AC012405.1',   'COL8A1', 'AC007402.1', 'IGFBP7', 'TNC', 'APOLD1', 'CCN1', 'SLC25A18',   'CST3']
Malignant | AC-gliosis-like | AC-gliosis-like 4 | ['CST3', 'MTRNR2L12',   'SPP1', 'APOE', 'IGFBP7', 'AQP4', 'CHI3L1', 'CRYAB', 'CXCL14', 'VOPP1']

Code and results in notebooks/experiment1

Outputs:
  
 - deepsearch_caroline: Review this first.  Deepsearch with improved referencing
 - deepsearch: deepsearch queries - refs unerliable and limited.
 -  pro - queries run without deepsearch.
 -  PaperQA_Crow_Manual - manually added example of [PaperQA](https://platform.futurehouse.org/) Crow search.  Appears to be high quality and well referenced (including text extracts from papers). We may switch to this in future but more work needed to autoamte.

Next steps: Run KG agent across results.

