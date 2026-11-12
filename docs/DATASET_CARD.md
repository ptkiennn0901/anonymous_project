# Dataset card

## Purpose

ViMed-Rad is a multimodal radiology benchmark intended to support image understanding, report-grounded tasks, and visual question answering (VQA). This anonymous review repository is designed to make the proposed release structure and annotation format inspectable without distributing unreviewed hospital-derived data.

## Intended modalities

| Modality | Planned content |
| --- | --- |
| X-ray | De-identified radiograph samples and associated de-identified reports, when approved. |
| CT | De-identified image volumes or approved derived images and associated de-identified reports. |
| MRI | De-identified image volumes or approved derived images and associated de-identified reports. |
| PET/CT | De-identified image volumes or approved derived images and associated de-identified reports. |

## Privacy and governance

The source data are hospital-derived. Broader release of the full dataset is subject to institutional data-sharing approval, applicable patient-privacy regulations, and removal of identifiers from both image pixels and associated text. The repository must not include source study IDs, admission IDs, PACS links, dates, provider names, or other direct or quasi-identifiers.

## Annotation format

The files in `annotations/` show the proposed JSON schema. The included record is synthetic and exists only to demonstrate field names and evaluation formatting; it is not derived from a clinical image or report.

## Reproducibility

Implementation code and reproduction instructions are intended for public release upon publication. This repository will document the exact split definitions, preprocessing version, task prompts, and evaluation scripts used for the public benchmark subset.
