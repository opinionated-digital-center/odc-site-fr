---
permalink: /about/
title: "A propos de l'Opinionated Digital Center"
toc: true
---
## Notre objectif

L'objectif de l'Opinionated Digital Center est de partager des ressources directement utilisables -- sous forme de templates, outils et connaissance organisée -- , qui reflètent de fortes opinions sur ce qui nous pensons va aider développeurs, équipes et organisations à être plus efficients dans le contexte des centres de développement numériques.

Ces ressources sont créées -- et utilisées quotidiennement -- par des développeurs, coachs et managers expérimentés, qui se sont lassés de réinventer la roue à chaque lancement de projet, organisation de centre numérique, livraison de développement en production, organisation du partage de la connaissance.

Nous voulons permettre aux développeurs d'augmenter leur capacité à créer, à innover et à livrer de la valeur, en apportant suffisamment de structure pour les soutenir et les guider dans leur travail, sans toutefois sur-structurer et sur-procédurer, ce qui causerait leur aliénation (maintes fois observée).

## Caractéristiques des ressources que nous proposons

Les ressources elles-mêmes sont principalement en anglais (la langue du développement), mais les éléments pertinents à la traduction seront traduits, en fonctions des besoins exprimés (et argumentés 😆 ).

En application de notre [ADR-0008](https://github.com/opinionated-digital-center/architecture-decision-records/blob/master/docs/adr/0008-use-github-as-main-hub-for-the-opinionated-digital-center.md), tous nos projets sont hébergés sur notre [compte GitHub](https://github.com/opinionated-digital-center) (même notre travail -- conséquent en proportion -- relatif à GitLab...).

Les ressources que nous partageons sont :

### Expliquées

* Le raisonnement et l'argumentation derrière nos choix sont écrits, principalement sous la forme d'Architecture Decision Records (voir [ADR-0000](https://github.com/opinionated-digital-center/architecture-decision-records/blob/master/docs/adr/0000-record-architecture-decisions.md) et [ADR-0001](https://github.com/opinionated-digital-center/architecture-decision-records/blob/master/docs/adr/0001-use-markdown-architectural-decision-records.md)).

### Documentées

* Nos ressources sont présentées avec une documentation la plus utile et complète possible, sous formes variées (documentation classique, tests humainement lisibles et compréhensibles écrits en [Gherkin](https://cucumber.io/docs/gherkin/reference/), pour ne donner que deux exemples).
* Des références sont mentionnées où que possible et utile (voir [cet ADR](https://github.com/opinionated-digital-center/architecture-decision-records/blob/master/docs/adr/0001-use-markdown-architectural-decision-records.md) par exemple).

### Testées et écrites avec la qualité en tête

* Aucun code n'est livré sans une [suite complète de tests](https://github.com/opinionated-digital-center/python-library-project-generator/blob/master/README.rst#fully-tested-features).
* Nous tachons de rester aussi proche que possible des principes et pratiques du [Software Crafsmanship](https://manifesto.softwarecraftsmanship.org/).

### Aussi simple que possible à mettre en place

* Nous tâchons de mettre à disposition aussi souvent que possible des outils d'automatisation d'installation, couplés avec une documentation détaillée.

## Fondateurs

{% for item in site.data.authors %}
{% if item[1].type == "founder" %}
{% assign author = item[1] %}
{% include author-details.html %}
{% endif %}
{% endfor %}

## Contributeurs distingués

{% for item in site.data.authors %}
{% if item[1].type != "founder" %}
{% assign author = item[1] %}
{% include author-details.html %}
{% endif %}
{% endfor %}
