# Analyse PTA with Jupyter Notebooks

This repository contains several Jupyter Notebooks to explore the Patristic Text Archive beyond the tools provided in the web frontend.

## Run Jupyter Notebooks in Binder

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/PatristicTextArchive/analyse_data/HEAD)

## This repository contains the following notebooks

- `pta_nlp_cld.ipynb` using [CLD](https://cld.bbaw.de)
- `pta_nlp_spacy.ipynb` using [grc_proiel_sm](https://huggingface.co/Jacobo/grc_proiel_sm) (cf. [greCy. Ancient Greek models for spaCy](https://github.com/jmyerston/greCy))
- `keywords-in-context.ipynb`
- `collocations.ipynb`
- `analyse_corpus.ipynb` (using [TF-IDF](https://en.wikipedia.org/wiki/Tf%E2%80%93idf))
- `biblical_quotations.ipynb` (using `severian_quotes.json` and [pta_metadata](https://github.com/PatristicTextArchive/pta_metadata) repository)
- `convert_pta_totext.ipynb` Helper notebook to convert PTA-XML to a csv file
- `lemmatize_all.ipynb` Helper notebook to lemmatize all text generated by convert_pta_totext.ipynb

## Data for use in notebooks

### in folder `data`

- `DejaVuSans.ttf` (to be able to use Greek Extended in wordclouds)
- `severian_plaintext.csv` as generated by `convert_pta_totext.ipynb`
- `severian_plaintext_lemmatized.csv` as generated by `lemmatize_all.ipynb`
- `severian_quotes.json` as generated by `convert_pta_totext.ipynb`

### in folder `assets`

- SpaCy model `grc_proiel_sm-3.7-py3-none-any.whl` (downloaded from https://huggingface.co/Jacobo/grc_proiel_sm and filename adjusted to adhere to format convention of pip > 24.1)