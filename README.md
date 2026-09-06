# Target AI

**Target AI is a therapeutic target evidence and risk-auditing platform built with Gradio.**

It resolves a human gene or protein and integrates source-backed evidence across target identity, disease biology, variants, pathways, interaction networks, clinical studies, expression, pharmacology, structural biology, and tractability.

AlphaFold structure visualization and optional on-demand P2Rank pocket prediction provide an additional computational structural-analysis layer.


<img width="1350" height="807" alt="Screenshot 2026-09-04 155724" src="https://github.com/user-attachments/assets/b273ab68-5ff5-43dd-a9f0-ccdeb743b440" />

<p align="center">
  <sub><strong>TargetAI snapshot:</strong> AF2-predicted EGFR structure with P2Rank-identified binding pockets, rendered in 3Dmol.js and ranked by confidence </sub> </p>


## Live Platform
Launch TargetAI → (https://target-ai-nobz.onrender.com) 

The hosted application runs independently in the cloud and can be explored directly from a browser.

Free cloud instances may require a short startup period after prolonged inactivity.



### Hosted deployment note

The public hosted demo does not currently run P2Rank pocket prediction because the free deployment environment does not include the required local Java 17+ and P2Rank runtime.





## Technology

Application

- Python
- Gradio web interface
- Plotly interactive charts
- 3Dmol.js
- Requests HTTP client
- Custom HTML and CSS

Biomedical data integration

- REST and GraphQL APIs
- Structured cross-database identifier resolution
- Concurrent and staged source retrieval
- Source-specific caching, timeouts, and fallback handling

Structural analysis

- Experimental structure retrieval from RCSB PDB
- Predicted structure retrieval from AlphaFold DB
- On-demand P2Rank pocket detection
- Interactive 3Dmol.js structure and pocket visualization
- PDB/CIF coordinate processing
- Local P2Rank execution requiring Java 17+

Deployment and development

- Git and GitHub version control
- Dependency pinning through requirements.txt
- Render-compatible cloud deployment
- Dynamic PORT configuration
- Server binding through 0.0.0.0


<details>
<summary><strong>Data Sources</strong></summary> 

## Data Sources

TargetAI currently integrates evidence from:

- [UniProt](https://www.uniprot.org/) — target identity, protein biology, sequence, annotations and cross-references
- [Open Targets](https://platform.opentargets.org/) — disease associations and tractability evidence
- [ChEMBL](https://www.ebi.ac.uk/chembl/) — drug mechanisms and pharmacology
- [BindingDB](https://www.bindingdb.org/) — experimental compound–target affinity data
- [Reactome](https://reactome.org/) — pathway biology
- [GTEx](https://gtexportal.org/) — normal tissue expression
- [cBioPortal](https://www.cbioportal.org/) — cancer alteration patterns across TCGA PanCancer Atlas cohorts
- [CIViC](https://civicdb.org/) — variant and clinical evidence
- [LitVar2](https://www.ncbi.nlm.nih.gov/research/litvar2/) — variant literature discovery
- [RCSB Protein Data Bank](https://www.rcsb.org/) — experimental protein structures
- [AlphaFold DB](https://alphafold.ebi.ac.uk/) — predicted protein structures
- [STRING](https://string-db.org/) — protein interaction networks
- [ClinicalTrials.gov](https://clinicaltrials.gov/) — clinical study retrieval
- [openFDA](https://open.fda.gov/) — regulatory drug-label annotations


</details> 

## Current Direction

TargetAI is an evolving research-software project.

Currently the platform establishes a foundation for reliable multi-source evidence retrieval and target-centric organization. Ongoing development is focused on an evidence-reconciliation layer for identifying cross-source discrepancies, relationship mismatches, evidence gaps, and uncertainty while preserving source provenance.







## Project

TargetAI was independently conceived and developed end-to-end to address a real therapeutic target-evaluation workflow gap by transforming fragmented biological evidence into a unified computational investigation framework.






## Public Repository Scope
This repository is the public showcase and documentation repository for TargetAI.
The core application source is maintained separately in a private development repository.






## Author

**Anmol Sinha**  
Computational Biology · Disease Biology & Target Analysis · Scientific AI

[LinkedIn](www.linkedin.com/in/anmol-sinha-877324215)

---

*TargetAI is a research and scientific software project. Information presented by the platform should not be interpreted as clinical or medical advice.*

