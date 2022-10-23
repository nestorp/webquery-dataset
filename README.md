#  WebQuery

This dataset is released as part of the paper "Automated Query Generation for Evidence Collection from Web Search Engines".
It's geared towards the development of systems for automated evidence collection from the web, with the purpose of assisting fact-checking.

The WebQuery dataset is composed of 390 claims extracted from news articles. Each claim is manually annotated with a search query used to find verifying evidence in the web, as well as a target URL.

### Data Format
Each sample contains 7 fields:
- claim_id: The ID of the claim. 
- headline: Headline of the article from where the claim was extracted.
- claim_text: Text of the claim
- target_search_query: Human-generated search query
- target_url: URL containing the evidence necessary to verify the claim
- target_url_clean: The target URL, stripped of protocol and query parameters
- evidence_snippet: The evidence sentence extracted from the target URL

Most of the experiments in the related paper were performed using 4-fold cross-validation. Thus, we publish the data splits for each of the folds in the `k0`-`k3` directories. Each directory contains a train, dev and test set. We also share the full dataset in a single file in `all_data`.tsv.

Please, cite the following paper if you use the dataset or the models in this repository:
```bib
coming soon
```



