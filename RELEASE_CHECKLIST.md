# Privacy release checklist

Before adding any hospital-derived image, report, or annotation:

- [ ] Replace source case, patient, encounter, accession, and series identifiers with random repository-local IDs.
- [ ] Remove direct identifiers from filenames, directory names, JSON fields, and metadata.
- [ ] Check image pixels for burned-in identifiers, including overlays and screenshots.
- [ ] Re-export or otherwise inspect DICOM/NIfTI headers and extensions for identifiers.
- [ ] Review report text for names, dates, locations, provider details, and other protected health information.
- [ ] Confirm that image--report links do not expose source-system URLs or identifiers.
- [ ] Obtain the required institutional and privacy approvals for the planned release scope.
- [ ] Record the de-identification method and release version in the dataset card.
