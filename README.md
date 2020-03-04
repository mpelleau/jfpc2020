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
bundle exec jekyll serve --config _config.yml,_config_dev.yml
```
qui va générer le site (dans le dossier `_site` par défaut) et faire un serveur local afin de pouvoir voir le site à l'adresse [http://localhost:4000](http://localhost:4000).

## Types de pages

Il y a 4 types de pages possibles et se trouvent dans le dossier `_layout/` :
  - pour les pages d'accueil `_layout/home.html`
  - pour les pages " normales " `_layout/page.html`
  - pour les pages avec une image en entête `_layout/page-image.html`
  - pour les pages vides sans barre de navigation `_layout/page-empty.html`

## Description des fichiers

Il y a certaines pages communes :
  - la page d'accueil `index.html`,
  - le programme général avec les dates importantes `_pages/agenda.md`,
  - les présidences des différents comités `_pages/comites.md`,
  - les informations et tarifs pour les inscirptions `_pages/inscription.md`,
  - les sponsors `_pages/sponsors.md`,
  - des informations `_pages/about.md`, 
  - des informations sur la ville de Nice `_pages/venue.md`,
  - comment venir à Nice `_pages/travel.md`,
  - et quelques adresses à Nice `_pages/booklet.md`.

Pour chacune des conférences, il y a :
  - la page d'accueil `_pages/jfpc.md` ou `_pages/jiaf.md`,
  - un page "à propos" `_pages/about_jfpc.md` ou `_pages/about_jiaf.md`,
  - le programme détaillé `_pages/programme_jfpc.md` ou `_pages/programme_jiaf.md`,
  - les comités `_pages/comites_jfpc.md` ou `_pages/comites_jiaf.md`,
  - les éditions précédentes `_pages/editions_jfpc.md` ou `_pages/editions_jiaf.md`,
  - les informations pour la soumission d'article `_pages/soumission_jfpc.md` ou `_pages/soumission_jiaf.md`.

Certaines de ces pages ou parties de page sont générées automatiquement à partir de fichiers de données.
Les fichiers de données se trouvent dans le dossier `_data`.
  - `comites_jfpc.yml` et `comites_jiaf.yml` contiennent les membres de chacun des comités ;
  - `dates_jfpc.yml` et `dates_jiaf.yml` contiennent les dates importantes ;
  - `editions_jfpc.yml` et `editions_jiaf.yml` contiennent des liens vers les précédentes éditions ;
  - `navigation_home.yml`, `navigation.yml` et `navigation_conf.yml` contiennent les éléments que l'on souhaite voir apparaître dans la barre de navigation pour respectivement, la page d'accueil commune, les pages communes, les pages pour les conferences ;
  - `programme_jfpc.yml` et `programme_jiaf.yml` contiennent les programme détaillés ;
  - `sitemap.yml`, `sitemap_jfpc.yml` et `sitemap_jiaf.yml` contiennent les éléments de la catégorie _plus d'infos_ de la page d'accueil commune, de JFPC et JIAF ;
  - `speakers.yml` contient des informations sur les conférenciers invités qui figureront sur la page d'accueil ;
  - `sponsors.yml` contient des informations sur les sponsors.


| Page                        | Générée totalement ou en partie à partir de                          |
|-----------------------------|----------------------------------------------------------------------|
| `_layout/home.md`           | `_data/sitemap.yml`, `_data/speakers.yml`, `_data/sponsors.yml`      |
| `_pages/agenda.md`          | `_data/dates_jfpc.yml`, `_data/dates_jiaf.yml`                       |
| `_pages/comites.md`         | `_data/comites_jfpc.yml`, `_data/comites_jiaf.yml`                   |
| `_pages/sponsors.md`        | `_data/sponsors.yml`                                                 |
| `_pages/jfpc.md`            | `_data/sitemap_jfpc.yml`, `_data/speakers.yml`, `_data/sponsors.yml` |
| `_pages/jiaf.md`            | `_data/sitemap_jiaf.yml`, `_data/speakers.yml`, `_data/sponsors.yml` |
| `_pages/programme_jfpc.md`  | `_data/programme_jfpc.yml`                                           |
| `_pages/programme_jiaf.md`  | `_data/programme_jiaf.yml`                                           |
| `_pages/comites_jfpc.md`    | `_data/comites_jfpc.yml`                                             |
| `_pages/comites_jiaf.md`    | `_data/comites_jiaf.yml`                                             |
| `_pages/editions_jfpc.md`   | `_data/editions_jfpc.yml`                                            |
| `_pages/editions_jiaf.md`   | `_data/editions_jiaf.yml`                                            |
| `_pages/soumission_jfpc.md` | `_data/dates_jfpc.yml`                                               |
| `_pages/soumission_jiaf.md` | `_data/dates_jiaf.yml`                                               |
