## Comment faire une Pull Request

* Forker le répertoire (dans votre espace GitHub)
* en local, `cd votre/repertoire`
* `git init` votre répertoire github localement
* `git pull` pour mettre à jour localement
* Créée une nouvelle branche (`git checkout -b ma_contribution`)
* Commit les modifications (`git commit -am 'mon message pour le commit'`)
* Push sur la nouvelle branche (`git push origin ma_contribution`)
* RDV au dessus [pull request](https://github.com/LPFP/LPFP.github.io/pulls)
* cliké sur: **New pull request** et laissez vous guider :rocket:

#### Apporter une correction au site.
Pour toute correction a faire qui nous auraient échappés, Github permet de faire des [issues](https://github.com/LPFP/LPFP.github.io/issues) ou de pouvoir inclure vos modifications avec un [merge](https://github.com/LPFP/LPFP.github.io/pulls), si vous avez préalablement "forké" le répertoire.

>éviter s'il vous plait l'envoie de mail pour nous signaler certaines erreurs, passer directement par Github ou par "Slack" --merci.

## Jekyll [petit Fab-Lab de Paris](http://lepetitfablabdeparis.fr/)
inforamtion sur [Jekyll](http://jekyllrb.com/docs/usage/).
information sur [l'installation général](http://jekyllrb.com/docs/installation/)

**installation en local**
* Télécharger l'archive [içi](https://github.com/LPFP/LPFP.github.io/archive/master.zip)

ou en ligne de commande depuis votre dossier:

```bash
git clone https://github.com/LPFP/LPFP.github.io.git
```

*besoin d'aide avec `git` [git - petit guide](http://rogerdudler.github.io/git-guide/index.fr.html)*

* RDV dans le dossier téléchargé ...
* installation de [Ruby RubyGems](http://rubygems.org/pages/download)

```shell
sudo apt-get install ruby-full rubygems
```

```ruby
gem update --system
gem install bundler
```

```shell
#Lancer jekyll et la version du site
cd LPFP.github.io
bundle install
bundle exec jekyll serve
```

>ouvrir votre navigateur à l'adresse `http://127.0.0.1:4000/`

**installation sur un server**

* *Option1* enter un [CNAME](https://help.github.com/articles/using-a-custom-domain-with-github-pages/) depuis le répertoir Github "settings".
* *Option2* Sur un server, envoyer le build `_site` avec [Travis](https://travis-ci.org/) (si pas de module Ruby sur le server).

### Demo
* [sur github](https://lpfp.github.io/)



#### CSS et mise en forme
BootStrap
[Bootstrap CDN](http://getbootstrap.com/getting-started/#download)
Latest compiled and minified CSS
dossier pour les fichiers .CSS `_includes/css.html` et mettre à jours les CDN.
Latest compiled and minified JavaScript
dossier pour le fichier .JS `_includes/js.html` et mettre à jours les CDN.

jQuery
[jQuery CDN](https://code.jquery.com/)
version 3.x minified
dossier pour le fichier .JS `_includes/js.html` et mettre à jours les CDN.

FontAwesome
[Font Awesome CDN](http://fontawesome.io/get-started/)
code par email.
dossier pour le fichier .JS `_includes/js.html`.

Custom Fonts
dossier pour les fichiers .CSS `static/fonts/`.

* [brainflower](http://deathmunkey.deviantart.com/art/Brain-Flower-A-Font-332204280)
* [LatoLatin](http://www.latofonts.com/lato-free-fonts/)
* [mFizz](http://fizzed.com/oss/font-mfizz)

#### Enregister / modifier un atelier/materiel/historique
voir dans le répertoire > fichier.json ci-dessous pour créer une nouvelle entré.

* Les Ateliers sont dans `_data/projects`
* Les évenements historique sont dans `_data/timeline`
* La liste hardware se trouve dans `_data/hardware`

#### Rédiger un poste.
Créée un nouveau fichier dans le répertoire `_posts` avec le format suivant:

> `AAAA-MM-JJ-titre-comme-cela.md`.

les premières lignes sont du `Front Matter en YAML` comme par exemple:

```yaml
---
layout: post
title:  "super poste"
date:   2016-06-21 13:37:00
categories: atelier
---
```
options:
```yaml
img: http://monimages.de/chat.html
disqus: yes
comments: yes
mailing: yes
img: pics.png
```

Le reste du post se rédige avec une synatxe en [Markdown](https://daringfireball.net/projects/markdown/basics).

#### ajouter un éditeur ou modifier les info de l'asso

Pour modifier l'association voir section `asso`.

pour ajouter un éditeur, dé commenter la section ci-dessous et remplir les information dans le fichier `_config.yaml`

```yaml
# nom:  #idem "poster" idem static/img/nom.jpg /!\ photo en .jpg
#   twitter:
#   github:
#   facebook:
#   pgp: "" #public key 64bit
#   lpfp: "" #role au petit fablab
#   quote: ""
```
