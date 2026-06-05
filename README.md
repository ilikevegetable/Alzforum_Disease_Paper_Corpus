# Alzforum Disease Paper Corpus

A list of **1,065 Alzheimer's-disease-related research papers** used as the
external knowledge base for the RAG benchmarking experiments in:

> Feng et al. *A benchmark of retrieval-augmented generation methods for
> Alzheimer's disease research.* (Manuscript in preparation.)

## What's in this repository

| File | Description |
|---|---|
| `alzforum_1065_corpus.csv` | The 1,065 papers as a structured list (PMC ID, PMC URL, title, DOI, PMID, journal, year). |
| `LICENSE` | MIT license **for this metadata listing only** (see below). |

The CSV is sorted by PMC ID. Each row has these columns:

- `pmc_id`   — PMC identifier, e.g. `PMC10031303`
- `pmc_url`  — Direct link to the article on PubMed Central, e.g.
  `https://pmc.ncbi.nlm.nih.gov/articles/PMC10031303/`
- `title`    — Article title
- `doi`      — DOI (when available)
- `pmid`     — PubMed identifier
- `journal`  — Journal name
- `year`     — Publication year

## Why metadata only, not full text

Full-text content for each paper is **not** redistributed from this
repository. Many of these articles are protected by publisher copyright,
even when they are freely readable through PubMed Central. Republishing
the full text would require explicit permission from each publisher.

The CSV is provided so that researchers can:

1. Reproduce the corpus used in the benchmark by retrieving each paper
   directly from its publisher via the supplied `pmc_url` (or via `doi`
   / `pmid`).
2. Cite individual papers in their own follow-up work.

Most papers in this corpus are part of the **PubMed Central Open Access
Subset** and can be downloaded in full from PMC under their respective
Creative Commons licenses. A small minority are author manuscripts or
publisher-deposited articles available for reading on PMC but subject
to publisher copyright; please consult each article's PMC page for its
license terms before redistributing the full text.

## License

The `LICENSE` file applies only to the **metadata listing** in this
repository (the CSV file and the README). It does **not** grant any
rights over the original articles themselves, which remain the property
of their respective copyright holders.
