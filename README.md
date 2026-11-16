# Data unification, cohort discovery and delivery, and research on Microsoft Fabric

A presentation that introduces Microsoft Fabric and then walks through a medical research demo built on it, one
section at a time:

1. **Data Unification**: how Epic, a PACS database, DICOM images and clinical documents reach OneLake by shortcuts
   and mirroring
2. **Medallion Architecture**: Bronze, the imaging enrichment, OMOP in Silver and i2b2 in Gold
3. **Semantic Model**: three semantic models in Fabric IQ, and GitHub Copilot asking one of them in plain language
4. **Cohort Discovery**: a researcher's question turned into an i2b2 query and a data request, approved in a Rayfin app
5. **Data Delivery**: the approved patients delivered to a lakehouse of their own by a Data Factory pipeline
6. **Research Platform**: the notebook that comes with the delivery, run cell by cell
7. **Research: Patient 360**: one patient's whole record, with the CT, the biopsy slide and a tumour genome in their
   own viewers
8. **Research: Conversational Insights**: GitHub Copilot answering questions about patients with those viewers

Each section is a motion-graphics figure that plays a step at a time, with a diagram of the Fabric items behind it.

**View it live:** https://sanjaynarendran.github.io/101-MSFT-public-fabric-rayfin-research-conversational-automatic-insights-patient360/

The presentation is a single self-contained HTML file ([`index.html`](index.html)): styles, scripts, fonts, icons and
medical images are all embedded, so it also works offline. Download it and open it in any modern browser (Edge,
Chrome, Safari, Firefox).

> [!IMPORTANT]
> **For demonstration, education and research only.** This presentation shows a demonstration of capability. It is
> not a medical device and nothing in it is clinical guidance. See [Disclaimer](#disclaimer).

## Controls

| Control | Action |
| --- | --- |
| Step chips and Play | Play a figure, or jump to a step |
| ← · → | Previous or next step of the figure in the middle of the window |
| Full view | Show an app screen across the whole window; Esc returns |
| Light · Dark | Colour theme |
| Hide · Show | Fold a section away or open it again |

The figures start by themselves the first time they come into view. With reduced motion set in the operating system,
they don't animate: each opens finished, and the chips jump between steps.

## Credits

Set in [Fira Sans](https://github.com/mozilla/Fira), embedded under the SIL Open Font License
([`FiraSans-LICENSE.txt`](FiraSans-LICENSE.txt)).

All patients are synthetic. Names are Synthea-generated; the research patients in sections 07 and 08 are public,
de-identified TCGA cases shown under synthetic names. The images are public research data:

- Chest CTs with the radiologists' nodule outlines and a chest X-ray: LIDC-IDRI, via NCI Imaging Data Commons
  ([doi:10.7937/K9/TCIA.2015.LO9QL9SX](https://doi.org/10.7937/K9/TCIA.2015.LO9QL9SX)), CC BY 3.0
- Pathology slides: TCGA-BRCA and TCGA-LUSC via NCI Imaging Data Commons, CC BY 3.0, and TCGA diagnostic slides from
  the NCI Genomic Data Commons, NIH GDC open access (cite the TCGA Research Network)
- AI lymphocyte maps: Stony Brook TCGA TIL maps (Saltz J et al., Cell Reports 2018,
  [doi:10.5281/zenodo.16966285](https://doi.org/10.5281/zenodo.16966285)), CC BY 4.0
- Brain MR slice: Synthea Coherent Data Set, The MITRE Corporation (simulated), CC BY 4.0

Product icons are from the official Microsoft Fabric, Azure and Power Platform icon sets, AWS Architecture Icons,
Google Cloud product icons, GitHub's Octicons and Simple Icons, used as their terms allow in presentations and
architecture diagrams. Every image and icon, with its source and terms, is listed in [`NOTICE.md`](NOTICE.md). All
product names and logos are trademarks of their owners and don't imply endorsement.

## Disclaimer

- This presentation is for education and research only. It shows a demonstration of capability: data architecture
  and user interface on Microsoft Fabric and Project Rayfin. It is not a medical device, has not been reviewed or
  cleared by any regulator, and has not been clinically validated.
- Nothing in it may be used to diagnose, treat, monitor or make any decision about a real patient.
- All data shown is openly available or synthetic. AI outputs in it (lymphocyte maps, nodule outlines, Copilot's
  answers) are illustrative and may be inaccurate.
- The app screens are replicas drawn for the presentation. The email address, workspace ID and app addresses in them
  are stand-ins.
- The presentation's own code and text are released under the [MIT License](LICENSE) (copyright Sanjay Narendran) and
  are provided "as is", without warranty of any kind. The embedded fonts, images and icons keep their own licences
  ([`NOTICE.md`](NOTICE.md)).
- Nothing here is endorsed by the data publishers, the NCI, or Microsoft.
