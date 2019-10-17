# Site pour les JFPC et JIAF

## Génération du site
Pour générer le site, il faut avoir ruby, bundle et jekyll d'installé sur sa machine.

Une fois le dépot git récupéré, il faut la première fois faire
```
bundle install
```
qui va installer les plugins nécessaires pour le site.

Pour générer le site il faut faire
```
bundle exec jekyll serve
```
qui va générer le site (dans le dossier `_site` par défaut) et faire un serveur local afin de pouvoir voir le site à l'adresse [http://localhost:4000](http://localhost:4000).

## Description des fichiers

Il y a certaines pages communes :
  - la page d'accueil `_layout/home.html`,
  - le programme général avec les dates importante `_pages/agenda.md`,
  - les présidences des différents comités `_pages/comites.md`,
  - les informations et tarifs pour les inscirptions `_pages/inscription.md`,
  - les sponsors `_pages/sponsors.md`,
  - des informations sur la ville de Nice `_pages/venue.md`.

Pour chacune des conférences, il y a :
  - la page d'accueil `_pages/jfpc` ou `_pages/jiaf`,
  - le programme détaillé `_pages/programme_jfpc.md` ou `_pages/programme_jiaf.md`,
  - les comités `_pages/comites_jfpc.md` ou `_pages/comites_jiaf.md`,
  - les éditions précédentes `_pages/editions_jfpc.md` ou `_pages/editions_jiaf.md`,
  - les informations pour la soumission d'article `_pages/soumission_jfpc.md` ou `_pages/soumission_jiaf.md`.

Certaines de ces pages ou parties de page sont générées automatiquement à partir de fichiers de données.
Les fichiers de données se trouvent dans le dossier `_data`.
  - `comites_jfpc.yml` et `comites_jiaf.yml` contient les membres de chacun des comités ;
  - `dates_jfpc.yml` et `dates_jiaf.yml` contient les dates importantes ;
  - `editions_jfpc.yml` et `editions_jiaf.yml` contient des liens vers les précédentes éditions ;
  - `navigation.yml`, `navigation_jfpc.yml` et `navigation_jiaf.yml` contient les éléments que l'on ;souhaite voir apparaître dans la barre de navigation pour respectivement, les pages communes, les pages pour les JFPC et les pages pour les JIAF ;
  - `programme_jfpc.yml` et `programme_jiaf.yml` contient le programme détaillé ;
  - `sitemap.yml` contient les éléments de la catégorie _plus d'infos_ de la page d'accueil ;
  - `speakers.yml` contient des informations sur les conférenciers invités qui figureront sur la page d'accueil ;
  - `sponsors.yml` contient des informations sur les sponsors.


| Page                        | Générée totalement ou en partie à partir de                     |
|-----------------------------|-----------------------------------------------------------------|
| `_layout/home.md`           | `_data/sitemap.yml`, `_data/speakers.yml`, `_data/sponsors.yml` |
| `_pages/agenda.md`          | `_data/dates_jfpc.yml`, `_data/dates_jiaf.yml`                  |
| `_pages/comites.md`         | `_data/comites_jfpc.yml`, `_data/comites_jiaf.yml`              |
| `_pages/sponsors.md`        | `_data/sponsors.yml`                                            |
| `_pages/programme_jfpc.md`  | `_data/programme_jfpc.yml`                                      |
| `_pages/programme_jiaf.md`  | `_data/programme_jiaf.yml`                                      |
| `_pages/comites_jfpc.md`    | `_data/comites_jfpc.yml`                                        |
| `_pages/comites_jiaf.md`    | `_data/comites_jiaf.yml`                                        |
| `_pages/editions_jfpc.md`   | `_data/editions_jfpc.yml`                                      |
| `_pages/editions_jiaf.md`   | `_data/editions_jiaf.yml`                                      |
| `_pages/soumission_jfpc.md` | `_data/dates_jfpc.yml`                                      |
| `_pages/soumission_jiaf.md` | `_data/dates_jiaf.yml`                                      |