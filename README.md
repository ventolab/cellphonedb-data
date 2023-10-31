# CellphoneDB database 

CellphoneDB database (aka cellphonedb-data) is a **manually curated** repository of receptors, ligands and their interactions. 

The database can be used to search for a particular ligand/receptor or, in combination with the [CellphoneDB tool](https://github.com/ventolab/cellphonedb),
to interrogate your own single-cell transcriptomics data.

For more information, visit https://www.cellphonedb.org/ or [our extended documentation](https://github.com/ventolab/CellphoneDB/blob/master/docs/RESULTS-DOCUMENTATION.md#database-of-interactions)

For CellphoneDB tool, visit https://github.com/ventolab/cellphonedb


## Key features of CellphoneDB
- Subunit architecture is included for both ligands and receptors, representing **heteromeric complexes** accurately. 
This is crucial, as cell-cell communication relies on multi-subunit protein complexes that go beyond the binary representation used in most databases and studies. 

- Includes interactions involving **non-proteins** (i.e., molecules not encoded by a gene/trasncript) acting as ligands. Examples of these include steroid hormones (e.g., estrogen), small molecules (e.g. histamine) or neurotransmitters. To do so, we have reconstructed the biosynthetic pathways and used the last representative enzyme as a proxy of ligand abundance. We retrieve this information by manually reviewing and curating relevant literature and peer-reviewed pathway resources such as REACTOME. Cellphonedb-data includes more than 200 interactions involving non-peptidic ligands! All non-protein ligands are coded as complexes in CellphoneDB. This is to allow the inclusion of all the key enzymes in their biosynthetic pathway (even if the number of enzymes n=1).


# Release notes

### cellphonedb-data v5.0.0
1) New database (v5.0.0) with more manually curated interactions, making up to a total of 2,912 interactions.
2) Includes a new module (CellSign) containing Receptor-to-TF relationships retrieved by manual revision of the literature and are restricted to transcription factors with high specificity for an upstream receptor. CellSign database contains a total of 211 highly-specific direct receptor-to-TF relationships. CellSign uses TF activation as a downstream sensor for receptor activation upon cell-cell interaction, thus adding an extra layer of evidence to the likelihood of the cell-cell interaction.
3) New annotations of interactions as a result of manual curation, including: interactors, classification, directionality and modulatory effect.

### cellphonedb-data v4.1.0
1) New database (v4.1.0) with more manually curated interactions, making up to a total of 2,923 interactions.
2) Non-curated exernal databases are discarded.

### cellphonedb-data v4.0.0
1) More manually curated interactions added, with special focus on protein acting as heteromeric complexes. This version fo the database includes almost 2,000 high-confidence interactions, including heteromeric complexes! We believe modelling complexes is key to minimise false positives in the predictions.
2) Includes interactions involving non-proteins (i.e., not encoded by a gene) acting as ligands. 

### cellphonedb-data v3.0.0
1) Updated interactions involving WNT pathway.
