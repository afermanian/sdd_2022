# UE 21.2 EC Science des données
Cours « science des données » à Mines ParisTech (2021–2022). [![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by-sa/4.0/)

__Organisation de ce repo__
* `environment.yml` permet de charger l'environnement conda pour les notebooks via l'interface graphique d'Anaconda ou 
```bash
   conda env create -f environment.yml -n sdd2021
   conda activate sdd2021
```
Notez que cet environnement vous fait utiliser JupyterLab et non pas Jupyter Notebook. JupyterLab est plus moderne et plus agréable d'utilisation (voir [la documentation](https://jupyterlab.readthedocs.io/en/stable/)). En particulier, JupyterLab permet de copier des cellules entre notebooks, et l'[extension "Table of contents"](https://github.com/jupyterlab/jupyterlab-toc/blob/master/toc.gif) qui facilite la navigation dans un notebook y est native.
* `poly/` contient tous les fichiers permettant de compiler le poly. La dernière version compilée à jour s'intitule `sdd_2021_poly.pdf`
* `pc/` contient un répertoire par PC
* `projet/` contient les données et instructions relatives au projet numérique.

__Équipe pédagogique__
* Responsables de cours : Bruno Figliuzzi et Adeline Fermanian
* Chargé·e·s d'enseignement : 

__Emploi du temps__
* __lundi 30/05 :__ 
  * __13h45-15h15 :__ cours 1 — Introduction et statistique descriptive (Chapitres 1 & 2)
  * __15h30-17h00 :__ cours 2 — Estimation et propriétés d'un estimateur (Chapitre 3, sections 3.1 à 3.4)

* __vendredi 3/06 :__
  * __9h00-10h30 :__ cours 3 — Techniques d'estimation (Chapitre 3, sections 3.5 & 3.6)
  * __10h45-12h15 :__ PC 1 — Statistique inférentielle (TD)

* __vendredi 10/06 :__
  * __9h00-10h30 :__ cours 4 Réduction de dimension (Chapitre 5)
  * __10h35-12h15 :__ PC 2 — Réduction de dimension (TP)

* __jeudi 10/06 :__
  * __13h45-15h15 :__ cours 5 — Tests statistiques (Chapitre 4)
  * __15h30-17h00 :__ cours 6 — Bonnes pratiques (Chapitre 6)

* __vendredi 17/06 :__ 
  * __9h00-10h30 :__ cours 7 - Introduction à l'apprentissage supervisé (Chapitre 7)
  * __10h45-12h15 :__ PC 3 — Pré-traitement & introduction à scikit-learn pour l'apprentissage supervisé

* __lundi 20/06 :__
  * __13h45-15h15 :__ cours 8 — Régularisation (Chapitre 8)
  * __15h30-17h00 :__ PC 4 — Sélection de modèles (TP)

* __vendredi 24/06 :__ 
  * __9h00-10h30 :__ cours 9 — Modèles d'apprentissage supervisé non-linéaires (Chapitre 9)
  * __15h30-17h00 :__ PC 5 — Modèles linéaires pour la classification (TD)

* __vendredi 1/07 :__
  * __9h00-12h15 :__  cours 10 — Modèles d'apprentissage supervisé non-linéaires et applications pratiques

__Pour contribuer à ce repo__
Ce repo contient un script `pre-commit.sh` qui permet de le nettoyer (supprimer les fichiers auxiliaires de latex, nettoyer les notebooks avec [`nbstripout`](https://pypi.org/project/nbstripout/)).

Il est possible de lancer automatiquement ce script lors d'un `git commit` grâce à un [`hook`](https://githooks.com/). Pour cela, il suffit de le copier dans le fichier `.git/hooks/pre-commit` ou d'utiliser un lien symbolique (pour conserver le contrôle de version) :
```bash
    cd .git/hooks/
    ln -s ../../pre-commit.sh pre-commit
```
