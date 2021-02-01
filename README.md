# Ontologies
This repo includes the main ontologies used in the [LiLa - Linking Latin](https://lila-erc.eu) project. This includes the main LiLa ontology for lemmas, forms and hypolemmas.

A special class of ontologies for tagset (which use the [OLiA](http://www.acoli.informatik.uni-frankfurt.de/resources/olia/) annotation and linking model) are groupped in a special folder.

## The LiLa ontology

Documentation coming soon. In the menawnile, check the comments and version info of the owl files...

## The Latin extension

As the main OLiA model (`olia.owl`, see next section) was missing a couple of concepts that are useful 
to describe Latin, we created a document called `latin-extension.owl`, which inherits 
the OLiA linking model but introduces a couple of new concepts or relations.

One instance is the `gerundive`.


## LiLa's OLiA-compliant Ontologies

Here is a series of ontologies for the LiLa project which adopt the OLiA linking 
approach and are connected to the main OLiA linking model.

### Structure

In principle, all tagset is described with 2 documents:
* annotation model: connects the tags (instances) to the project-specific concepts
* linking model: connects the project-specific concepts to a unified OLiA model

### URI schema

All the OLiA-compliant ontologies use the following URI schema:

* domain: `http://lila-erc.eu/data`
* type: `doc`
* concept: `vocabulary`
* reference: `document#element`

Thus, the ablative case in the Perseus annotation document is identified as:

```
http://lila-erc.eu/data/doc/vocabulary/perseus-annotation.owl#ablative

```
