# Repositories

During my PhD, I aimed to study reuse in bioinformatics workflows, specifically in the next generation systems Nextflow and Snakemake. Here is an overview of the main repositories linked to that project.

## Intro

My aim was to understand how workflows are actually used by the bioinforlatics community, and also to understand reuse practices.

## Collecting and transforming the data

In order to study reuse practices, I had to collect workflows.
I chose to do so on public GitHub repositories in order to get a large amount of them.

A crucial information in order to compare workflows is the workflows' functions, or the bioinformatics operations that the workflows are performing.
As this information was not readily available, I had to analyze the workflows' code to extract the bioinformatics tools. For further information, I used other databases to enrich this database. In particular, the [bio.tools](https://bio.tools/) was used to get semantic annotations of bioinformatics tools in the [EDAM](https://edamontology.org/EDAM.owl) ontology. 


(image outil wf to bt + légende + citation)
Workflow extraction and annotation process. It is composed of three major units : i) CrawlWF retrieves and extracts GitHub workflows, ii) ParsWF analyses the workflows to extract significant information, and iii) WF2BT retrieves the bio.tools annotations linked to the workflows' tools.

This process was first elaborated and implemented for Snakemake workflows in 
[this repository](https://github.com/mdjaffardjy/Snakemake_workflow_analysis).

During interships that I supervized, it was adaptated on Nextflow workflows, and the resulting tool can be found in [this repository](https://github.com/mdjaffardjy/AnalyseDonneesNextflow).

The output of those tools were annotated workflows, and this information was later stored in a relational database as well as a knowledge graph (a semantic web representation of the data). Those representations aimed to be universal to workflows written in all languages.

## Analyzing the data

After collectif the workflows, I conducted investigations on the reuse in the Nextflow and Snakemake systems. 
This investigation was conducted at several levels (reuse of steps, reuse of code, reuse of tools) by proposing similarity metrics and applying them to the corpus.
The results can be found in [this repository](https://github.com/mdjaffardjy/Reuse_in_processes).

During an internship I co-supervized, a similarity study on the 




TODO :
- link to paper
- link to thesis
- add images

