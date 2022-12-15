---
layout: page
title: Collecter
subtitle: et référencer des informations précises
orientation: assurer la présence d’informations de qualité sur l’accessibilité des livres numériques
audience: agences bibliographiques, agrégateurs 
previous: ./traiter.html
next: ./diffuser.html
---

<h2 class="color_orange link"> Principes</h2>

Afin de rendre possible l’information de l’utilisateur, les métadonnées collectées sur les ouvrages numériques référencés doivent inclure les informations d’accessibilité. Cela permet aussi d’avoir un chiffrage précis de l’évolution du nombre de titres rendus accessibles. 

Comme ces informations et leur affichage s’inscrit dans un cadre légal, leur exactitude revêt une importance particulière car elle engage les différents acteurs, éditeurs, intermédiaires et revendeurs. Une démarche d’information et de validation devrait être mise en oeuvre pour assurer cette exactitude.

<h3 class="color_orange link"> Les informations nécessaires</h3>

Les exigences de la directive Européenne (lien vers la page la loi) impliquent que des informations sont disponibles sur les modes de lecture (tout le contenu disponible en format texte, mise en forme modifiable, synchronisation texte et audio), sur les possibilitées de navigation dans le fichier (TOC nav; Page Navigation) et sur le non blocage des fonctionnalités d’accessibilité (DRM). 

Une façon simple d’assurer cette information consiste à s’assurer que le document est conforme à EPUB accessibility AA (ONIX * 196 code 03 https://ns.editeur.org/onix/en/* 196/03) 

Si le document est conforme EPUB accessibility A (ONIX * 196 code 02) il devrait aussi assurer qu’il est redistribuable (list code)

Si aucune des conformité n’est atteinte ou déclarée, il faut alors recueillir les informations suivantes : 


* 196 	11 	Navigation dans la table des matières
* 196 	12 	Navigation dans l’index
* 196 	13 	Ordre de lecture
* 196 	14 	Brèves descriptions alternatives
* 196 	15 	Descriptions alternatives complètes
* 196 	16 	Représentations graphiques de données également accessibles comme données non graphiques
* 196 	17 	Contenu mathématique accessible
* 196 	18 	Contenu chimique accessible
* 196 	22 	Balisage de la langue fourni
* 196 	25 	Usage de la couleur
* 196 	26 	Usage du contraste


Les informations 
* 196 	17 Contenu mathématique accessible et 
* 196 18 Contenu chimique accessible 

devraient toujours être recueillies et transportées. Même si elles sont induites par la conformité EPUB Accessibility il est utile de les recueillir car elles ne concernent que certains ouvrages. 
Si des risques existent ils doivent être déclarés

<h3 class="color_orange link"> Les informations supplémentaires utiles</h3>

<h2 class="color_orange link">  Ressources</h2>


[ONIX liste 196](https://ns.editeur.org/onix/fr/196)

[Tableau de correspondances en Français](https://edition-accessible.github.io/signalement/protoype2/references.html)


[Tableau de correspondances en Anglais](https://w3c.github.io/a11y-discov-vocab/crosswalk/)
