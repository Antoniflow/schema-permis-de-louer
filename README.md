# Schéma : communes à permis de louer

Ce schéma décrit un fichier CSV qui recense, commune par commune, les deux régimes du « permis de louer » prévus par le code de la construction et de l'habitation :

- l'**autorisation préalable de mise en location** (articles L. 635-1 et suivants, cerfa n° 15652), demandée avant la signature du bail ;
- la **déclaration de mise en location** (articles L. 634-1 et suivants, cerfa n° 15651), faite dans les 15 jours qui suivent la signature.

## Contexte

Aucune liste nationale officielle n'existe. Chaque commune ou intercommunalité décide de ses zones par une délibération. Quelques collectivités publient leurs périmètres en données ouvertes (Bordeaux Métropole, Métropole européenne de Lille, Métropole Aix-Marseille-Provence, Communauté d'agglomération Plaine Vallée), et certaines DDTM publient une liste départementale (Pas-de-Calais, Hérault), chacune avec ses propres colonnes.

Ce schéma propose des colonnes communes pour que ces listes se rassemblent sans travail de reprise : une ligne par commune, le régime, l'étendue, les secteurs tels que la source les décrit, la date d'entrée en vigueur, et pour chaque ligne la source officielle, son type, sa date et la date à laquelle elle a été lue.

## Principes

- Une ligne par commune, identifiée par son code INSEE (clé primaire).
- Chaque ligne cite une source officielle : délibération, page de la commune, de l'intercommunalité, de l'ADIL ou de l'ANIL, ou page de l'État.
- Une date absente de la source reste vide ; elle n'est jamais calculée.
- Le fichier ne contient aucune donnée personnelle.
- La délibération de la commune ou de l'intercommunalité fait foi ; le fichier ne vaut pas avis juridique.

## Fichiers

- `schema.json` : le schéma au format [Table Schema](https://specs.frictionlessdata.io/table-schema/).
- `exemple-valide.csv` : un extrait valide.

## Jeu de données conforme

[Liste des communes à permis de louer](https://www.data.gouv.fr/datasets/liste-des-communes-a-permis-de-louer-autorisation-prealable-et-declaration-de-mise-en-location), publiée sur data.gouv.fr par Naistor (843 communes au 29 octobre 2026), sous Licence Ouverte 2.0. Le fichier complet est valide pour ce schéma (contrôle Frictionless du 30 octobre 2026).

## Gouvernance

Schéma proposé par Naistor. Les remarques et propositions de modification sont les bienvenues dans les tickets de ce dépôt ou à contact@naistor.fr. Les versions suivent la [gestion sémantique de version](https://semver.org/lang/fr/).

## Licence

Licence Ouverte / Open Licence version 2.0.
