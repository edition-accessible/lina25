---
layout: document
date:  2025-05-05
title: "Recommandations pour l'affichage des informations d'accessibilité"
previous: ../pages/diffuser.html
titlePrev: Informer
draft: false
---

<div markdown="1" id="principes">

À partir du 28 juin 2025, les sites et portails proposant des livres numériques en prêt ou à la vente doivent informer les personnes des caractéristiques d’accessibilité des livres numériques qui leur sont proposés.

Le W3C, à travers son groupe de travail sur l'accessibilité des publications numériques, a publié en avril 2025 la version 2.0 de son guide de présentation des métadonnées d'accessibilité. Ce guide, intitulé <a href="https://www.w3.org/publishing/a11y/metadata-display-guide/guidelines/">"<span lang="en">Accessibility Metadata Display Guide for Digital Publications 2.0"</span></a> (Guide d'affichage des métadonnées d’accessibilité), vise à standardiser la manière dont les informations d'accessibilité sont présentées aux utilisateurs. Il est disponible en anglais, de précédentes versions étaient traduites pour faciliter les retours, mais la dernière version n'a pas été traduite. Cette page résume les informations à connaître pour utiliser au mieux ce guide.

Ce guide a été élaboré dans le cadre du <a href="https://www.w3.org/community/publishingcg/"><span lang="en">Publishing community group</span></a>, un espace ouvert et public auquel il est possible de participer sans adhérer au W3C. Les discussions sont publiques et les décisions prises au consensus. C’est un espace de collaborations internationales où des organisations professionnelles, comme EDRLab, DAISY Consortium, Benetech, Fondazione LIA, et des acteurs industriels, comme Kobo et VitalSource, travaillent ensemble pour développer des outils et des standards communs.

Le guide est accompagné de documents techniques pour faciliter l’implémentation par les équipes techniques ainsi que d’une série de fichiers de formulations en différentes langues pour permettre la localisation du vocabulaire au plus proche des réalités culturelles et, potentiellement, des audiences spécifiques.

*Cette recommandation est établie au niveau international par le W3C et transcrite en français à partir d’un travail interprofessionnel piloté par EDRLab dans le cadre d’une mission confiée par le comité de pilotage interministeriel. Elle a désormais atteint une maturité suffisante mais peut être mise à jour en fonction des avancées du projet et des recommandations internationales.*

<h3>Métadonnées généralistes</h3>

Toutes les métadonnées utilisées pour déterminer l'accessibilité d'une publication ne sont pas strictement classées dans la catégorie d'accessibilité. Les détails du produit, par exemple, fournissent des informations importantes sur la facilité d'utilisation d'un livre électronique par rapport aux besoins spécifiques de l'utilisateur.

En particulier, les informations suivantes devraient toujours être affichées&nbsp;:

* **Format de fichier** (EPUB 2 ou 3, PDF, MP3, livre audio, etc.) - Le format de fichier donne une forte indication de l'accessibilité&nbsp;: un PDF ne permet pas de modifier la typographie, l'EPUB 2 est déprécié, un EPUB 3 prend en charge la navigation dans les pages et une meilleure sémantique structurelle ; un livre audio au format MP3 sera moins structuré qu'un livre audio, etc.
* **Mesure de protection** ou absence de mesure de protection - La mesure de protection peut bloquer les technologies d'assistance telles que les lecteurs d'écran. En outre, de nombreux appareils de lecture électronique spécifiques, tels que les lecteurs DAISY ou les appareils de prise de notes en braille, ne sont pas équipés pour lire les fichiers cryptés.
* **Nom de la maison d'édition** - Le nom de la maison d'édition peut mettre en évidence les efforts qu'elle a faits en matière d'accessibilité.
* **Langue principale du contenu** - La langue principale du contenu permet aux lecteurs d'être sûrs qu'ils pourront lire avec leur technologie d'assistance qui utilise la voix synthétisée ou la table de traduction en braille correspondant à la langue.

Il n'est pas nécessaire d'inclure ces métadonnées dans la section relative à l'accessibilité ; il suffit de les mettre à la disposition des utilisateurs dans l'affichage des métadonnées d'une publication.

<h3>Les principales catégories d'accessibilité</h3>

Le guide du W3C identifie huit catégories clés pour informer sur l'accessibilité d'un livre numérique&nbsp;:

* Lisibilité (<span lang="en">Ways of reading</span>)&nbsp;: Peut-on modifier l'apparence du texte et de la mise en page ? Peut-on lire ce livre en braille ou avec la voix de synthèse ?
* Règles d'accessibilité (<span lang="en">Conformance</span>)&nbsp;: Le livre respecte-t-il des normes reconnues (comme WCAG 2.1) ?
* Points de repère (<span lang="en">Navigation</span>)&nbsp;: Le livre inclut-il des tables des matières, des index, ou des références de pagination ?
* Contenus spécifiques (<span lang="en">Rich content</span>)&nbsp;: Les images, graphiques ou formules mathématiques sont-ils décrits de manière accessible ?
* Points d'attention (<span lang="en">Hazards</span>)&nbsp;: Le livre contient-il des éléments potentiellement problématiques (flashs, sons intempestifs) ?
* Informations supplémentaires (<span lang="en">Accessibility summary</span>)&nbsp;: Des détails sur l'accessibilité sont-ils fournis ?
* Considérations juridiques (<span lang="en">Legal considerations</span>)&nbsp;: Le livre respecte-t-il les exigences légales en matière d'accessibilité ?
* Informations complémentaires (<span lang="en">Additional accessibility information</span>)&nbsp;: D'autres fonctionnalités d'accessibilité sont-elles disponibles ?

<h3>Trois informations clés à toujours afficher</h3>

Parmi ces catégories, trois informations sont jugées essentielles et devraient toujours être présentées aux lecteurs&nbsp;:
* Lisibilité (<span lang="en">Ways of reading</span>)&nbsp;: Par exemple, "L'apparence du texte et la mise en page peuvent être modifiées."
* Points de repère (<span lang="en">Navigation</span>)&nbsp;: Par exemple, "Le livre contient une table des matières navigable."
* Règles d'accessibilité (<span lang="en">Conformance</span>)&nbsp;: Par exemple, "Ce livre respecte les normes WCAG 2.1 Level AA."

<h3>Flexibilité</h3>

Pour assurer le consensus et permettre une adoption la plus large possible, le guide propose plusieurs points de flexibilité. 

<h4>Formulations compactes et descriptives</h4>

Le guide propose des formulations courtes ou longues à utiliser selon le contexte, la place disponible et le niveau d’information nécessaire aux personnes utilisatrices. Par exemple, la formulation courte “L'affichage peut être adapté" correspond à la formulation longue “L'apparence du texte et la mise en page peuvent être modifiées en fonction des capacités du système de lecture (famille et taille des polices, espaces entre les paragraphes, les phrases, les mots et les lettres, ainsi que la couleur de l'arrière-plan et du texte)."

<h4>L’intitulé de la section </h4>

Les informations d’accessibilités doivent être regroupées dans une section facilement atteignable et identifiable, notamment par les technologies d’assistance. Le titre de cette section doit  clairement indiquer à l'utilisateur final que les informations proviennent directement de l'éditeur et qu'elles représentent l'intention de communication de ce dernier. Il est suggéré d'introduire la section en utilisant des termes tels que « Déclarations d'accessibilité.

<h4>L'ordre dans lequel afficher les informations</h4>

Selon le contexte, l’ordre de présentation des informations permet de mettre en avant une activité de certification ou, au contraire, de mettre l’accent sur les fonctionnalités liées à la lecture. 

<h4>Utilisation ou non des titres de catégories</h4>

Bien que les catégories de métadonnées soient nommés dans le guide, il n'est pas nécessaire que les responsables de la mise en œuvre utilisent ces noms comme en-têtes de champ. Ils peuvent utiliser d'autres noms de champs s'ils ont plus de sens dans leur contexte d'affichage.

<h4>Afficher ou masquer l’absence d’information </h4>

Lorsque l'éditeur ne fournit aucune métadonnée d'accessibilité, il est préférable d'éviter de faire une déclaration négative qui pourrait lui être attribuée (par exemple, déclarer que l'on ne sait pas si une fonctionnalité est disponible pourrait être interprété à tort comme une déclaration de l'éditeur indiquant qu'il n'est pas sûr). La mention neutre « Aucune information n'est disponible » est à privilégier dans ce cas.

Dans certains cas, le distributeur peut ne pas être autorisé à afficher des déclarations que l'éditeur n'a pas faites. Dans ce cas, il est préférable de masquer ces sections.

<h3> Techniques</h3>
Le guide est accompagné de deux documents techniques détaillant les algorithmes en language XPath qui permettent d’obtenir ces affichages depuis des métadonnées disponibles dans un EPUB ou dans une fiche ONIX. Des documents similaires sont attendus pour les documents PDF et les notices MARC. Pour le moment, le document de référence <a href="https://w3c.github.io/a11y-discov-vocab/crosswalk/">Accessibility Properties Crosswalk (schema.org, ONIX, MARC21 & UNIMARC)</a> peut permettre de palier aux besoins. 

<h3>Outils de test</h3>

* <a href="https://daisy.github.io/a11y-meta-viewer/">DAISY Accessibility Metadata Viewer</a>&nbsp;: Le visualiseur de métadonnées d'accessibilité DAISY est un outil de test gratuit basé sur un navigateur qui permet aux utilisateurs d'examiner les métadonnées qui seront générées selon les directives et les techniques d'affichage. Il peut être exécuté en ligne ou téléchargé et exécuté localement. La visionneuse permet d'afficher les mentions descriptives ou compactes, de sélectionner la langue d'affichage et de supprimer les champs pour lesquels aucune information n'est disponible.
* <a href="https://thorium.edrlab.org/">Thorium Desktop</a>&nbsp;: Cette application de lecture développée par EDRLab affiche les informations d'accessibilité disponibles dans les livres au format EPUB ainsi que celles fournies via un flux de catalogue OPDS.

<h3>Les défis à relever</h3>

Malgré les progrès réalisés, plusieurs défis subsistent&nbsp;:

* **Enrichir les métadonnées**&nbsp;: Tous les éditeurs ne fournissent pas encore des métadonnées d'accessibilité complètes, cela est encore plus vrai lorsqu’il s’agit d’ajouter de l’information aux livres du fond. Des règles d’inférence existent et peuvent être mise en oeuvre, notamment en utilisant l’utilitaire <a href="https://github.com/readium/cli">Readium CLI</a> (précédement inclut dans le Readium Go Toolkit).
* **Implémenter le guide à tous les niveaux**&nbsp;: que ce soit sur un catalogue en ligne comportant des centaines de milliers de référence ou bien sur la page du site de l’éditeur, ces informations devraient être disponibles partout. Le guide et son appareillage permettent une implémentation facile.
* **Associer les lecteurs**&nbsp;: Les utilisateurs doivent être informés de la présence de ces métadonnées pour choisir des livres adaptés à leurs besoins, il est suggéré de mettre en oeuvre des pages de documentation dédiées, des sondages et des communications pour associer les lecteurs.
* **Collecter et comparer**&nbsp;: des études statistiques devraient être mises en oeuvre pour faire connaître et mesurer l’évolution du nombre de livres disponibles avec des fonctionnalités d’accessibilité. 


<h3>Au sujet des livres imprimés</h3>
<p>Les livres imprimés ne peuvent prétendre à une accessibilité universelle, à moins d'être livrés en différentes versions dans une même édition. Cependant certaines éditions spécialisées peuvent répondre à des besoins spécifiques. </p>
<p>ONIX permet d'informer sur ces éditions. Si la liste 196 est dédiée à l'accessibilité numérique, la <a href="https://ns.editeur.org/onix/fr/21">liste 21</a> permet d'indiquer un type d'édition particulier. On retiendra en particulier&#8239;:</p>

* <a href="https://ns.editeur.org/onix/fr/21/HRE">21:HRE Édition haute lisibilité</a>
* <a href="https://ns.editeur.org/onix/fr/21/BRL">21:BRL Édition en Braille</a>
* <a href="https://ns.editeur.org/onix/fr/21/ETR">21:ETR Édition facile à lire</a>
* <a href="https://ns.editeur.org/onix/fr/21/LTE">21:LTE Édition en grands caractères</a>
* <a href="https://ns.editeur.org/onix/fr/21/ULP">21:ULP Édition en très gros caractères</a>
  
<p>Les libellés peuvent être utilisés tels que proposés par ONIX.</p>

</div>