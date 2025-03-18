---
layout: page
title: Distribuer
date: 2025-01-24
subtitle: par la vente ou le prêt
orientation: permettre aux personnes d'acquérir ou d'emprunter un livre numérique
audience: libraires et bibliothèques
previous: ./diffuser.html
next: ./afficher.html
titleNext: Afficher
titlePrev: Informer
draft: false
---

<div markdown="1" id="principes">

{%- include principes.html -%}

Les services de vente et de prêt en ligne sont concernés par des exigences d’accessibilité prévues par les textes européens : la directive 2016/2102 du 26 octobre 2016 relative à l'accessibilité des sites internet et des applications mobiles des organismes du secteur public et la directive 2019/882 du 17 avril 2019 relative aux exigences en matière d'accessibilité applicables aux produits et services. Ces exigences ont été transposées, pour les sites publics, dans les articles 47 et 47-1 de la Loi n° 2005-102 du 11 février 2005 et, pour les sites de commerce électronique, dans le code de la consommation (Art. D. 412-49 et suivants).

Ces services peuvent prendre la forme d'un site web ou d'un catalogue dans un format de distribution privé (API) ou standardisé comme OPDS. Dans tous les cas, des mesures doivent être prises pour qu’il n’y ait pas de ruptures ni d’obstacles dans le parcours utilisateur pour la consultation de livres numériques via les sites de vente ou de prêt.

<h3 id="sitesweb">Accessibilité du parcours utilisateur sur les sites de vente et de prêt de livres numériques</h3>

Pour s'assurer que les livres numériques peuvent être achetés ou empruntés par un grand nombre de personnes incluant celles en situation de handicap les développeurs de bibliothèques ou librairies en ligne doivent prendre en compte plusieurs aspects. Voici une liste détaillée basée sur les normes et recommandations liées dans les ressources :

1. Assurer que le site web respecte les critères de succès des WCAG, au niveau AA.
2. Effectuer des tests avec des utilisateurs en situation de handicap pour identifier les obstacles les plus bloquants et les stratégies de contournement.
3. Réaliser des évaluations régulières pour s'assurer que le site web ou l'application respecte les normes d'accessibilité.
4. Former les équipes de développement et de design aux principes de l'accessibilité numérique.
Sensibilisation : Sensibiliser l'ensemble de l'organisation à l'importance de l'accessibilité numérique.
5. Mettre en place des mécanismes pour recueillir le feedback des utilisateurs en situation de handicap et maintenir dans le temps un niveau correct d’accessibilité (niveau AA des WCAG).

Les points d'attention principaux concernent : 
* Permettre une navigation complète au clavier, sans nécessiter l'utilisation de la souris.
* Assurer la compatibilité avec les technologies d’assistance comme les lecteurs d'écran, les synthèses vocales, les dispositifs braille ou encore les méthodes de pointage alternatif.
* Utiliser des combinaisons de couleurs avec un contraste suffisant et ne pas utiliser les couleurs comme seul moyen de transmettre des informations.
* Adapter la mise en page pour faciliter la lecture (justification, interlignage, espacement des mots).
* Assurer la compatibilité avec les dispositifs de contacteur et les sticks de contrôle.
* Intégrer des commandes vocales pour faciliter la navigation.
* Nommer les boutons et les liens pour qu'ils soient facilement compréhensibles.
* Rendre les formulaires et les messages d'erreur clairs et accessibles.
* Fournir des sous-titres et des transcriptions pour les contenus audio et vidéo.
* Offrir des alternatives textuelles pour les images et les éléments non textuels.
* Assurer que le site web ou l'application est performant et stable pour tous les utilisateurs.

<h3 id="catalogues">Accessibilité des catalogues numériques</h3>

L'accès aux collections de livres numériques pour les lecteurs doit être rendu possible sans passer par un site web, et doit pouvoir être proposé directement depuis leur application de lecture préférée. Plusieurs solutions existent, souvent sous forme d'APIs privées qui nécessitent un développement spécifique pour être intégrées dans une application de lecture. Toutes ces APIs doivent respecter les WCAG (Web Content Accessibility Guidelines) et assurer un niveau d'information et de compréhension via les mêmes mécanismes que ceux utilisés pour les sites web.

Afin de garantir l’interopérabilité et le choix de l'application de lecture sans multiplier les besoins de développement, il est conseillé de privilégier un standard ouvert comme le protocole OPDS (Open Publication Distribution System). Ce protocole permet aux applications de lecture de proposer un grand nombre de catalogues sans efforts de développement supplémentaires.

Les catalogues créés avec le protocole OPDS permettent leur consultation directement au sein des applications de lecture, offrant ainsi à l'utilisateur la possibilité d'utiliser un logiciel auquel il est habitué. Cela évite à l'utilisateur de changer de contexte et de devoir comprendre l'organisation d'un site web, améliorant ainsi l'expérience utilisateur.

Quel que soit le protocole choisi pour votre catalogue, vous devez vous assurer de fournir une information riche et cohérente, comprenant notamment les métadonnées d’accessibilité. Il est également crucial de proposer des fonctionnalités de recherche et de filtrage pour permettre aux utilisateurs de trouver facilement les ressources qui les intéressent. En intégrant ces éléments, vous pouvez créer un catalogue de livres numériques qui est non seulement accessible, mais aussi intuitif et facile à utiliser pour tous les lecteurs.

Bien sûr, pour que le lecteur en tire tout le bénéfice possible, il est nécessaire que l'application de lecture soit elle même accessible selon les principes détaillés à la page [Afficher](https://www.lina25.fr/pages/afficher.html) de ce site web.  

</div>

<section  class="ressources" markdown="1">

<h2>Ressources</h2>
<h3>Textes</h3>

<a href="https://eur-lex.europa.eu/legal-content/FR/TXT/?uri=CELEX:32016L2102" class="link color_orange">Directive 2016/2102 relative à l'accessibilité des sites web du secteur public</a>

<a href="https://eur-lex.europa.eu/legal-content/FR/TXT/?uri=CELEX:32019L0882" class="link color_orange">Directive 2019/882 sur l'accessibilité des produits et services</a>

<a href="https://www.legifrance.gouv.fr/codes/section_lc/JORFTEXT000000809647/LEGISCTA000006125163/#LEGISCTA000006125163" class="link color_orange">Article 47 de la Loi n° 2005-102 du 11 février 2005 pour l'égalité des droits et des chances, la participation et la citoyenneté des personnes handicapées</a>

<a href="https://www.culture.gouv.fr/Thematiques/livre-et-lecture/le-livre-et-la-lecture-en-france2/accessibilite-du-livre-et-de-la-lecture2/l-acces-a-la-lecture-pour-les-personnes-en-situation-de-handicap">L’accès à la lecture pour les personnes en situation de handicap (Ministère de la culture et de la communication)

<h3>Standards</h3>

<a href="https://opds.io/" class="link color_orange"><span lang="en">Open Publication Distribution System</span> (en anglais)</a>

</section>