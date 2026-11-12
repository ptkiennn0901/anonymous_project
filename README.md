# ViMed-Rad: Anonymous Review Repository

This repository supports anonymous peer review of the ViMed-Rad benchmark. It documents the planned release format for representative, de-identified image--report samples, example VQA annotations, and reproduction materials.

## Current contents

- `docs/DATASET_CARD.md` describes the intended scope, data governance, and release limitations.
- `data/` defines the delivery layout for X-ray, CT, MRI, and PET/CT samples.
- `annotations/` contains a synthetic, non-clinical VQA-format example and its schema.
- `RELEASE_CHECKLIST.md` lists the mandatory privacy review before any hospital-derived image or report is added.

## Data availability

No hospital-derived image, report, patient identifier, or accession identifier is included in this repository yet. Representative samples will be added only after de-identification review, including screening for pixel-level identifiers and free-text protected health information. The full ViMed-Rad dataset remains subject to institutional data-sharing and patient-privacy requirements.

## Planned sample layout

Each approved sample will use a repository-local random ID, such as `xray_sample_001`, rather than a source study or patient identifier. Source filenames, directory names, dates, and DICOM/NIfTI metadata that could enable re-identification will not be released.

See the dataset card and release checklist for details.
