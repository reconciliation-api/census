---
layout: single
title: Services
permalink: /services/
---

This page lists available reconciliation services.

## Servers

Beyond publicly available hosted services, some software exposes reconciliation endpoints locally.

### csv-reconcile

[csv-reconcile](https://pypi.org/project/csv-reconcile/) is a Python based project can be used to run a reconciliation service off any CSV file.
It supports version 0.2 of the protocol.

### reconcile-csv

[reconcile-csv](https://okfnlabs.org/projects/reconcile-csv/) is a Clojure based project can be used to run a reconciliation service off any CSV file.
It supports version 0.1 of the protocol.

### OpenRefine's RDF extension

The [RDF extension](https://github.com/stkenny/grefine-rdf-extension) can be used to wrap a SPARQL endpoint into a reconciliation service.
It supports version 0.1 of the protocol.

### datasette-reconcile

[datasette-reconcile](https://github.com/drkane/datasette-reconcile) is a plugin for [Datasette](https://docs.datasette.io/en/stable/) to expose a reconciliation endpoint from a table stored in a Datasette instance.
It supports version 0.2 of the protocol.

### Discogs reconciliation
[discogsreconciliation](https://github.com/judaicadh/discogsreconciliation) is a Python based self-hosted reconciliation service for the [Discogs](https://www.discogs.com/developers/) music catalog API.

## Hosted services

A list of hosted services is maintained on Wikidata and can be viewed
in our [reconciliation test bench](https://reconciliation-api.github.io/testbench/).

Other reconciliation services (including discontinued services) can be found on [OpenRefine's wiki](https://github.com/OpenRefine/OpenRefine/wiki/Reconcilable-Data-Sources).

### How to add a service to the test bench

*Requirements:* Make sure your service is publicly accessible - local endpoints (such as those with `localhost` or `127.0.0.1` in their address) should not be added.

If your service fulfills these requirements, let us know about it by opening an [issue](https://github.com/reconciliation-api/census/issues) or add the necessary information to Wikidata by yourself like in [this example](https://www.wikidata.org/wiki/Q922063#P6269).

*Steps:*
1. Find out if there is already a Wikidata item about your service, your database or your identifier. You can use [Wikidata's search interface](https://www.wikidata.org/wiki/Special:Search?ns0=1) for that. If there is not, you can [create a new one](https://www.wikidata.org/wiki/Special:NewItem).
1. Add a statement on that item, using the [API endpoint (P6269)](https://www.wikidata.org/wiki/Property:P6269) property, adding the [OpenRefine reconciliation service API (Q64490175)](https://www.wikidata.org/wiki/Q64490175) as [protocol (P2700)](https://www.wikidata.org/wiki/Property:P2700) in a qualifier.
1. Optionally add a link to the documentation for the endpoint by adding a [described at URL (P973)](https://www.wikidata.org/wiki/Property:P973) or [user manual link (P2078)](https://www.wikidata.org/wiki/Property:P2078) qualifier.
1. Optionally add a link to the source code for the endpoint by adding a [source code repository (P1324)](https://www.wikidata.org/wiki/Property:P1324) qualifier.

