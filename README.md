# ViMed-Rad: Vietnamese Multimodal Radiology Dataset and Benchmark

This anonymous repository accompanies the paper **“Unifying Medical Vision-Language Learning Across Imaging Modalities in Vietnamese: A Multimodal Dataset and Benchmark.”**

ViMed-Rad contains 93,781 radiology studies paired with Vietnamese reports across X-ray, CT, MRI, and whole-body PET/CT. ViMed-Bench evaluates report generation and three report-grounded VQA tasks: VQA-Select, VQA-Respond, and VQA-Compose.

## Dataset overview

| Modality | Full dataset | Experimental cohort |
| --- | ---: | ---: |
| X-ray | 62,148 studies | 37,369 chest studies |
| CT | 13,247 studies | 5,428 chest studies |
| MRI | 12,010 studies | 3,649 brain studies |
| PET/CT | 6,376 studies | 2,757 whole-body scans |
| **Total** | **93,781 studies** | — |

The complete dataset contains approximately 28.8 million slices. The source studies are native DICOM acquisitions paired with radiologist-authored Vietnamese reports.

## Public samples for peer review

The repositories below contain de-identified review samples drawn from the predefined train, validation, and test splits. They are provided so reviewers can inspect the imaging data, reports, VQA annotations, and release format. These samples are not the complete ViMed-Rad dataset.

| Modality | Public review sample |
| --- | --- |
| X-ray | [AnonymousPersonViMedRad/vimed-rad-xray-train-val-test](https://huggingface.co/datasets/AnonymousPersonViMedRad/vimed-rad-xray-train-val-test) |
| CT | [AnonymousPersonViMedRad/vimed-rad-ct](https://huggingface.co/datasets/AnonymousPersonViMedRad/vimed-rad-ct) |
| MRI | [vimed-rad-anon/ViMed-Rad-sample](https://huggingface.co/datasets/vimed-rad-anon/ViMed-Rad-sample) |
| PET/CT | [AnonymousPersonViMedRad/vimed-rad-petct](https://huggingface.co/datasets/AnonymousPersonViMedRad/vimed-rad-petct) |

The intended review package contains 140 studies per modality: 100 training, 20 validation, and 20 test studies. The live Hugging Face dataset card for each modality is authoritative for its files, fields, and privacy preparation.

## Complete release upon acceptance

Upon acceptance, we will release:

- all 93,781 de-identified native DICOM studies, including studies not used in the experiments;
- radiologist-authored Vietnamese reports, including normalized CT reports;
- VQA-Select, VQA-Respond, and VQA-Compose annotations;
- train, validation, and test split manifests for every task;
- the selected-series list for each study; and
- preprocessing, training, and evaluation code with the exact configurations used in the paper.

The complete dataset will be hosted as a gated Hugging Face repository under the **CC BY-NC-SA 4.0** licence together with a data use agreement. Applicants will provide their name, affiliation, and intended research use. Access is limited to non-commercial research. Users must not attempt patient re-identification or redistribute the original data. Requests will be reviewed by the authors.

## Intended use

ViMed-Rad is intended for non-commercial research in medical vision-language learning. It is not a clinical device. Generated reports and VQA answers must not be used for diagnosis or patient care without qualified clinical review.

## Citation

The manuscript is currently under double-blind review. Citation information will be added after publication.
