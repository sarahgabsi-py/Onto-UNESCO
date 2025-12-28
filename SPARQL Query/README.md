# Some Query SPARQL sample
1- List of all UNESCO sites and their names:
SELECT ?Sito ?Nome
WHERE{ ?Sito rdf:type :Sito_UNESCO .
?Sito :ha_nome_sito ?Nome
}

2- List of intangible heritage elements and their corresponding municipalities:
SELECT ?Patrimonio ?Comune
WHERE{ ?Patrimonio rdf:type
:Patrimonio_Culturale_Immateriale .
?Patrimonio :ha_comune ?Comune
}

3- List of UNESCO sites and their recognition dates after the year 2000
SELECT ?Sito ?data
WHERE{
?Sito rdf:type :Sito_UNESCO .
?Sito :data_di_riconoscimento_sito ?data .
FILTER(?data >"2000"^^xsd:gYear)
}

4- Intangible heritage elements present in more than one region (interregional):
SELECT ?Patrimonio
WHERE{
?Patrimonio rdf:type :Patrimonio_Culturale_Immateriale ;
:è_interregionale_immateriale true .
}
