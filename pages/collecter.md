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

Les recommandations françaises sur l'affichage des informations d'accessibilité peut-être utile pour comprendre le sens de chaque code.
### Les informations nécessaires

Les [exigences de la directive Européenne](/lina25/pages/loi.html#exigences-relatives-au-livre-numrique) impliquent que des informations sont disponibles sur les modes de lecture (tout le contenu disponible en format texte, mise en forme modifiable, synchronisation texte et audio) ; sur les possibilitées de navigation dans le fichier (Table des matières dans le contenu, pagination de référence d’un imprimé) et sur le non blocage des fonctionnalités d’accessibilité par des mesures de protection inadéquates (DRM).

Il faut pour cela recueillir les informations suivantes :

-   [196 11 Navigation dans la table des matières](https://ns.editeur.org/onix/en/196/11)
-   [196 12 Navigation dans l’index](https://ns.editeur.org/onix/en/196/12)
-   [196 13 Ordre de lecture](https://ns.editeur.org/onix/en/196/13)
-   [196 14 Brèves descriptions alternatives](https://ns.editeur.org/onix/en/196/14)
-   [196 15 Descriptions alternatives complètes](https://ns.editeur.org/onix/en/196/15)
-   [196 16 Représentations graphiques de données également accessibles comme données non graphiques](https://ns.editeur.org/onix/en/196/16)
-   [196 22 Balisage de la langue fourni](https://ns.editeur.org/onix/en/196/22)
-   [196 25 Usage de la couleur](https://ns.editeur.org/onix/en/196/25)
-   [196 26 Usage du contraste](https://ns.editeur.org/onix/en/196/26)

Si le contenu des ouvrages le justifie, les informations suivantes sont également nécessaires : 

-   [196 17 Contenu mathématique accessible](https://ns.editeur.org/onix/en/196/17) et
-   [196 18 Contenu chimique accessible](https://ns.editeur.org/onix/en/196/18)

Pour la pagination de référence au livre imprimé deux informations sont nécessaires : 

* [Liste 196 Code 19 Numérotation de pages équivalente au document imprimé](https://ns.editeur.org/onix/en/196/19)
* [Liste 51 Code 13 Publication numérique basée sur (édition papier)](https://ns.editeur.org/onix/en/51/13)

Si des risques existent ils doivent être déclarés. Ces informations sont transportées par les codes suivants : 

* [Liste 143 Code 13 : Avertissement : risque de clignotement](https://ns.editeur.org/onix/en/143/13)
* [Liste 143 Code 15 : Effets sonores](https://ns.editeur.org/onix/en/143/15)
* [Liste 143 Code 17 : Avertissement : risque de simulation de mouvement](https://ns.editeur.org/onix/en/143/17)

Même si ils n'ont pas vocation à être affichés, les codes déclarant une absence de risque permettent de s'assurer que l'absence de ces trois codes n'est pas due à un manque de vigilance : 

* [Liste 143 Code 14 : Aucun avertissement nécessaire pour les risques liés à un clignotement](https://ns.editeur.org/onix/en/143/13)
* [Liste 143 Code 16 : Aucun avertissement nécessaire pour les risques liés à un niveau sonore](https://ns.editeur.org/onix/en/143/15)
* [Liste 143 Code 18 : Aucun avertissement nécessaire pour les risques liés à des simulations de mouvement](https://ns.editeur.org/onix/en/143/17)


### Les informations supplémentaires utiles

Une façon simple d’assurer cette information consiste à s’assurer que le document est conforme à EPUB accessibility AA ([liste 196 code 03](https://ns.editeur.org/onix/en/196/03)). 

Si le document est conforme EPUB accessibility A ([liste 196 code 02](https://ns.editeur.org/onix/en/196/02)) il devrait aussi assurer que la mise en forme est modifiable (Liste 175 Code E200 : Redimensionnable).

Si il est présent, le résumé d'accessibilité ([Liste 196 Code 00 : Résumé sur l’accessibilité](https://ns.editeur.org/onix/en/196/00)) devrait être transporté. Ce résumé devrait être le même que celui contenu dans le fichier EPUB (schema.org accessibility summary) et préciser notament les déficiences potentielles.

Les informations relatives à la conformité et à la politique d'accessibilité de l'éditeur contenues dans les codes 196 93 à 99 devraient également être transportées si elles sont présentes.

* [196 	93 	Certification de conformité par](https://ns.editeur.org/onix/en/196/93)
* [196 	94 	Page web pour les informations détaillées d’accessibilité](https://ns.editeur.org/onix/en/196/94)
* [196 	95 	Page web d’un intermédiaire approuvé pour les informations détaillées d’accessibilité](https://ns.editeur.org/onix/en/196/95)
* [196 	96 	Page web de l’éditeur pour les informations détaillées d’accessibilité](https://ns.editeur.org/onix/en/196/96)
* [196 	97 	Compatibilité testée](https://ns.editeur.org/onix/en/196/97)
* [196 	98 	Contact intermédiaire approuvé](https://ns.editeur.org/onix/en/196/98)
* [196 	99 	Contact éditeur pour informations complémentaires sur l’accessibilité](https://ns.editeur.org/onix/en/196/99)

</div>

<aside markdown="1">
<h2> Ressources</h2>

<a href="https://ns.editeur.org/onix/fr/196" class="link color_orange">ONIX liste 196</a>

<a href="https://edition-accessible.github.io/signalement/references/references.html" class="link color_orange">Tableau de correspondances schema.org et ONIX en Français</a>

<a href="https://w3c.github.io/publ-a11y/drafts/a11y-crosswalk-MARC/" class="link color_orange">Tableau de correspondances schema.org, ONIX, MARC21 et UNIMARC en Anglais</a>

<a href="https://w3c.github.io/publ-a11y/drafts/a11y-crosswalk-MARC/" class="link color_orange">Tableau de correspondances schema.org, ONIX, MARC21 et UNIMARC en Anglais</a>

</aside>
