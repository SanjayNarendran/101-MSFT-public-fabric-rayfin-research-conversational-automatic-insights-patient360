# Notices

`index.html` embeds fonts, medical images and product icons that are not covered by the MIT licence of this
repository. Each keeps the licence or terms listed here. File names are those of the presentation's source, where
each image or icon is a separate file.

## Fonts

Set in Fira Sans, Fira Sans Condensed and Fira Mono ([mozilla/Fira](https://github.com/mozilla/Fira)), embedded
under the SIL Open Font License 1.1 ([`FiraSans-LICENSE.txt`](FiraSans-LICENSE.txt)).

## Medical images

The medical images in Fig 7 (section 06) are the ones the Explore notebook of the demo-mode delivery of request 1005
shows. They were read from Bronze_ImagingArchive and saved as small WebP files. The CT frames are the notebook's own:
a lung window, with the LIDC radiologist's outline of the study's largest nodule drawn in orange. The other images were
scaled to 360 px. The DICOM headers in the archive carry the demo's synthetic patients; the images themselves are
unchanged research data.

| File | Image | Source | Licence |
|---|---|---|---|
| `ct-slices.webp`, `ct-closeup.webp` | 8 chest CT slices and their close-ups, with the nodule outline from a DICOM SEG object | LIDC-IDRI, patient LIDC-IDRI-0230, from [NCI Imaging Data Commons](https://imaging.datacommons.cancer.gov/) ([doi:10.7937/K9/TCIA.2015.LO9QL9SX](https://doi.org/10.7937/K9/TCIA.2015.LO9QL9SX)) | CC BY 3.0 |
| `dx.webp` | Chest X-ray (DX) | LIDC-IDRI, patient LIDC-IDRI-0248, as above | CC BY 3.0 |
| `sm.webp` | Pathology slide thumbnail (SM) | TCGA-BRCA, patient TCGA-E2-A1IL, from NCI Imaging Data Commons ([doi:10.5281/zenodo.12689962](https://doi.org/10.5281/zenodo.12689962)) | CC BY 3.0 |
| `mr.webp` | Brain MR slice | [Synthea Coherent Data Set](https://registry.opendata.aws/synthea-coherent-data/), The MITRE Corporation (simulated) | CC BY 4.0 |

The images in Figs 8 and 9 (sections 07 and 08) are the ones Patient 360 shows for Levi Hills, Damian Macejkovic and
Jettie Osinski. The CT frames were rendered from Levi Hills' CT in the imaging archive the way the app's viewer shows
it: a lung window, with each nodule outlined where at least half of the LIDC radiologists who marked it drew it. The
slides were stitched from the app's deep-zoom tiles. The lymphocyte maps keep one pixel per 50 µm square of tissue.
Levi Hills is one of the demo's synthetic patients, with research images under him; Damian Macejkovic and Jettie
Osinski are TCGA cases with synthetic names.

| File | Image | Source | Licence |
|---|---|---|---|
| `levi-ct-axial.webp`, `levi-ct-coronal-n1.webp`, `levi-ct-coronal-n6.webp`, `levi-ct-sagittal-n1.webp`, `levi-ct-sagittal-n6.webp` | Chest CT: 15 axial slices from nodule 1 to nodule 6, and the coronal and sagittal planes through each, with the nodule outlines | LIDC-IDRI, patient LIDC-IDRI-0510, from NCI Imaging Data Commons ([doi:10.7937/K9/TCIA.2015.LO9QL9SX](https://doi.org/10.7937/K9/TCIA.2015.LO9QL9SX)) | CC BY 3.0 |
| `levi-slide.webp`, `levi-slide-13.webp`, `levi-slide-14.webp` | H&E slide: the whole slide and two crops at 10× and 20× | TCGA-LUSC, patient TCGA-94-7943, from NCI Imaging Data Commons ([doi:10.5281/zenodo.12689962](https://doi.org/10.5281/zenodo.12689962)) | CC BY 3.0 |
| `damian-slide.webp`, `damian-slide-15.webp`, `damian-slide-16.webp`, `jettie-slide.webp` | Diagnostic H&E slides: the whole slides, and two crops of TCGA-60-2722's at 10× and 20× | TCGA-LUSC patient TCGA-60-2722 and TCGA-LUAD patient TCGA-J2-8192, from the [NCI Genomic Data Commons](https://portal.gdc.cancer.gov/) | NIH GDC open access; cite the TCGA Research Network |
| `damian-til.webp`, `jettie-til.webp` | AI lymphocyte (TIL) maps of those two slides | Stony Brook TCGA TIL maps, Saltz J et al., Cell Reports 2018 ([doi:10.5281/zenodo.16966285](https://doi.org/10.5281/zenodo.16966285)) | CC BY 4.0 |

## Product icons

Product icons used in the presentation's figures, unmodified, with where each one comes from and the terms it is used under.

| File | Icon | Source | Terms |
|---|---|---|---|
| `fabric.svg`, `databases.svg`, `data-factory.svg`, `analytics.svg`, `real-time-intelligence.svg`, `power-bi.svg`, `copilot.svg`, `onelake.svg`, `rayfin.svg`, `lakehouse.svg`, `notebook.svg`, `pipeline.svg`, `report.svg` | Microsoft Fabric, its workloads, Copilot, OneLake and Rayfin, and the lakehouse, notebook, data pipeline and report item icons used in sections 01 to 08 (`analytics.svg` is the Fabric data science workload icon; `databases.svg` also marks Bronze_PACS) | npm package [`@fabric-msft/svg-icons`](https://www.npmjs.com/package/@fabric-msft/svg-icons) 12.0.0, 48 px colour icons | [Microsoft Fabric icon terms](https://learn.microsoft.com/fabric/fundamentals/icons): permitted in architectural diagrams, training materials and documentation |
| `folder.svg`, `folder-shortcut.svg`, `table.svg` | The folder, shortcut folder and table icons of the lakehouse explorer in section 05 (`folder_20_non-item.svg`, `folder_shortcut_20_regular.svg`, `table_header_20_regular.svg`; the two single-colour ones are drawn inline in the page's text colour) | npm package `@fabric-msft/svg-icons` 12.0.0, 20 px icons | as above |
| `iq.png` | Fabric IQ | Supplied by the presenter from Microsoft's Fabric slides (there is no IQ icon in the public Fabric icon set); transparent margin trimmed and scaled to 160 px tall | Microsoft product icon, used to identify Fabric IQ |
| `mirrored-catalog.svg` | The mirrored Azure Databricks catalog in section 01 | npm package `@fabric-msft/svg-icons` 12.0.0, `mirrored_catalog_48_item.svg` | Microsoft Fabric icon terms, as in the first row |
| `functions.svg` | Rayfin functions in section 07, shown with the Fabric user data functions item icon | npm package `@fabric-msft/svg-icons` 12.0.0, `user_data_functions_48_item.svg` | Microsoft Fabric icon terms, as in the first row |
| `governance-purview.svg` | Governance, shown with the Microsoft Purview icon | same package, `purview_48_color.svg` | as above |
| `azure-storage.svg` | Azure (Storage accounts) | [Azure architecture icons](https://learn.microsoft.com/azure/architecture/icons/) V24, `10086-icon-service-Storage-Accounts.svg` | Azure icon terms: permitted in architectural diagrams, training materials and documentation |
| `on-premises.svg` | On‑premises (Server farm) | Azure architecture icons V24, `10835-icon-service-Server-Farm.svg` | as above |
| `dataverse.svg` | Dataverse | [Microsoft Power Platform icons](https://learn.microsoft.com/power-platform/guidance/icons), `Dataverse_scalable.svg` | Power Platform icon terms: permitted in architectural diagrams, training materials and documentation |
| `amazon-s3.svg` | Amazon S3 | [AWS Architecture Icons](https://aws.amazon.com/architecture/icons/) (July 2026 package), `Arch_Amazon-Simple-Storage-Service_64.svg` | AWS permits these icons in architecture diagrams and presentations |
| `google-cloud-storage.svg` | Google Cloud (Cloud Storage) | [Google Cloud product icons](https://cloud.google.com/icons), core product icons, `Cloud_Storage-512-color.svg` | Google Cloud's official icon library for diagrams and documentation |
| `databricks.svg`, `snowflake.svg` | Databricks, Snowflake | [Simple Icons](https://simpleicons.org) 16.36.0, filled with each brand's colour (#FF3621, #29B5E8) | Simple Icons is CC0; the marks remain trademarks of Databricks, Inc. and Snowflake Inc. |
| `container-apps.svg` | Azure Container Apps, which hosts Patient 360's chat relay in section 08 | Azure architecture icons V24, `02989-icon-service-Container-Apps-Environments.svg` | Azure icon terms: permitted in architectural diagrams, training materials and documentation |
| `sql-server.svg` | SQL Server on premises, on the Epic stack in section 01 | Azure architecture icons V24, `10132-icon-service-SQL-Server.svg` | Azure icon terms: permitted in architectural diagrams, training materials and documentation |
| `microsoft-foundry.svg` | Microsoft Foundry | Azure architecture icons V24, `035746832-icon-service-AI-Foundry.svg` | Azure icon terms: permitted in architectural diagrams, training materials and documentation |
| `github-copilot.svg` | GitHub Copilot | [Primer Octicons](https://github.com/primer/octicons) `copilot-48.svg`, filled #1F2328 (the page inverts it to white on the dark theme, as GitHub's single-colour mark allows) | MIT, © GitHub Inc.; GitHub Copilot is a trademark of GitHub, Inc. |
| `epic.svg` | Epic (shown for Epic Cogito Cloud in section 01) | [Wikimedia Commons, `Epic_Systems.svg`](https://commons.wikimedia.org/wiki/File:Epic_Systems.svg); the Inkscape metadata removed and the viewBox trimmed to the wordmark, path and colour (#BA0239) unchanged | Public domain on Commons (a text logo); Epic is a trademark of Epic Systems Corporation |

All product names, logos and icons are trademarks of their owners. They identify the products described and don't imply endorsement.
