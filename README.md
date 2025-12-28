# 🏛️ ONTO-UNESCO: Ontology for Representing UNESCO World Heritage in Italy Semantic Web • OWL • SWRL • SPARQL
OntoUNESCO is an ontology developed in Protégé to formally represent, structure, and query information about Italian UNESCO World Heritage Sites and Intangible Cultural Heritage elements.
The project aims to provide a semantic, interoperable model that supports reasoning, data integration, and advanced SPARQL queries. This work was developed as part of the Ontology and Semantic Web course project.

# 🧩 Ontology Overview
The ontology includes:
✔ Classes
  - UNESCO Site
  - Intangible Cultural Heritage
  - UNESCO Criteria (material & intangible)
  - Geographic Location (Region, Province, Municipality)
  - Historical Periods (Prehistory, Middle Ages, Renaissance, etc.)
  - Typologies of sites and intangible heritage

✔ Object Properties
  - ha_criterio_UNESCO_materiale
  - ha_criterio_UNESCO_immateriale
  - ha_localizzazione_sito_UNESCO
  - ha_periodo_storico_sito_UNESCO
  - ha_tipologia_patrimonio_immateriale
  - Inverse properties for bidirectional reasoning

✔ Data Properties
  - Recognition dates
  - Names
  - Boolean values (e.g., interregional, universal value)
  - Historical period start/end

✔ Individuals
456 individuals representing:
  - UNESCO sites
  - Intangible heritage elements
  - Regions, provinces, municipalities
  - Historical periods

# 🧠 SWRL Rules Implemented
The ontology includes four SWRL rules to enhance reasoning:
- Identify interregional intangible heritage
- Identify interregional UNESCO sites
- Assign universal value to material sites with at least one criterion
- Assign universal value to intangible heritage with at least one criterion
These rules automate semantic inference and reduce manual annotation.

# 📊 Ontology Metrics (Protégé)
- Axioms: 3,535
- Logical axioms: 2,961
- Classes: 20
- Object properties: 33
- Data properties: 13
- Individuals: 456
- Object property assertions: 2,032
- Data property assertions: 293
These metrics reflect a rich, expressive ontology suitable for reasoning and semantic querying.

# 🏗️ Technologies Used
- Protégé 5.x — ontology modeling
- OWL 2 — Web Ontology Language
- SWRL — inference rules
- SPARQL 1.1 — semantic queries
- RDF/XML — ontology serialization format

