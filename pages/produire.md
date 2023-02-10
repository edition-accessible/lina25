---
layout: page
title: Produire
subtitle: des structures sémantiques riches
orientation: assurer la qualité des fichiers produits et leur conformité avec les exigences de la directive européenne.
audience: services de production et prestataires techniques des éditeurs
previous: ./concevoir.html
next: ./traiter.html
titleNext: Traiter
titlePrev: Concevoir
---

<div markdown="1" id="principes">

{%- include principes.html -%}

Un environnement de lecture ne peut être accessible que s’il s’appuie sur des standards techniques ouverts et partagés. Les personnes en situation de handicap recourent à des outils de lecture spécifiquement conçus pour répondre à leurs besoins. Ces dispositifs dits technologies d’assistance, sont par exemple&#8239;: lecteurs d’écran, logiciels de synthèse vocale, lecteurs de livres audio structurés, logiciels d’adaptation automatique des paramètres d’affichage des textes, ou plages braille. Il est donc souhaitable d’utiliser des formats de publication interopérables, qui puissent être pris en charge par ces technologies. Parce qu’il répond à ces attentes, l’EPUB 3 est aujourd’hui le format de référence pour les professionnels du secteur en matière d’accessibilité du livre numérique et son utilisation tend à se généraliser.

### Reproduire les information sémantiques dans le code

Les technologies d'assistance comme les dispositifs de lecture s'appuient sur la richesse sémantique du balisage des contenus. Pour chaque groupe et portion de texte, il faut ainsi assigner la sémantique correspondante. Il faut privilégier le vocabulaire HTML5, mais comme ce dernier reste très générique, il est nécessaire de le préciser à l'aide des vocabulaires EPUB type et DPUB ARIA. Ces deux derniers sont complémentaires, le premier adressant les dispositifs de lecture et le second les technologies d'assistance. Vous pouvez vous référer aux document des standards 
<span lang="en"><cite>EPUB 3 Structural Semantics Vocabulary 1.1</cite></span> et 
<span lang="en"><cite>DPUB-ARIA vocabulary</cite></span>. En cas de doute la Base de connaissance 
<span lang="en"><cite>Accessible Publishing Knowledge Base</cite></span> maintenue par le Consortium Daisy vous permettra de consulter des exemples et de trouver de l'information supplémentaire. Les balises génériques comme `div` et `span` ne devraient être utilisées que pour des besoins non couverts par les balises HTML.

Afin de faciliter et standardiser la production de livres numériques nativement accessibles au format EPUB 3, le SNE (Syndicat national de l’Edition) a rédigé une charte technique, disponible au format PDF. Cette charte “EPUB NAC” (pour _Nativement ACcessible_) reprend les recommandations des référentiels d’accessibilité internationaux et apporte des éclaircissements sur tout ce qui fait question dans les standards d’accessibilité applicables au format EPUB.

Il n'existe pas à ce jour de document répertoriant l'usage des Roles ARIA par les technologies d'assistance comme les lecteurs d'écrans. Nous savons néanmoins que les meilleures prises en charge sont assurées par talkback (android) et donc constatables sur les applications Google Play Livre ou Aldiko.

### Insérer les descriptions des ressources graphiques

Dans la plupart des cas, l’auteur du livre n’aura pas décrit les images de l’ouvrage. Les services de production devront alors se référer au guide de bonnes pratiques rédigé par le SNE pour la rédaction des alternatives aux images. Le document _Mise en accessibilité des images dans les EPUBs - synthèse des travaux du groupe normes et standard du SNE_ apporte des explications sur les principes et techniques à appliquer.

Le groupe de travail sur la transition vers l'EPUB du Consortium DAISY maintient un document <span lang="en"><cite>Best Practices for Authoring Extended Descriptions in EPUB</cite></span> qui vous permettra de tester les possibilités et d'étudier leur réalisation.

### Contrôler la qualité des fichiers

Une fois produits, les fichiers EPUB 3 devront être validés par la version à jour de EPUBCheck. Mais cet outil ne teste pas l’accessibilité des publications. Pour cela, il faudra faire appel à l’outil de test Ace by DAISY développé par le Consortium DAISY. Le logiciel Ace n’est pas conçu pour être utilisé de manière automatique&#8239;: il ne délivre pas un jugement du type _“cet EPUB est / n’est pas accessible”_ mais génère un rapport HTML mettant l'accent sur les enfreintes aux règles d'accessibilité&#8239;; il met également en évidence la structure de la publication et affiche les attributs d’accessibilité présents dans ses images. La qualité sémantique de la publication n’est pas jaugée par la mécanique de cet outil. La génération de métadonnées d’accessibilité, et en particulier l’évaluation d’un niveau de conformité WCAG, nécessite un audit du rapport Ace.

