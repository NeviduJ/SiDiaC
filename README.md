# SiDiaC: Sinhala Diachronic Corpus

A curated collection of Sinhala literary texts and related resources with OCR outputs and basic metadata for each work. This repository organizes original PDFs alongside finalized OCR text and machine-readable `metadata.json` files per title.

### Repository structure
- `Books_PDF/`: Original source PDFs for each title.
- `OCR_Final/`: Finalized OCR results per title, each directory containing:
  - `metadata.json`: Minimal bibliographic and processing metadata
  - `<title>.txt`: Plain text content extracted via OCR

### Example metadata.json
```json
{
  "title": "පන්සිය පනස් ජාතක පොත",
  "title_en": "Pansiya Panas Jathaka Potha",
  "author": "Unknown",
  "author_en": "Unknown",
  "genre": "Fiction; Religious",
  "issued_date": "1881",
  "written_date": "1303 - 1333",
  "ocr_confidence": 0.9987
}
```

### Goals
- Preserve Sinhala texts in accessible, searchable formats.
- Provide lightweight, consistent metadata to enable downstream use.

### Contributing
1. Literary works under `Books_PDF/<Work Name>.pdf` and `OCR_Final/<Work Name>/`.
2. Includes both `metadata.json` and a UTF-8 encoded `<Work Name>.txt`.

### Notes
- Filenames and directory names may include Sinhala characters.
- `ocr_confidence` is a heuristic score from the OCR process and may vary by work.

### Citation

```json
@misc{jayatilleke2025sidiacsinhaladiachroniccorpus,
      title={SiDiaC: Sinhala Diachronic Corpus}, 
      author={Nevidu Jayatilleke and Nisansa de Silva},
      year={2025},
      eprint={2509.17912},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2509.17912}, 
}
```
