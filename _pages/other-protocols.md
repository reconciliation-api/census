---
layout: single
title: Other protocols
permalink: /other-protocols/
---

This page lists protocols, formats or other specifications that are
similar to OpenRefine's reconciliation API.

## NIF web services

The [NLP Interchange Format](https://persistence.uni-leipzig.org/nlp2rdf/) (NIF)
is an RDF-based format to annotate natural language text. It can be used
to [represent the output of an entity linking system](https://github.com/dice-group/gerbil/wiki/NIF) (which spots mentions of entities
in text). This format is used by [GERBIL](http://gerbil.aksw.org/gerbil/) to benchmark
entity linking heuristics.

Entity linking (spotting mentions of entities in text) and entity matching (linking database entries which refer to the same entity) are different tasks, but they have some similarities.

## OpenSearch

[OpenSearch](http://www.opensearch.org/Home) is a protocol that can be used
by search engines to expose their results in a uniform way, to be consumed
by client applications such as web browsers.

Given that reconciliation is very often search-based, it might make sense to
take some inspiration from this protocol.

## HOBBIT and SEALS

The [HOBBIT platform](https://hobbit-project.github.io/index.html) has been developed
to benchmark entity matching systems in a uniform and principled way.
Matchers need to conform to [a Java API](https://hobbit-project.github.io/system_integration.html) to be evaluated. This system is used in the [Ontology Alignment Evaluation Initiative](http://oaei.ontologymatching.org/), an academic workshop run in
conjunction with the [International Semantic Web Conference](http://www.semanticweb.org/).

Similarly, there seems to be a [SEALS platform](https://github.com/DanFaria/OAEI_SealsClient), not documented as extensively, which might do the same thing. Its use is described [on the corresponding OAEI 2019
page](http://oaei.ontologymatching.org/2019/seals/index.html).

## SemTab

[SemTab](https://www.cs.ox.ac.uk/isg/challenges/sem-tab) stands for annual Semantic Web Challenge on Tabular Data to Knowledge Graph Matching collocated with the [International Semantic Web Conference](http://www.semanticweb.org). The systems for semantic table interpretation are benchmarked using [SemTab evaluators](https://github.com/sem-tab-challenge/aicrowd-evaluator). The specifications for each task in SemTab are documented at [AIcrowd](https://www.aicrowd.com/organizers/tabular-data-to-knowledge-graph-matching).

## Questioning Authority

[Questioning Authority](https://github.com/samvera/questioning_authority) is a web service that wraps various authority databases into one unified API that can be used to search for records by text, similarly to the reconciliation API. It is used in the library communities.

## Common Terminology Services 2

The [Common Terminology Service 2](https://www.omg.org/cts2/) specification defines an interface to a vocabulary system in the medical domain. The [D2Refine](https://github.com/caCDE-QA/D2Refine) project exposes such systems as reconciliation services in OpenRefine, which seems to suggest that they might have similarities with the reconciliation protocol we develop in this group. It should therefore be investigated.