Le Consortium DAISY a donc également développé un outil nommé SMART (Simple Manual Accessibility Report Tool), qui indique les contrôles manuels nécessaires pour garantir la conformité aux exigences EPUB et WCAG. SMART est le compagnon idéal de Ace, il vous guide pour établir et générer un rapport de conformité complet. Ensemble, ils fournissent la méthode la plus complète pour les tests de conformité d'accessibilité des publications EPUB.

Pour utiliser SMART, vous devez d'abord faire passer votre EPUB par Ace, qui effectue une vérification automatisée et recueille des informations sur les caractéristiques du titre. Ace génère un rapport au format JSON, qui est ensuite chargé par l'utilisateur dans l'outil SMART. SMART remplit les informations de l'évaluation et configure intelligemment le protocole de test manuel sur la base des résultats de Ace.

À partir de ce moment&#8239;:

-   SMART vous guide tout au long du processus de vérification manuelle
-   Les points de contrôle sont adaptés en fonction des propriétés de votre publication
-   SMART génère un rapport cohérent et clair

SMART est conçu pour être polyvalent. Il s'intègre à la base de connaissances sur la publication accessible de DAISY pour fournir des informations sur l'accessibilité qui font autorité aux auteurs, aux éditeurs et aux fournisseurs de la chaîne d'approvisionnement. Il peut être intégré à de nombreux flux de travail différents dans une variété de points de contrôle d'assurance qualité.

SMART est libre d'utilisation. Créez un compte à l’adresse smart.daisy.org pour avoir un accès complet à l'application. À ce jour, SMART n’est disponible qu’en anglais.

Notez que pour vérifier comment sont rendus les arguments ARIA Role il est nécessaire de lire et manipuler le livre avec un lecteur d'écran. Les fabricants de ces derniers ne communiquent pas sur l'usage qu'ils en font, ce dernier pouvant être influencé par le paramétrage de verbosité sélectionné par l'utilisateur. 

epubtest.org donne une visibilité sur la prise en charge des fonctionnalités d'accessibilité par les dispositifs de lecture. Les fichiers utilisés pour ces tests sont disponibles à la même adresse et peuvent servir d'exemple si vous avez des doutes sur les formes et imbrications à utiliser. 

### Ajouter des métadonnées d’accessibilité aux fichiers

La classe schema.org CreativeWork comprend un ensemble de propriétés utilisées pour identifier les qualités d'accessibilité d'une publication. Ces métadonnées doivent être incluses dans le paquet OPF du fichier EPUB.

