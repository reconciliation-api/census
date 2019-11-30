---
layout: single
title: Services
permalink: /services/
---

This page lists available reconciliation services.

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

## Servers

Beyond publicly available hosted services, some software exposes reconciliation endpoints locally.

### reconcile-csv

[reconcile-csv](http://okfnlabs.org/reconcile-csv/) can be used to run a reconciliation service off any CSV file.

### OpenRefine's RDF extension

The [RDF extension](https://github.com/stkenny/grefine-rdf-extension) can be used to wrap a SPARQL endpoint into a reconciliation service.

### Open Reconcile

[Open Reconcile](https://github.com/OpenRefine/open-reconcile) is a project that can be used to run a reconciliation service on top of a SQL database.
