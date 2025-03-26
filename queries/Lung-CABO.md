# SPARQL queries for Lung-CABO-KG competency questions

Here we include the 13 SPARQL queries for each of the competency questions designed to validate EBOCA-KG, SEM-DISNET module.


## Lung-CABO1
 Can we identify patterns of gene fusions that are shared across different types of pathologies?
 ```Sparql
PREFIX obo:<http://purl.obolibrary.org/obo/>

SELECT ?definition
WHERE {obo:SO_0001060 obo:IAO_0000115 ?definition}
 ```

## Lung-CABO2
What level of confidence is there in the genes described in lung cancer?
```Sparql
PREFIX ncit:<http://ncicb.nci.nih.gov/xml/owl/EVS/Thesaurus.owl#>
PREFIX owl:<http://www.w3.org/2002/07/owl#>
PREFIX rdfs:<http://www.w3.org/2000/01/rdf-schema#>

SELECT ?encode_relationship
WHERE {?encode_relationship a owl:ObjectProperty ;
                              rdfs:domain ncit:C16612 ;
                              rdfs:range ncit:C17021
      }
```
## Lung-CABO3
Can we determine the chromosomal positions of the gene variants described in lung cancer?

## Lung-CABO4
Of the genes involved in Non-small cell lung cancer and small cell lung cancer, what pathways do they share?
## Lung-CABO5
Which object property defines the relationship between a variant and a disease?

## Lung-CABO6
Which semantic type is used to classify a disease in Lung-CABO throught the asociated genes?

## Lung-CABO7
How many pathways are associated with a specific lung cancer subtype?

## Lung-CABO8
What is the parent class and external alignment of a given disease in Lung-CABO?

## Lung-CABO9
Which genes do not have an associated PSI?

## Lung-CABO10
Can a given gene be associated with more than two variant?

## Lung-CABO11
Are fusion genes represented with their partner genes?

## Lung-CABO12
Are genomic variants annotated with their chromosomal position and alleles?

## Lung-CABO13
What is the score or evidence index associated with a gene-disease association?

