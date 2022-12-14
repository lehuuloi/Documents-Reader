# Dataset for pdf-struct (Logical structure analysis tool for visually structured documents)

This is the dataset to reproduce the experiments for pdf-struct, a tool for extracting fine-grained logical structures (such as boundaries and their hierarchies) from visually structured documents (VSDs) such as PDFs.

Please visit the website at https://github.com/stanfordnlp/pdf-struct for data specifications and other details.

## Dataset specification

Our dataset consists of following files:

```
pdf-struct-dataset/
  - contract_pdf_en/
    - raw/
    - anno/
    - source.tsv
  - contract_pdf_ja/
  - contract_text_en/
  - legistration_pdf_en/
  - LICENSE
  - README.md
```

Each root-level directory represents a single type of dataset: 

* `contract_pdf_en/`: English NDAs in PDF format
* `legistration_pdf_en/`: English executive orders from local authorities
* `contract_text_en/`: English NDAs in visually structured plain text format
* `contract_pdf_ja/`: Japanese NDAs in PDF format

Raw documents are located in `raw/` directory.
Annotated data (generated by `pdf-struct init-dataset` and then annotated by hand) is located in `anno/` directory.
`source.tsv` shows the URL that each document was obtained from.

## Changelog and release note

* 11/7/2021: Initial release
