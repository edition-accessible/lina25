---
layout: page
title: Collecter
subtitle: et référencer des informations précises
orientation: assurer la présence d’informations de qualité sur l’accessibilité des livres numériques
audience: agences bibliographiques, agrégateurs
previous: ./traiter.html
next: ./diffuser.html
---

<div markdown="1" id="principes">

{%- include principes.html -%}

Afin de rendre possible l’information de l’utilisateur, les métadonnées collectées sur les ouvrages numériques référencés doivent inclure les informations d’accessibilité. Cela permet aussi d’avoir un chiffrage précis de l’évolution du nombre de titres rendus accessibles.

Comme ces informations et leur affichage s’inscrit dans un cadre légal, leur exactitude revêt une importance particulière car elle engage les différents acteurs, éditeurs, intermédiaires et revendeurs. Une démarche d’information et de validation devrait être mise en oeuvre pour assurer cette exactitude.

Les informations indiquées ici sont exprimées en ONIX. Des tableaux de correspondance permettent de les transposer en UNIMARC et MARC21. 

### Les informations nécessaires

Les [exigences de la directive Européenne](/lina25/pages/loi.html#exigences-relatives-au-livre-numrique) impliquent que des informations sont disponibles sur les modes de lecture (tout le contenu disponible en format texte, mise en forme modifiable, synchronisation texte et audio) ; sur les possibilitées de navigation dans le fichier (Table des matières dans le contenu, pagination de référence d’un imprimé) et sur le non blocage des fonctionnalités d’accessibilité par des mesures de protection inadéquates (DRM).


Une façon simple d’assurer cette information consiste à s’assurer que le document est conforme à EPUB accessibility AA ([liste 196 code 03](https://ns.editeur.org/onix/en/196/03)).

Si le document est conforme EPUB accessibility A ([liste 196 code 02](https://ns.editeur.org/onix/en/196/02)) il devrait aussi assurer que la mise en forme est modifiable (Liste 175 Code E200 : Redimensionnable).

Si aucune des conformité n’est atteinte ou déclarée, il faut alors recueillir les informations suivantes :

-   196 11 Navigation dans la table des matières
-   196 12 Navigation dans l’index
-   196 13 Ordre de lecture
-   196 14 Brèves descriptions alternatives
-   196 15 Descriptions alternatives complètes
-   196 16 Représentations graphiques de données également accessibles comme données non graphiques
-   196 22 Balisage de la langue fourni
-   196 25 Usage de la couleur
-   196 26 Usage du contraste

Si le contenu des ouvrages le justifie, les informations

-   196 17 Contenu mathématique accessible et
-   196 18 Contenu chimique accessible

devraient toujours être recueillies et transportées. Même si elles sont induites par la conformité EPUB Accessibility il est utile de les recueillir car elles ne concernent que certains ouvrages.

Pour la pagination de référence au livre imprimé deux informations sont nécessaires : 

* Liste 196 Code 19 Numérotation de pages équivalente au document imprimé
* Liste 51 Code 13 Publication numérique basée sur (édition papier)



Si des risques existent ils doivent être déclarés. Ces informations sont transportées par les codes suivants : 

* Liste 143 Code 13 : Avertissement : risque de clignotement 	
* Liste 175 Code A310 : Effets sonores 
* Liste 143 Code 17 : Avertissement : risque de simulation de mouvement

### Les informations supplémentaires utiles

Si il est présent, le résumé d'accessibilité (Liste 196 Code 00 : Résumé sur l’accessibilité) devrait être transporté. Ce résumé devrait être le même que celui contenu dans le fichier EPUB (schema.org accessibility summary) et préciser notament les déficiences potentielles.

Les informations relatives à la conformité et à la politique d'accessibilité de l'éditeur contenues dans les codes 196 93 à 99 devraient également être transportées si elles sont présentes.

* 196 	93 	Certification de conformité par
* 196 	94 	Page web pour les informations détaillées d’accessibilité
* 196 	95 	Page web d’un intermédiaire approuvé pour les informations détaillées d’accessibilité
* 196 	96 	Page web de l’éditeur pour les informations détaillées d’accessibilité
* 196 	97 	Compatibilité testée
* 196 	98 	Contact intermédiaire approuvé
* 196 	99 	Contact éditeur pour informations complémentaires sur l’accessibilité

</div>

<aside markdown="1">
<h2> Ressources</h2>

<a href="https://ns.editeur.org/onix/fr/196" class="link color_orange">ONIX liste 196</a>

<a href="https://edition-accessible.github.io/signalement/references/references.html" class="link color_orange">Tableau de correspondances schema.org et ONIX en Français</a>

<a href="https://w3c.github.io/publ-a11y/drafts/a11y-crosswalk-MARC/" class="link color_orange">Tableau de correspondances schema.org, ONIX, MARC21 et UNIMARC en Anglais</a>

<a href="https://w3c.github.io/publ-a11y/drafts/a11y-crosswalk-MARC/" class="link color_orange">Tableau de correspondances schema.org, ONIX, MARC21 et UNIMARC en Anglais</a>

</aside>
