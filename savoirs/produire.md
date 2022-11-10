---
layout: page
title: Produire des structures sémantiques riches 
permalink: 
ressources: 
orientation: 
audience: services de production et prestataires techniques des éditeurs
image: /assets/images/customizable-feature.png
---
Un environnement de lecture ne peut être accessible que s’il s’appuie sur des standards techniques ouverts et partagés. Les personnes en situation de handicap recourent à des outils de lecture spécifiquement conçus pour répondre à leurs besoins, dits technologies d’assistance, tels que : lecteurs d’écran, logiciels de synthèse vocale, lecteurs de livres audio structurés, logiciels d’adaptation automatique des paramètres d’affichage des textes, ou plages braille. Il est donc souhaitable d’utiliser des formats de publication interopérables, qui puissent être pris en charge par ces technologies. Parce qu’il répond à ces attentes, l’EPUB 3 est aujourd’hui le format de référence pour les professionnels du secteur en matière d’accessibilité du livre numérique et son utilisation tend à se généraliser.

Afin de faciliter et standardiser la production de livres numériques nativement accessibles au format EPUB 3, le SNE (Syndicat national de l’Edition) a rédigé une charte technique, disponible au format PDF : [Charte technique pour la production d’EPUBs “textuels” nativement accessibles (SNE)]
Cette charte “EPUB NAC” (pour Nativement ACcessible) reprend les recommandations des référentiels d’accessibilité internationaux et apporte des éclaircissements sur tout ce qui fait question dans les standards d’accessibilité applicables au format EPUB. 

Dans la plupart des cas, l’auteur du livre n’aura pas décrit les images de l’ouvrage. Les services de production devront alors se référer au guide de bonnes pratiques rédigé par le SNE pour la rédaction des descriptions d’images.
[Titre du guide SNE pour les description d’images](lien)

Bien entendu, une fois produits, les fichiers EPUB 3 devront être validés par la version à jour de EPUBCheck (https://github.com/w3c/epubcheck/releases). 

Mais cet outil ne teste pas l’accessibilité des publications. Pour cela, il faudra faire appel à l’outil de test [Ace by DAISY](https://daisy.org/activities/software/ace/) développé par le Consortium DAISY. Il est important de savoir que le logiciel Ace n’est pas conçu pour être utilisé de manière automatique : il ne délivre pas un jugement du type “cet EPUB est / n’est pas accessible” mais génère un rapport HTML mettant l'accent sur les violations de règles d’accessibilité, la présence ou non de métadonnées d’accessibilité ; il met également en évidence la structure de la publication et affiche les attributs d’accessibilité présents dans ses images. La qualité sémantique de la publication n’est pas jaugée par la mécanique de cet outil. La génération de métadonnées d’accessibilité, et en particulier l’évaluation d’un niveau de conformité WCAG, nécessite un audit du rapport Ace. 

Le Consortium DAISY a donc également développé un outil nommé [Ace SMART](https://daisy.org/activities/services/smart/), qui fournit les contrôles manuels nécessaires pour garantir la conformité aux exigences EPUB et WCAG. SMART est proposé directement par DAISY et ses membres dans le cadre d'un service de conseil ou d'audit, son usage libre par les éditeurs est limité à cinq livres par mois.

## Pour en savoir plus

### Référentiels applicables aux livres numériques au format EPUB 3 :
* Techniques d’Accessibilité EPUB 1.0 : http://www.edrlab.org/public/sne/TAE_HTML_V3/Techniques_d_Accessibilite_EPUB%201.0.htm 
* Guide de description des images (Diagram center, traduction BrailleNet)
* Ressources éducatives libres relatives à l’édition inclusive (traduction française de Inclusive Publishing in Practice) :
* Édition inclusive en pratique : https://www.inclusivepublishinginpractice.org/
* Référentiels en anglais, version stable :
* EPUB Accessibility 1.0 : https://www.w3.org/Submission/epub-a11y/ 
* EPUB Accessibility Techniques 1.0 : https://idpf.org/epub/a11y/techniques/ 

### Référentiels en anglais, version en cours de validation :
* EPUB Accessibility 1.1 : https://www.w3.org/TR/epub-a11y-11/ 
* EPUB Accessibility Techniques 1.1 : https://www.w3.org/TR/epub-a11y-tech-11/ 
* Ouvrage en anglais, version numérique maintenant gratuite : Accessible EPUB 3, by Matt Garrish (O’Reilly, téléchargement gratuit) : https://www.oreilly.com/library/view/accessible-epub-3/9781449329297/ 
* Guides en anglais de description d’images :
    * Diagram center 
    * Poet description tool 
* Référentiels en anglais, applicables aux pages Web qui constituent les ressources des fichiers EPUB 3 :
    * Web Content Accessibility Guidelines (WCAG) 2.0 : https://www.w3.org/TR/WCAG20/ 
    * ARIA Authoring Practices Guide : https://www.w3.org/WAI/ARIA/apg/ 
