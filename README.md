
# Scantrad

## Objectif du projet

Créer une application [**Electron**](https://electronjs.org/) capable de recevoir des extraits dans une langue et de proposer à l'utilisateur de les lire et/ou de les traduire dans une langue pour permettre à plus de monde de connaître les oeuvres lues.

### Contraintes techniques
|Technologie | Description |
|-|-|
| [**NodeJS**](https://nodejs.org/en/) | Création de l'application |
|[**VueJS**](https://vuejs.org/) | Architecture de l'application |
|[**Electron**](https://electronjs.org/) | Encapsulation de l'application |
|[**Bootstrap**](https://getbootstrap.com/) ou [**Materialize**](https://materializecss.com/) | Style graphique de l'application|

 >**Attention** : Puisque l'on utilisera *NodeJS*, il faudra utiliser des paquets nodes Bootstrap/Materialize, pas les versions présentes sur les sites respectifs.
 >De plus, cloner ce projet basé sur ce [modèle Electron-Vue](https://github.com/SimulatedGREG/electron-vue) permettra de ne pas avoir à configurer *VueJS* et *Electron*.

### Indications

 1. Les oeuvres seront présentées par une image et leur titre sur la page d'accueil, si possible arrangées en grille, comme sur la maquette Accueil.
 > **Astuce :** Cards [*Bootstrap*](https://getbootstrap.com/docs/4.0/components/card/) ou [*Materialize*](https://materializecss.com/cards.html)

 2. Les extraits seront organisés par oeuvre, puis chapitre.
Il sera donc intéressant de garder le cheminement de l'utilisateur, comme visible sur la maquette Lecture.
> **Astuce :** Breadcrumb [*Bootstrap*](https://getbootstrap.com/docs/4.1/components/breadcrumb/) ou [*Materialize*](https://materializecss.com/breadcrumbs.html) pour le visuel.  
>[VueRouter](https://router.vuejs.org/) pour la dynamisation des pages.

 3.  Il faudra pouvoir récupérer et envoyer des données depuis et vers un serveur REST qui fera le relais vers la base de données.
 > **Astuce :** Utilisation de [Axios](https://github.com/axios/axios) pour faciliter les *GET* et *POST* de données.

### Maquettes
![Maquette accueil](https://github.com/Shadovokun/Scantrad/blob/master/MaquetteAccueil.PNG)
![Maquette fiche](https://github.com/Shadovokun/Scantrad/blob/master/MaquetteFiche.PNG)
![Maquette lecture](https://github.com/Shadovokun/Scantrad/blob/master/MaquetteLecture.PNG)
![Maquette traduction](https://github.com/Shadovokun/Scantrad/blob/master/MaquetteTraduction.PNG)
### Etapes pour le développement
Après avoir cloné le projet en local :
``` bash
# Se déplacer dans le dossier
cd Scantrad

# Installer les dépendances
npm install

# Servir le projet sur la machine
npm run dev
```
