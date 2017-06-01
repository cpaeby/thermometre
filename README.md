# Introduction
La gestion de la température est un problème que de nombreuses personnes ou entreprises rencontrent. Le but de ce projet est de faire un thermomètre connecté à un Raspberry Pi qui produit de manière autonome un rapport au format pdf en s'approchant le plus possible des normes GMP de l'industrie pharmaceutique. 

# Outline
Le projet se détache en plusieurs parties. 

## Mesure
La mesure se réalise avec un [senseur](https://www.sparkfun.com/products/245) numérique permettant une précision au degré Celsius entre -55°C et 125°C

## Connection avec le Raspberry Pi
La connection se fait avec le board de [Adafruit](https://learn.adafruit.com/adafruit-pi-cobbler-kit) qui permet une connection simple et légèrement distante du Raspberry Pi. 

## Enregistrement des données
Un scripte en python est écrit pour lire les informations de manière réglulière (1 min - 60 min) et les enregistrer dans un fichier avec les données brutes. 

## Création des graphiques
Les données sont ensuite mise ensemble sous forme de graphique temps-température en utilisant un programme R.

## Gestion des températures hors range
Les valeurs qui sont hors des valeurs autorisées doivent pouvoir être expliquées par l'utilisateur et enregistreées. 

Une annonce des alarmes se fait soit par e-mail, soit par telegram. 

## Création du rapport
Le rapport est écrit de manière automatique en utilisant LaTeX. Un script Python met en forme le document tex et ensuite compile en utilisant TeTeX ou un autre compileur comme PDFLatex. 

## Communication du rapport
L'envoi du rapport se fait soit par e-mail de manière régulière, soit par telegram. 



# Labbook
## Timeline
2017-05-21 Début du projet et recherche d'informations sur R, le programme avec lequel j'ai le moins d'informations et d'expériences pour le moment. J'ai trouvé des informations sur [Coursera](https://www.coursera.org/learn/data-scientists-tools/) qui sont à mon avis des outils que je n'ai pas encore, je suis donc en train de commencer cette formation. 

2017-06-01 Création du projet GitHub pour faire les choses comme il faut :-)

## Mesure
### 2017-05-21 Un tutoriel est disponible par l'université de Cambridge https://www.cl.cam.ac.uk/projects/raspberrypi/tutorials/temperature/

## Connection avec le Raspberry Pi
### 2017-05-21 Un tutoriel est disponible par l'université de Cambridge https://www.cl.cam.ac.uk/projects/raspberrypi/tutorials/temperature/

## Enregistrement des données
### 2017-05-21 Un tutoriel est disponible par l'université de Cambridge https://www.cl.cam.ac.uk/projects/raspberrypi/tutorials/temperature/

## Création des graphiques
### 2017-05-21 Renseignement sur R et comment former un graphique 

## Gestion des températures hors range

## Création du rapport

## Communication du rapport