Les métadonnées obligatoires sont <span lang="en">**accessMode**, **accessModeSufficient**, **accessibilityFeature**</span> et <span lang="en">**accessibilityHazard**. **accessibilitySummary**</span> est fortement recommandé. Le nom de ce dernier est trompeur. Il ne s'agit pas d'un résumé complet, mais d'un complément d'information, d'une clarification et d'une amélioration des autres métadonnées d'accessibilité. Lors de la création du résumé d'accessibilité, il faut partir du principe que les autres métadonnées d'accessibilité ont déjà été présentées et que le résumé d'accessibilité sert à améliorer ces métadonnées. Si la publication présente des caractéristiques ou des lacunes qui ne sont pas exprimées dans les autres métadonnées d'accessibilité, le résumé d'accessibilité est l'endroit approprié pour inclure ces informations. Un guide de rédaction de ce résumé est en cours d'élaboration au sein du groupe des éditeurs du W3C. <span lang="en"><cite>[Accessibility Summary Authoring Guidelines for EPUB Publications Draft Community Group Report 07 December 2022](https://w3c.github.io/publ-a11y/drafts/schema-a11y-summary/)</cite></span>.

### Le cas des EPUB Fixed Layout et des PDF

La directive Européenne exige que le livre numérique utilise _une police de caractères de taille et de forme appropriées compte tenu des conditions d’utilisation prévisibles, ainsi qu’un contraste suffisant, et en ménageant un espace ajustable entre les lettres, les lignes et les paragraphes (Section III-b-v)_.

Cette exigence est remplie par le format EPUB redistribuable puisqu'il permet à l'utilisateur de modifier la police, la taille et les espacements. Ce n'est pas le cas des formats fixes tels que l'EPUB Fixed-Layout ou le PDF.

Dans ce cas, il est recommandé de prévoir une version accessible de l'ouvrage au format EPUB redistribuable. Un groupe de travail du W3C dédié à la question de l'accessibilité du Fixed Layout travaille actuellement sur l'élaboration de techniques pour surmonter les difficultés inhérentes au format.

</div>

<section  class="ressources" markdown="1">

<h2>Ressources</h2>
<ul>
<li>

<a href="https://www.sne.fr/app/uploads/2020/12/ePubAccessibleCharteSNE_v1.0-au-08-12-2020.pdf" class="link color_orange">Charte technique pour la production d’EPUBs “textuels” nativement accessibles (SNE)</a></li>
<li>

<span lang="en"><a href="https://kb.daisy.org/publishing/docs/" class="link color_orange">Accessible Publishing Knowledge Base (en anglais, base de connaissance maintenue par le consortium DAISY)</a></span></li>

<li><a href="https://www.oreilly.com/library/view/accessible-epub-3/9781449329297/" class="link color_orange">Accessible EPUB 3, by Matt Garrish (en anglais, ebook publié par O’Reilly, téléchargement gratuit)</a>
</li>
<li><a href="https://w3c.github.io/epub-specs/epub33/fxl-a11y/" class="link color_orange">EPUB Fixed Layout Accessibility (en anglais, travaux en cours sur l'accessibilité des formats EPUB Fixed Layout)</a>
</li>
</ul>

### Les référentiels
<ul>

<li>

<a href="http://www.edrlab.org/public/sne/TAE_HTML_V3/Techniques_d_Accessibilite_EPUB%201.0.html" class="link color_orange">Techniques d’Accessibilité EPUB 1.0</a></li>

<li>

<a href="https://www.w3.org/Submission/epub-a11y/" class="link color_orange">EPUB Accessibility 1.0 (en anglais, version stable)</a></li>

<li>

<a href="https://idpf.org/epub/a11y/techniques/" class="link color_orange">EPUB Accessibility Techniques 1.0  (en anglais, version stable)</a></li>

<li>

<a href="https://www.w3.org/TR/epub-a11y-11/" class="link color_orange">EPUB Accessibility 1.1  (en anglais, version en cours de validation)</a></li>

<li>

<a href="https://www.w3.org/TR/epub-a11y-tech-11/" class="link color_orange">EPUB Accessibility Techniques 1.1  (en anglais,  version en cours de validation)</a></li>

<li>
<span lang="en"><a href="https://www.w3.org/TR/epub-ssv/" class="link color_orange">EPUB 3 Structural Semantics Vocabulary 1.1</a></span></li>

<li>

<span lang="en"><a href="https://www.w3.org/TR/dpub-aria/" class="link color_orange">DPUB-ARIA vocabulary</a></span></li>

<li>
<a href="https://www.w3.org/TR/WCAG20/" class="link color_orange">Web Content Accessibility Guidelines (WCAG) 2.0 (en anglais, applicables aux pages Web qui constituent les ressources des fichiers EPUB 3)</a></li>

<li>
<a href="https://www.w3.org/WAI/ARIA/apg/" class="link color_orange">ARIA Authoring Practices Guide (en anglais, applicables aux pages Web qui constituent les ressources des fichiers EPUB 3)</a>
</li>

</ul>






### Alternatives aux ressources graphiques
<ul>

<li>
<a href="https://www.sne.fr/app/uploads/2022/10/SNE-Normes-et-stanrdards-Textes-alternatifs-image-Document-de-synthese-.._vdef2.pdf" class="link color_orange">Mise en accessibilité des images dans les EPUBs - synthése des travaux du groupe normes et standard du SNE, octobre 2022 (PDF non balisé, 2 Mo)</a></li>

<li>

<a href="https://daisy.github.io/transitiontoepub/best-practices/extended-desc/ExtendedDescriptionsBestPractices.html" class="link color_orange">Best Practices for Authoring Extended Descriptions in EPUB</a></li>

</ul>

### Contrôle
<ul>

<li>
<a href="https://github.com/w3c/epubcheck/releases" class="link color_orange">EPUBCheck</a></li>

<li>

<a href="https://daisy.org/activities/software/ace/" class="link color_orange">Ace by DAISY</a></li>

<li>

<a href="https://daisy.org/activities/services/smart/" class="link color_orange">SMART by DAISY</a></li>

<li>

<a href="https://epubtest.org/results" class="link color_orange">epubtest.org</a></li>
 <!-- permet de vérifier la prise en charge des fonctionnalitées par les dispositifs de lecture. Les fichiers test peuvent aussi être utiles comme exemples. -->
</ul>

### Métadonnées

<ul>

<li>
<a href="http://www.schema.org/CreativeWork" class="link color_orange">schema.org CreativeWork class</a>
</li>

<li>
<span lang="en"><a href="https://w3c.github.io/publ-a11y/drafts/schema-a11y-summary/" class="link color_orange">
Accessibility Summary Authoring Guidelines for EPUB Publications Draft Community Group Report 07 December 2022</a></span></li>

</ul>

</section>