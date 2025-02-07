---
layout: document
title: "Guide d'affichage des métadonnées d'accessibilité 2.0 (projet)"
date: 2025-02-07
previous: ../pages/diffuser.html
titlePrev: Renseigner
---

<p>
  <a href="https://www.w3.org/standards/types%23reports"
    >Projet de rapport du groupe communautaire</a
  > 05 février 2025. Traduction française, EDRLab.</p>
<p>Cette version : 
  <a
    href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/draft/guidelines/"
    >https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/draft/guidelines/</a
  >
</p>
<p>Dernière version en cours d’écriture : 
   <a href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/draft/guidelines/"
    >https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/draft/guidelines/</a
  >
</p>
<p>Éditeurs:</p>
* Charles LaPierre (<a href="http://www.benetech.org/">Benetech</a>)
* Gregorio Pellegrino (<a href="https://fondazionelia.org/">Fondazione LIA</a>)
* Gautier Chomel (<a href="https://www.edrlab.org/">EDRLab</a> )
* George Kerscher (<a href="https://daisy.org/">DAISY Consortium</a>)

<p>Retour d'information :  <a href="https://github.com/w3c/publ-a11y/issues/new/choose">new issue</a>.
</p>
<p>
  <a href="https://www.w3.org/policies/%23copyright">Copyright</a> © 2024 les
  contributeurs au Guide de l'expérience utilisateur pour l'affichage des
  métadonnées d'accessibilité 2.0, publié par le
  <a href="https://www.w3.org/groups/cg/publishingcg"
    >Publishing Community Group</a
  > dans le cadre de l'<a
    href="https://www.w3.org/community/about/agreements/cla/"
    >accord de licence des contributeurs communautaires du W3C (CLA)</a
  >. Un
  <a href="https://www.w3.org/community/about/agreements/cla-deed/">résumé</a
  > lisible par une personne est disponible.
</p>
<section id="abstract">
<p>L'accessibilité d'une publication est utile pour savoir
quelles que soient les capacités d'une personne, comme les éléments tels
Comme la possibilité de faire des ajustements visuels rendent un meilleur
Expérience de lecture pour tout le monde. Ces directives
documenter un cadre partagé pour présenter la publication
Déclarations de métadonnées d'accessibilité dans un
manière conviviale -pour offrir les informations aux utilisateurs finaux
d'une manière facile à comprendre
indépendamment de leurs connaissances techniques et sont cohérents
dans différentes publications et différents
Catalogues numériques. </p>
</section>
<section id="sotd"></section>
<section id="intro">
<h2>Introduction</h2>

<section id="overview">
<h3>Aperçu</h3>

<p>La lecture d'une publication numérique est une expérience très personnelle.
Pour la plupart des gens, c'est une routine et peu
une considération est accordée à la façon dont le titre a été obtenu avant
il est lu. Les utilisateurs peuvent aller dans une librairie ou une bibliothèque,
Recherchez le titre à acheter en ligne ou avoir le titre
sélectionné pour eux par un instructeur pour un
classe.</p>

<p>Considérez maintenant que la personne est aveugle et s'appuie sur l'assistance
technologie. L'utilisateur a besoin de cette technologie
pour les aider dans le processus d'achat ainsi que pour lire
le livre électronique. La personne peut se demander: volonté
Le lecteur d'écran travaille avec ce titre; y a-t-il une image
descriptions qui seront prononcées pour décrire
ces images; Y a-t-il des numéros de page accessibles;
L'ordre de lecture est-il correct, donc une prudence sera annoncée
Avant de lire le paragraphe qui pourrait être dangereux? Tous
De ces problèmes d'accessibilité sont des problèmes potentiels
Les consommateurs ont lorsqu'ils essaient d'acheter et finalement lire un
publication numérique dans n'importe quel format.</p>

<p>La bonne nouvelle est de plus en plus des éditeurs créent
publications numériques qui naissent accessibles (c'est-à-dire
accessible dès le départ, non fixé plus tard) et l'obtention du
validation d'accessibilité ou audit effectué par
organisations indépendantes.</p>

<p>Ces directives aident ceux qui souhaitent rendre l'accessibilité
les métadonnées directement aux utilisateurs comprennent comment
représenter les réclamations d'accessibilité inhérentes à
métadonnées d'accessibilité lisible par machine dans un
Interface utilisateur /expérience utilisateur conviviale (UI /UX). Ce
Document cible des implémenteurs tels que
librairies, bibliothèques, détaillants, distributeurs, etc. Contenu
Les créateurs bénéficieront de la lecture de ces directives et
sont encouragés à suivre<a
href="https://www.w3.org/TR/epub-a11y-11/">EPUB
Accessibilité 1.1
Section des exigences de conformité et de découverte et
ses techniques.</a></p>

<div class="note">
<p>Ce document présente des directives de haut niveau sans
allant dans des problèmes techniques liés au
Différentes normes de métadonnées dans l'industrie de l'édition.
</p>
<p> Par conséquent, <a href="#techniques"> Les techniques sont
disponible </a> qui illustrent aux développeurs comment
Récupérez les données pour afficher les informations décrites dans ce
document. </p>
</div>

<p>Métadonnées trouvées dans une publication numérique ou dans un
Le dossier externe correspondant peut avoir
des affirmations d'accessibilité importantes qui aident les utilisateurs finaux à trouver et
déterminer si la publication peut répondre à leur
besoins d'accessibilité spécifiques. </p>

<p> Ces métadonnées d'accessibilité utilisent des vocabulaires contrôlés pour
Laissez-le extraire et affiché uniformément à travers
différentes publications et localisée à différents utilisateurs
langues d'interface. La seule exception est l'accessibilité
Résumé, qui permet des déclarations d'accessibilité qui sont
unique à une publication et qui ajoute des informations pas
couvert par d'autres entrées de métadonnées. </p>

<p> Un aspect important est que le rôle de l'accessibilité
Les métadonnées résumées ont changé dans la dernière
Version de la spécification d'accessibilité EPUB, donc plus
analyse approfondie dans le<a
href="#accessibility-summary">Résumé de l'accessibilité </a>
La section est recommandée. </p>

<p> Ce document offre des conseils sur la façon de les agréger et d'afficher
réclame inhérent aux métadonnées aux utilisateurs finaux;
Ce ne sont pas des directives strictes, mais des suggestions pour
offrant une expérience cohérente aux utilisateurs à travers
différents portails. Différents implémenteurs peuvent choisir de
mettre en œuvre ces directives dans un peu
différent. Certains exemples peuvent être vus dans le <a
href="#implementations">Implémentations </a> Section
du document. </p>
</section>

<section id="processing-guide">
<h3>Traitement des métadonnées </H3>

<p> Le diagramme suivant illustre comment ces directives sont liées
aux techniques spécifiques au format dans le
processus de réception et d'affichage de l'accessibilité
métadonnées. </p>

<img class="responsive" src="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/draft/guidelines/media/MetadataProcessing.png"
aria-details="ecosystem"
alt="Aperçu du traitement des métadonnées EPUB, PDF, ONIX et Marc. La description suit." />

<div class="note">
<p>Les travaux sur l'intégration de PDF et Marc sont en cours. Le
Le diagramme et le texte de cette section seront mis à jour
dans les versions futures comme les documents connexes sont
finalisé. </p>
</div>

<p> Le diagramme classe deux façons de les métadonnées
accompagne une publication. Dans le premier sont numériques
formats de publication qui intégrent directement l'accessibilité
métadonnées (EPUB et PDF). Dans le second sont
Formats d'enregistrement des métadonnées externes (ONIX et Marc)
accompagner une publication numérique à mesure qu'elle bouge
à travers la chaîne d'approvisionnement. </p>

<p> Dans certains cas, une publication numérique peut inclure les deux
métadonnées internes et externes (par exemple, un epub
pourrait avoir des métadonnées d'accessibilité dans le document de package informatique
et être également fourni à un vendeur avec un
Enregistrement ONIX). Dans ces cas, les vendeurs et le système de lecture
Les développeurs déterminent par eux-mêmes qui
Ensemble de métadonnées qu'ils utiliseront pour afficher aux utilisateurs.</p>

<div class="note">
<p>Ce guide suppose que les métadonnées sont déjà dans l'un des
les formats décrits dans le diagramme, mais
Selon la façon dont les métadonnées sont soumises, elle peut
besoin d'être transformé. Par exemple, si un vendeur
préfère gérer uniquement les métadonnées ONIX pour l'affichage
Ensuite, ils devraient prétraiter les métadonnées
intégré dans un epub ou un pdf pour créer l'Onix. </p>
<p> Le processus de transformation des métadonnées n'est pas la portée
pour ce document et comment réconcilier
métadonnées lorsqu'elle est fournie sous plusieurs formes. Le
Guide suppose que tout traitement a déjà
s'est produit. Pour plus d'informations sur la cartographie entre
formats, reportez-vous au<a
href="https://w3c.github.io/publ-a11y/drafts/a11y-crosswalk-MARC/">Accessibilité
Propriétés
Cross-patauge </a>. </p>
</div>

<p> Le niveau suivant du diagramme représente le codage
Normes attendues pour chaque format. Ce guide
suppose que les métadonnées sont conformes à un
standard, sinon il serait difficile de
anticiper et traiter les informations entrantes pour
utilisateurs: </p>

<ul>
<li> Pour EPUB, la norme d'accessibilité EPUB
[[epub-a11y-11]] définit requis et recommandé
métadonnées pour des publications accessibles. Orientation
L'application de ces métadonnées se trouve dans l'Epub
Techniques d'accessibilité [[EPUB-A11Y-TECH-11]]. </li>
<li> Pour Onix, les caractéristiques d'accessibilité de la
La publication numérique correspondante est
exprimé en utilisant<a
href="https://ns.editeur.org/onix/en">code
Listes </a> [[ONIX]], et guide
sur l'application de ces valeurs est défini dans le
Remarque d'application <a
href="https://www.editeur.org/files/ONIX%203/APPNOTE%20Accessibility%20metadata%20in%20ONIX%20(advanced).pdf">Fourniture
métadonnées d'accessibilité dans ONIX (Advanced) </a>.
</li>
<li> Pour PDF, la norme PDF /UA
[[ISO14289-1]] [[ISO14289-2]] et<a
href="https://pdfa.org/wtpdf/">PDF bien marqué
Guide </a> Définissez comment décrire l'accessibilité
métadonnées. </li>
</ul>

<p> Sachant comment les métadonnées sont codées et comment elle est
Exprimé, la prochaine étape du traitement est d'utiliser
les algorithmes définis dans les techniques respectives
documents pour découvrir et traduire le
Informations sur les déclarations lisibles par l'homme. Ces
Les documents sont destinés principalement aux développeurs,
pour les aider avec le traitement spécifique du
GRAMMAIRS DE BUCKUP DE MÉTADATES. </p>

<p> Enfin, ce document est montré au dernier stade de
traitement, tel qu'il définit l'objectif de chaque
morceau de métadonnées plus en détail et priorise le
affichage pour les lecteurs. </p>
</section>

<section id="techniques">
<h3> Techniques d'affichage </h3>

<p> pour aider les développeurs à mettre en œuvre ces directives,
Des notes approfondies sont disponibles pour expliquer comment
Extraire les informations des métadonnées de l'industrie de l'édition
Normes. </p>

<p> Au moment de publier ce document, le disponible
Les techniques pour les normes de métadonnées sont: </p>

<ul>
<li>
<p><a href="../techniques/epub-metadata/index.html">Afficher les techniques pour les métadonnées d'accessibilité EPUB 2.0</a></p>
</li>
<li>
<p><a href="../techniques/onix-metadata/index.html">Techniques d'affichage pour les métadonnées d'accessibilité ONIX 2.0</a></p>
</li>
</ul>

<div class="note">
<p>Les éditeurs mettent à jour leurs enregistrements ONIX au besoin. Nous
s'attendre à ce que les métadonnées d'accessibilité "inconnues" peuvent être
initialement fourni mais peut changer comme plus
les informations deviennent disponibles. Pour cette raison,
Les implémenteurs doivent être prêts à mettre à jour le
Les métadonnées d'accessibilité comme de nouveaux flux ONIX sont fabriqués
disponible.</p>
</div>
</section>

<section id="terminology">
<h3>Terminologie </H3>

<p> Il y a plusieurs termes utilisés dans ces directives
doit être défini pour plus de clarté: </p>

<dl>
<dt> <dfn> Publication numérique </dfn> </dt>
<dd>
<p> Le terme publication numérique est utilisé dans ce
document pour se référer aux publications produites dans
n'importe quel nombre de formats numériques. Numérique
Les publications ne se limitent pas aux livres, mais
englober tout travail écrit, visuel ou audio
distribué et lu sous forme numérique. </p>
<p> Certains exemples de publications numériques incluent
Ebooks, livres audio, mangas, bandes dessinées,
revues, manuels numériques, livres d'images et
Livres d'image des enfants avec l'accompagnement
Audio. Les formats dans lesquels ils viennent comprennent epub,
PDF et livres de parole numériques (DTB). </p>
</dd>

<dt> <dfn> Braille dynamique </dfn> </dt>
<dd>
<p> Le terme braille dynamique est utilisé pour indiquer
Contenu généré en braille à la volée,
par opposition au braille numérique préformaté
formats. Ce rendu dynamique de
Le contenu est parfois appelé électronique
braille ou braille rafraîchissable. </p>

<p> Le braille dynamique est généralement rendu sur un
Séparer l'appareil du système de lecture, un
avec
épingles pop-up pour présenter le braille sur un tactile
écran. Ces appareils, communément appelés
Des écrans de braille rafraîchables peuvent être attachés à
un ordinateur personnel, ou ils peuvent être un
preneur de notes polyvalent autonome avec un
Affichage en braille rafraîchissable. </p>
</dd>

<dt> <dfn> Lire la parole à haute voix </dfn> </dt>
<dd>
<p> Le terme discours à haute voix est utilisé pour désigner
Contenu généré dans la parole synthétique
À la volée, par opposition à la narration préenregistrée.
Lire la fonctionnalité à haute voix est souvent une fonctionnalité
de systèmes de lecture, mais peuvent être fournis par un
technologie d'assistance séparée. </p>
</dd>

<dt> <dfn> Système de lecture </dfn> </dt>
<dd>
<p> Toutes les publications numériques nécessitent un système de lecture
Pour présenter la publication à l'utilisateur final.
Les systèmes de lecture peuvent être des applications qui s'exécutent sur un intelligent
téléphone ou tablette. Il existe des systèmes de lecture qui
sont des applications qui s'exécutent sur des ordinateurs personnels.
Il existe également des systèmes de lecture qui sont
intégré dans des appareils dédiés consacrés à un
but unique, pour présenter une publication.
Il y a même des compétences qui fonctionnent sur des haut-parleurs intelligents
qui peut être considéré comme des systèmes de lecture. </p>
</dd>
</dl>
</section>
</section>
<section id="meta-display">
<h2>Affichage de métadonnées</h2>

<section id="a11y-section">
<h3>Section d'accessibilité</h3>

<section id="a11y-display-hd">
<h4>Afficher la tête </h4>

<p> lors de la présentation des métadonnées d'accessibilité fournies par le
éditeur, il est suggéré que la section est
introduit en utilisant des termes tels que «réclamation» ou
"Déclarations" (par exemple, "réclamations d'accessibilité"). </p>

<p> Le cap doit être clairement transmis à
l'utilisateur final que les informations proviennent directement du
éditeur et représente l'accessibilité
informations que l'éditeur a l'intention de communiquer. </p>
</section>

<section id="rec-fields">
<h4>Champs d'affichage recommandés </H4>

<p> Il existe plusieurs informations qui sont au cœur de la description de l'accessibilité d'une publication numérique: </p>

<ul>
<li> Les personnes qui ont besoin d'ajuster la présentation visuelle
veulent savoir s'ils peuvent agrandir le texte,
ce qui est essentiel pour les utilisateurs à basse vision. Les gens avec
La dyslexie doit pouvoir sélectionner la police
et ajustez le premier plan, l'arrière-plan et la ligne
espacement et longueur. Personnes à faible vision ou à la dyslexie
représentent le plus grand pourcentage de la
Population imprimée. </li>
<li> Les personnes qui utilisent un lecteur d'écran doivent savoir si tout le contenu du titre leur sera accessible. Le texte de la publication doit être disponible pour conversion en discours ou en braille. De plus, lorsque les images ont des descriptions de texte (texte alt), ce qui l'indiquera dans les métadonnées permettra aux utilisateurs de savoir qu'ils ne manqueront pas les informations essentielles. Les utilisateurs aveugles bénéficieront considérablement de ces informations, tout comme les individus qui utiliseront la fonctionnalité à haute voix dans les systèmes de lecture. </li>
<li> les personnes qui sélectionnent du matériel pour le public
Des institutions telles que les bibliothèques ou les écoles ont besoin
savoir si le contenu est conforme à
Normes. </li>
</ul>

<p> c'est pourquoi ces directives recommandent que les éléments suivants<a
href="#a11y-display-fields">accessibility fields</a> should be
displayed:</p>

<ul>
<li> <a href="#ways-of reading"> façons de lire </a> -en particulier le
<a href="#visual-ajustements"> ajustements visuels </a>
et <a href="#supports-non-visuelle Reading"> Prise en charge de la lecture non visuelle </a> Instructions </li>
<li> <a href="#conformance-group"> conformance </a> </li>
</ul>

<p> Les autres champs de métadonnées fournissent des détails supplémentaires sur des fonctionnalités ou des lacunes spécifiques dans
une publication. Ils donnent aux gens les informations dont ils ont besoin pour faire un choix éclairé lors de la sélection
une publication numérique particulière. </p>
</section>

<section id="field-order">
<h4> Afficher l'ordre du champ </h4>

<p> Les implémenteurs peuvent choisir l'ordre dans lequel ils préfèrent afficher le <a
href="#a11y-display champs"> champs de métadonnées d'accessibilité </a>. </p>

<p> De plus, bien que les champs de métadonnées de ce document soient nommés, il n'est pas nécessaire que
Les implémenteurs utilisent ces noms comme en-têtes de champ. Les implémenteurs peuvent utiliser une alternative
Noms de champ s'ils avaient plus de sens dans leur contexte d'affichage. </p>
</section>
<section id="additional-a11y-meta">
<h4> Métadata d'accessibilité supplémentaire </h4>

<p> Bien que ce document présente des exemples de métadonnées importantes qui devraient être présentes
Dans un large éventail de publications, les schémas de métadonnées disponibles peuvent soutenir les déclarations sur de nombreux
Autres fonctionnalités. </p>

<p> les documents de techniques <a href="##> Documents </a> Décrivez comment diffuser des informations supplémentaires non répertoriées dans ce
document. De plus, les implémenteurs peuvent choisir d'afficher des métadonnées qui ne sont pas couvertes par
ce document ou les techniques. </p>
</section>

<section id="missing-metadata">
<h4> Métadonnées manquantes </h4>

<p> Lorsqu'aucune métadonnée d'accessibilité n'est fournie par l'éditeur, il est préférable de
Évitez de faire une déclaration négative qui pourrait leur être attribuée (par exemple, indiquant
On ne sait pas si une fonctionnalité est disponible pourrait être mal interprétée comme l'éditeur
disant qu'ils ne sont pas sûrs). La déclaration neutre "aucune information n'est disponible"
affiché pour ce cas. </p>
<p> Dans certains cas, le distributeur peut ne pas être autorisé à afficher les déclarations que l'éditeur n'a pas faites.
Cacher de telles sections est acceptable dans ces cas. </p>
</section>
</section>

<section id="alt-statements">
<h3>Alternative statements</h3>
<p> bien que les instructions d'affichage répertoriées dans ce document et dans les techniques <a href="#techniques">
Les documents </a> sont recommandés pour une utilisation et ont été traduits pour soutenir la localisation,
Les implémenteurs peuvent préférer utiliser des libellés différents dans certaines situations. </p>

<p> Ce document n'empêche pas les implémenteurs d'utiliser un phrasé alternatif, cependant
Tout écart doit être fait avec prudence. Les phrases définies dans ce document ont abouti
D'après de nombreuses discussions entre les professionnels de l'accessibilité ainsi que les commentaires des utilisateurs. </p>

<p> Si la cause du libellé alternatif est due à des problèmes de traduction, les exécutants sont encouragés
à <a href = "https://github.com/w3c/publ-a11y/issues/"> Techniques Documents </a> Pour la correction. </p>
</section>

<section id="non-a11y-meta">
<h3> Métadonnées non accessibles </h3>

<p> Toutes les métadonnées utilisées pour déterminer l'accessibilité d'une publication sont strictement classées comme
métadonnées d'accessibilité. Les détails du produit, par exemple, fournissent des informations importantes sur le
utilisabilité d'un ebook par rapport aux besoins spécifiques des utilisateurs. </p>

<p> En particulier, les informations suivantes doivent toujours être affichées: </p>

<ul>
<li> Format de fichier (epub 2 ou 3, pdf, mp3, livre audio, etc.) -
Le format de fichier donne une forte indication de
Accessibilité: un PDF ne permet pas la typographie
Modification, Epub 2 est
déprécié, une navigation de la page d'assistance EPUB 3 et
meilleure sémantique structurelle; un livre audio au format MP3
sera moins structuré qu'un livre audio, etc. </li>

<li> Mesure de protection ou absence de celle-ci -le
La mesure de protection peut bloquer l'assistance
Des technologies telles que les lecteurs d'écran. En outre,
De nombreux dispositifs de refus spécifiques tels que les lecteurs de Daisy
ou les preneurs de notes en braille ne sont pas équipées pour lire
Fichiers cryptés. </li>

<li> Nom de la maison d'édition -le nom du
La maison d'édition peut mettre en évidence le
efforts qu'il a faits en termes de
accessibilité. </li>

<li> Langue principale du contenu -la langue principale
du contenu permet aux lecteurs de
Soyez convaincu qu'ils pourront lire
avec leur technologie d'assistance qui utilise
voix synthétisée ou braille correspondante
table de traduction
pour la langue. </li>
</ul>

<p> Ces métadonnées ne doivent pas être incluses dans le cadre de la section d'accessibilité; ça seulement
doit être mis à la disposition des utilisateurs de l'affichage des métadonnées pour une publication. </p>
</section>
</section>
<section id="a11y-display-fields">
<h2> Champs d'affichage d'accessibilité </h2>
<section id="ways-of-reading">
<h3 data-localization-id="ways-of-reading-title">Façons de lire </h3>

<section id="visual-adjustments">
<h4> Ajustements visuels </H4>

<div class="note">
<p> Ce champ d'affichage doit être rendu même
S'il n'y a pas de métadonnées. </p>
</div>

<p> indique si les utilisateurs peuvent modifier l'apparence du texte
et la disposition de la page selon le
possibilités offertes par le système de lecture. </p>

<p> Ce champ d'affichage répond si les ajustements visuels sont
possible, non possible ou inconnu. </p>

<p> lecteurs ayant des déficiences visuelles ou des troubles cognitifs
besoin de la capacité de changer la couleur de
texte et son arrière-plan (contraste), la famille des polices et
taille de police utilisée, ainsi que l'espacement entre
lettres, mots, phrases ou paragraphes. </p>

<p> Connaître
qu'une publication peut refléter pour s'adapter au
La zone d'affichage du système de lecture n'est pas suffisante pour savoir
que les modifications de la police, de l'espacement et
Les couleurs sont possibles ou que les modifications ne provoqueront pas
Autres problèmes de lisibilité (par exemple, le texte étant
coupé par son conteneur). </p>
<section id="va-statements">
<h5> afficher les instructions </h5>

<p> Les instructions descriptives et compactes pour l'ajustement visuel sont les suivantes. </p>

<dl>
<dt> Si l'affichage est modifiable: </dt>
<dd>
<p data-localization-id="ways-of-reading-visual-adjustments-modifiable"
data-localization-mode="compact">Apparence
peut être modifié </p>
<p data-localization-id="ways-of-reading-visual-adjustments-modifiable"
data-localization-mode="descriptive">L'apparition du texte et de la disposition de la page peut
être
modifié en fonction des capacités de
Le système de lecture (famille et police
taille,
espaces entre paragraphes, phrases, mots,
et des lettres, ainsi que la couleur de l'arrière-plan
et texte) </p>
</dd>

<dt> Si l'affichage n'est pas modifiable: </dt>
<dd>
<p data-localization-id="ways-of-reading-visual-adjustments-unmodifiable"
data-localization-mode="compact">Apparence
ne peut pas être modifié </p>
<p data-localization-id="ways-of-reading-visual-adjustments-unmodifiable"
data-localization-mode="descriptive">Texte
et la mise en page ne peut pas être modifiée comme le
L'expérience de lecture est proche d'une impression
version, mais les systèmes de lecture peuvent encore
Fournir des options de zoom </p>
</dd>

<dt> Si aucune métadonnée n'est fournie: </dt>
<dd>
<p data-localization-id="ways-of-reading-visual-adjustments-unknown"
data-localization-mode="compact">Aucune information sur la modification de l'apparence n'est disponible </p>
<p data-localization-id="ways-of-reading-visual-adjustments-unknown"
data-localization-mode="descriptive">
Aucune information sur la modification de l'apparence n'est disponible </p>
</dd>
</dl>
</section>

<section id="va-techniques">
<h5> Afficher les techniques de support des ajustements visuels </h5>

<p> Les techniques spécifiques pour répondre à ce principe sont
défini dans les documents suivants: </p>

<ul>
<li> <A
href = "../Techniques /EPUB-Metadata /index.html # Visual-Adjustments"> Epub
Accessibilité:
Ajustements visuels </a> </li>
<li> <A
href = "../Techniques /Onix-Metadata /index.html # Visual-Adjustments"> ONIX:
Visuel
Ajustements </a> </li>
</ul>
</section>
</section>

<section id="supports-nonvisual-reading">
<h4> Prise en charge de la lecture non visuelle </h4>

<div class="note">
<p> Ce champ d'affichage doit être rendu même
S'il n'y a pas de métadonnées. </p>
</div>

<p> indique si tout le contenu requis pour la compréhension
peut être consommé dans le texte et est donc
Disponible pour les systèmes de lecture avec [= lire à haute voix Speech =]
ou [= dynamique braille =] capacités. </p>

<p> Ce champ d'affichage répond si une lecture non visuelle est possible,
non possible, ou inconnu. </p>
<p> publications numériques avec contenu essentiel inclus dans
forme non textuelle (comme les images, les photographies, les graphiques,
tableaux ou
Les équations présentées comme des images, des vidéos, etc.) doivent
Inclure des alternatives textuelles pour s'assurer que les utilisateurs
lire avec d'autres sens que la vue (principalement auditif
et tactile) ont accès à la même
informations en tant que lecteurs visuels. Ces textuels
Les alternatives peuvent inclure du texte alt sur les images, étendu
descriptions,
transcriptions, légendes, etc. en fonction de la nature de
le contenu non visuel. </p>

<section id="nv-statements">
<h5> afficher les instructions </h5>

<p> Les instructions descriptives et compactes pour la lecture non visuelle sont les suivantes. </p>

<dl>

<dt> Si tout le contenu est lisible sous forme de texte: </dt>
<dd>
<p data-localization-id="ways-of-reading-nonvisual-reading-readable"
data-localization-mode="compact">Lisible en lecture à haute voix ou en braille dynamique</p>
<p data-localization-id="ways-of-reading-nonvisual-reading-readable"
data-localization-mode="descriptive">Tous les contenus peuvent être lus comme lus à haute voix ou en braille dynamique</p>
</dd>

<dt>Si tout le contenu n'est pas lisible sous forme de texte:</dt>
<dd>
<p data-localization-id="ways-of-reading-nonvisual-reading-not-fully"
data-localization-mode="compact">Pas entièrement lisible en lecture à haute voix ou en braille dynamique</p>
<p data-localization-id="ways-of-reading-nonvisual-reading-not-fully"
data-localization-mode="descriptive">Tous les contenus ne seront pas lisibles en tant que discours à haute voix ou braille dynamique </p>
</dd>

<dt> Si le contenu ne peut pas être lu sous forme de texte: </dt>
<dd>
<p data-localization-id="ways-of-reading-nonvisual-reading-none"
data-localization-mode="compact">Pas lisible en lisant à haute voix ou en braille dynamique</p>
<p data-localization-id="ways-of-reading-nonvisual-reading-none"
data-localization-mode="descriptive">Le contenu n'est pas lisible comme lus à haute voix ou en braille dynamique </p>
</dd>

<dt> Si aucune métadonnée n'est fournie: </dt>
<dd>
<p data-localization-id="ways-of-reading-nonvisual-reading-no-metadata"
data-localization-mode="compact">Aucune information sur la lecture non visuelle n'est disponible</p>
<p data-localization-id="ways-of-reading-nonvisual-reading-no-metadata"
data-localization-mode="descriptive">Aucune information sur la lecture non visuelle n'est disponible</p>
</dd>

<dt> Si des alternatives de texte sont fournies: </dt>
<dd>
<p data-localization-id="ways-of-reading-nonvisual-reading-alt-text"
data-localization-mode="compact">A un texte alternatif</p>
<p data-localization-id="ways-of-reading-nonvisual-reading-alt-text"
data-localization-mode="descriptive">A des descriptions de texte alternatives pour les images</p>
</dd>
</dl>
</section>

<section id="nv-techniques">
<h5> Afficher les techniques de prise en charge de la prise en charge de la lecture non visuelle </h5>

<p> Les techniques spécifiques pour répondre à ce principe sont
défini dans les documents suivants: </p>

<ul>
<li> <A
href = "../Techniques /ePub-Metadata /index.html # supports de non-visualité"> epub
Accessibilité: prise en charge de non visuelle
lecture </a> </li>
<li> <A
href = "../Techniques /ONIX-Metadata /index.html # supports-Nonvisual Reading"> ONIX:
Soutien
pour la lecture non visuelle </a> </li>
</ul>
</section>
</section>

<section id="prerecorded-audio">
<h4> Audio préenregistré </H4>

<div class="note">
<p> Ce champ d'affichage peut être masqué si les métadonnées sont
manquant. Alternativement, il peut être indiqué que
<span
data-localization-id="ways-of-reading-prerecorded-audio-no-metadata"
data-localization-mode="descriptive">
Aucune information sur l'audio préenregistré n'est disponible </span>.
</p>
</div>

<p>Indicates the presence of prerecorded audio and specifies if this audio is standalone (an audiobook), is an alternative to the text (synchronized text with audio playback), or is complementary audio (portions of audio, (e.g., reading of a poème). </p>

<p> Les livres audio créés pour une utilisation traditionnelle fournissent une importance importante
accès pour de nombreux utilisateurs handicapés même
bien qu'ils ne soient pas accessibles à tous. Au fur et à mesure qu'ils grandissent
popularité, les livres audio peuvent en fournir plus
Options d'accessibilité à l'avenir. </p>

<p> Certaines publications fournissent audio préenregistré avec du texte
synchronisation. Utilisateurs avec entendre
Les déficiences peuvent toujours accéder au contenu complet de ces
livres. </p>

<section id="prerecorded-audio-statements">
<h5> afficher les instructions </h5>

<p> Les instructions descriptives et compactes pour l'audio préenregistré sont les suivantes. </p>

<dl>
<dt> Si la publication est un livre audio préenregistré: </dt>
<dd>
<p data-localization-id="ways-of-reading-prerecorded-audio-only"
data-localization-mode="compact">Audio préenregistré uniquement</p>
<p data-localization-id="ways-of-reading-prerecorded-audio-only"
data-localization-mode="descriptive">
Livre audio sans alternative de texte </p>
</dd>

<dt> S'il y a un audio préenregistré synchronisé avec le texte: </dt>
<dd>
<p data-localization-id="ways-of-reading-prerecorded-audio-synchronized"
data-localization-mode="compact">Audio préenregistré synchronisé avec du texte</p>
<p data-localization-id="ways-of-reading-prerecorded-audio-synchronized"
data-localization-mode="descriptive">Tout
Le contenu est disponible en audio préenregistré
synchronisé avec le texte </p>
</dd>

<dt> S'il y a des clips audio préenregistrés: </dt><dd>
<p data-localization-id="ways-of-reading-prerecorded-audio-complementary" data-localization-mode="compact">Clips audio préenregistrés </p>
<p data-localization-id="ways-of-reading-prerecorded-audio-complementary" data-localization-mode="descriptive">Les clips audio préenregistrés sont intégrés dans le contenu </p>
</dd>

<dt> Si aucune métadonnée n'est fournie: </dt>
<dd>
<p data-localization-id="ways-of-reading-prerecorded-audio-no-metadata"
data-localization-mode="compact">
Aucune information sur l'audio préenregistré n'est disponible </p>
<p data-localization-id="ways-of-reading-prerecorded-audio-no-metadata"
data-localization-mode="descriptive">
Aucune information sur l'audio préenregistré n'est disponible </p>
</dd>
</dl>
</section>

<section id="prerecorded-audio-techniques">
<h5> Afficher les techniques de support audio préenregistré
</h5>
<p> Les techniques spécifiques pour répondre à ce principe sont
défini dans les documents suivants: </p>
<ul>
<li><a
href="../techniques/epub-metadata/index.html#prerecorded-audio">Époule
Accessibilité: audio préenregistré </a> </li>
<li> <A
href="../techniques/onix-metadata/index.html#prerecorded-audio">ONIX: Audio préenregistré </a> </li>
</ul>
</section>
</section>

<section id="wr-examples">
<h4> Exemples </h4>
<aside class="example" title="Publication with accessible ways of reading">
<p> L'exemple suivant montre les instructions descriptives et compactes qui afficheraient
Pour une publication avec un affichage modifiable, qui est compatible avec la lecture non visuelle,
Et cela a synchronisé l'audio préenregistré avec le texte. </p>

<dl>
<dt> Affichage compact </dt>
<dd>
<p class="ex-hd" data-localization-id="ways-of-reading-title">Façons de lire</p>
<p data-localization-id="ways-of-reading-visual-adjustments-modifiable"
data-localization-mode="compact">L'apparence peut être modifiée</p>
<p data-localization-id="ways-of-reading-nonvisual-reading-readable"
data-localization-mode="compact">Lisible dans
Lisez à haute voix ou en braille dynamique </p>

<p data-localization-id="ways-of-reading-prerecorded-audio-synchronized"
data-localization-mode="compact">Audio préenregistré synchronisé avec le texte </p>
<p data-localization-id="ways-of-reading-nonvisual-reading-alt-text"
data-localization-mode="compact">A un texte alternatif </p>
</dd>

<dt> Affichage descriptif </dt>
<dd>
<p class="ex-hd" data-localization-id="ways-of-reading-title">Façons de lire </p>
<p data-localization-id="ways-of-reading-visual-adjustments-modifiable"
data-localization-mode="descriptive">L'apparition du texte et de la disposition de la page peut être
modifié en fonction des capacités de
Le système de lecture (famille des polices et taille de police,
espaces entre paragraphes, phrases, mots,
et des lettres, ainsi que la couleur de l'arrière-plan
et texte) </p>
<p data-localization-id="ways-of-reading-nonvisual-reading-readable"
data-localization-mode="descriptive">Tous les contenus peuvent être lus comme lus à haute voix ou en braille dynamique </p>

<p data-localization-id="ways-of-reading-prerecorded-audio-synchronized"
data-localization-mode="descriptive">Tout le contenu est disponible en audio préenregistré synchronisé avec du texte </p>
<p data-localization-id="ways-of-reading-nonvisual-reading-alt-text"
data-localization-mode="descriptive">A des descriptions de texte alternatives pour les images </p>
</dd>
</dl>
</aside>
</section>
</section>
<section id="conformance-group">
<h3 data-localization-id="conformance-title">Conformité </h3>

<div class="note">
<p> Ce champ d'affichage doit être rendu même
S'il n'y a pas de métadonnées. </p>
</div>

<p> identifie si la publication numérique prétend se rencontrer
conformité reconnue internationalement
Normes d'accessibilité. </p>

<p> Les métadonnées de conformité utilisent souvent la terminologie que la plupart
Les gens ne comprendront pas, et donc <a
href="#conf-statement"> instructions simples </a> devrait
être fourni lors de l'accessibilité à epub et
Les niveaux de WCAG sont identifiés. </p>

<p> Si la publication n'inclut pas de réclamation de conformité,
L'énoncé doit indiquer qu'aucune information n'est disponible. </p>

<p> Dans la plupart des cas, les gens voudront en savoir plus sur le
conformité et certification de la
publication. L'organisation de certification doit être
identifié avec leurs références et
placé immédiatement après la déclaration de conformité. </p>

<section id="conf-statements">
<h4>Afficher les instructions </h4>

<div class="note">
<p> Certaines déclarations de conformité intègrent des métadonnées de publication. Pour indiquer où
Ce texte sera inséré, les instructions incluent les variables d'espace réservées. Ces
Les espaces réservés sont identifiés en étant enfermés dans des supports d'angle (par exemple,
<span class="placeholder"> <placeholder> </span>). </p>
</div>

<div class="note">
<p> Toutes les instructions de conformité n'ont pas de formes compactes et descriptives. Dans ces cas,
La même chaîne est utilisée pour les deux. </p>
</div>

<section id="conformance-general">
<h5> CONFORMANCE GÉNÉRALE </H5>

<dl>
<DT> Si la publication répond aux conditions d'accessibilité minimales: </dt>
<dd>
<p data-localization-id="conformance-a"
data-localization-mode="compact">Cette publication répond à une accessibilité minimale
Normes </p>
<p data-localization-id="conformance-a"
data-localization-mode="descriptive">La publication contient une conformité
Déclaration selon laquelle il répond à l'accessibilité EPUB et au niveau WCAG 2 A norme </p>
</dd>
<DT> Si la publication répond aux conditions d'accessibilité largement acceptées: </dt>
<dd>
<p data-localization-id="conformance-aa"
data-localization-mode="compact">Cette publication répond à l'accessibilité acceptée
Normes </p>
<p data-localization-id="conformance-aa"
data-localization-mode="descriptive">La publication contient une conformité
Déclaration selon laquelle il répond à l'accessibilité EPUB et à la norme AA de niveau 2 WCAG </p>
</dd>
<DT> Si la publication dépasse les conditions d'accessibilité acceptées: </dt>
<dd>
<p data-localization-id="conformance-aaa"
data-localization-mode="compact">Cette publication dépasse l'accessibilité acceptée
Normes </p>
<p data-localization-id="conformance-aaa"
data-localization-mode="descriptive">La publication contient une conformité
Déclaration selon laquelle il répond à l'accessibilité EPUB et à la norme AAA de niveau WCAG 2 </p>
</dd>

<dt> Si aucune métadonnée n'est fournie: </dt>
<dd>
<p data-localization-id="conformance-no"
data-localization-mode="compact">Aucune information n'est disponible </p>
<p data-localization-id="conformance-no"
data-localization-mode="descriptive"> Aucune information n'est disponible </p>
</dd>
<DT> Si un nom de certificateur est fourni: </dt>
<dd>
<p><span
data-localization-id="conformance-certifier"
data-localization-mode="compact">Le
La publication a été certifiée par </span>
<span class="placeholder"> <nom du certificateur> </span> </p>
</dd>
<DT> Si le certificateur a un diplôme: </dt>
<dd>
<p><span
data-localization-id="conformance-certifier-credentials"
data-localization-mode="compact">The certifier's credential is </span>
<span class="placeholder"><certifier credential></span></p>
</dd>
</dl>
</section>

<section id="detailed-conformance-information">
<h5> Conformance détaillée </h5>

<p> Les informations suivantes peuvent être placées dans une section
qui montre les détails de la conformité
informations. </p>

<dl>
<DT> Si une affirmation de conformité détaillée est faite: </dt>
<dd>
<p data-localization-mode="compact">
<span data-localization-id="conformance-claim"
data-localization-mode="compact">Ce
La publication prétend rencontrer </span>

Accessibilité de l'EPUB
<span class="placeholder"> <1.x> </span>

Wcag
<span class="placeholder"> <2.x> </span>

Niveau
<span class="placeholder"> <a ou aa ou aaa> </span>
</p>
<p data-localization-mode="descriptive">
<span data-localization-id="conformance-claim"
data-localization-mode="descriptive">This
La publication prétend rencontrer </span>

Accessibilité de l'EPUB
<span class="placeholder">&lt;1.X&gt;</span>
Lignes directrices sur l'accessibilité du contenu Web (WCAG)
<span class="placeholder"> <2.x> </span>

Niveau
<span class="placeholder"> <a ou aa ou aaa> </span>
</p>

<div class="note">
<p> Les espaces réservés de ces chaînes permettent l'affichage de chaque version du
Norme respective. Par exemple, les instructions descriptives pour WCAG 2 seraient: </p>
<ul>
<li data-localization-id="conformance-wcag-2-0"
data-localization-mode="descriptive">Lignes directrices sur l'accessibilité du contenu Web (WCAG) 2.0 </li>
<li data-localization-id="conformance-wcag-2-1"
data-localization-mode="descriptive">Lignes directrices sur l'accessibilité du contenu Web (WCAG) 2.1 </li>
<li data-localization-id="conformance-wcag-2-2"
data-localization-mode="descriptive">Lignes directrices sur l'accessibilité du contenu Web (WCAG) 2.2 </li>
</ul>
</div>
</dd>
<DT> Si la date de certification est fournie: </dt>
<dd>
<p>
<span data-localization-id="conformance-certification-info"
data-localization-mode="compact">Le
La publication a été certifiée sur </span>
<span class="placeholder">&lt;Date de certification&gt;</span></p>
</dd>
<DT> Si le certificateur fournit un rapport d'accessibilité: </dt>
<dd>
<p><span data-localization-id="conformance-certifier-report"
data-localization-mode="compact">Pour
Plus d'informations se réfèrent au
Rapport du certificateur </span> </p>
</dd>
</dl>
</section>
</section>

<section id="conf-examples">
<h4>Exemples</h4>

<aside class="example"
title="Conformance statement that claims to meet accepted accessibility standards followed by detailed conformance information">

<dl>
<dt> Affichage compact </dt>
<dd>
<p class="ex-hd" data-localization-id="conformance-title">Conformité </p>
<p data-localization-id="conformance-aa"
data-localization-mode="compact">Ce
La publication répond aux normes d'accessibilité acceptées </p>
<p>
<span
data-localization-id="conformance-certifier"
data-localization-mode="compact">Le
La publication a été certifiée par </span>
Test d'accessibilité de Foo
</p>
<p>
<span
data-localization-id="conformance-certifier-credentials"
data-localization-mode="compact">L'identification du certificateur est </span> "Enterprise
Note d'accessibilité "
</p>

<p class="ex-hd" data-localization-id="conformance-details-title">Informations de conformité détaillées </p>
<p>
<span
data-localization-id="conformance-claim">This
publication claims to meet</span>Ce
La publication prétend rencontrer </span>
<span-localization-id="conformance-epub-accessibility-1-1">Époule
Accessibilité
1.1 </pan>
<span
data-localization-id="conformance-wcag-2-1"
data-localization-mode="descriptive">Web
Lignes directrices sur le contenu de l'accessibilité (WCAG)
2.1 </pan>
<span
data-localization-id="conformance-level-aa">Niveau
Aa </pan>
</p>
<p><span data-localization-id="conformance-certification-info">Le
La publication a été certifiée sur </span>
2021-09-07 </p>
<p><span data-localization-id="conformance-certifier-report">Pour
Plus d'informations se réfèrent au
<a
href="http://www.example.com/a11y/report/9780000000001">certifier's
report</a></span>
</p>
</dd>

<dt> Affichage descriptif </dt><dd>
<p class="ex-hd" data-localization-id="conformance-title">Conformité</p>
<p data-localization-id="conformance-aa"
data-localization-mode="compact">La publication contient une déclaration de conformité
qu'il répond à l'accessibilité EPUB et à la norme AA de niveau 2 WCAG. </p>
<p>
<span
data-localization-id="conformance-certifier"
data-localization-mode="compact">Le
La publication a été certifiée par </span>
Test d'accessibilité de Foo
</p>
<p>
<span
data-localization-id="conformance-certifier-credentials"
data-localization-mode="compact">L'identification du certificateur est </span> "Enterprise
Note d'accessibilité "
</p>

<p class="ex-hd" data-localization-id="conformance-details-title">
Informations de conformité détaillées </p>
<p>
<span
data-localization-id="conformance-claim">Ce
La publication prétend rencontrer </span>
<span
data-localization-id="conformance-epub-accessibility-1-1">Époule
Accessibilité
1.1 </pan>
<span
data-localization-id="conformance-wcag-2-1"
data-localization-mode="descriptive">Web
Lignes directrices sur le contenu de l'accessibilité (WCAG)
2.1 </pan>
<span
data-localization-id="conformance-level-aa">Niveau
Aa </pan>
</p>
<p><span data-localization-id="conformance-certification-info">Le
La publication a été certifiée sur </span>
2021-09-07 </p>
<p><span data-localization-id="conformance-certifier-report">Pour
Plus d'informations se réfèrent au
<a
href="http://www.example.com/a11y/report/9780000000001">certifier's
report</a></span>
</p>
</dd>
</dl>
</aside>

<aside class="example"
title="Missing a conformance statement">
<p class="ex-hd" data-localization-id="conformance-title">Conformité</p>
<p data-localization-id="conformance-no"
data-localization-mode="compact">Aucune information n'est disponible </p>
<p class="note"> Il n'y a pas de différence entre les sorties compactes et descriptives dans ce cas. </p>
</roprows>
</section>

<section id="conf-techniques">
<h4> Afficher les techniques de support de conformité </H4>
<p> Les techniques spécifiques pour répondre à ce principe sont
défini dans les documents suivants: </p>

<ul>
<li><a
href="../techniques/epub-metadata/index.html#conformance-group">Époule
Accessibilité:
Conformité </a> </li>

<li><a
href="../techniques/onix-metadata/index.html#conformance-group">Onix:
Conformité </a> </li>

</ul>
</section>
</section>
<section id="navigation">
<h3 data-localization-id="navigation-title">Navigation</h3>

<div class="note">
<p> Ce champ d'affichage peut être masqué si les métadonnées sont
manquant. Alternativement, il peut être indiqué que
<span data-localization-id="navigation-no-metadata"
data-localization-mode="descriptive">Aucune information n'est disponible </span>.
</p>
</div>

<p> identifie les fonctionnalités de navigation incluses dans le
publication. </p>

<p> naviguer dans une publication numérique à travers un tableau de
Contenu, un index, par titres ou par allez à la page
Les raccourcis sont importants pour permettre à l'utilisateur de facilement
accéder à chaque partie de la publication numérique. Ces
Les fonctionnalités sont
à la fois essentiels à l'accessibilité et importants pour tous
utilisateurs lisant des publications. Donc,
communiquer clairement à l'utilisateur quelle navigation
Les fonctionnalités sont disponibles dans la publication est
important pour permettre une sélection de titres appropriée. </p>

<p> Notez que les directives d'accessibilité du contenu Web (WCAG)
2.1 La norme nécessite que <q> plus d'un
Way est disponible pour localiser une page Web dans un ensemble
de pages Web </Q> (<cite> <a
href = "https://www.w3.org/tr/wcag21/#multiple-ways"> Succès
Critère 2.4.5 multiple
Façons </a> </cite>). </p>
<div class="note"> <p> Bien que non requis, si cela est disponible, il peut être utile d'identifier les informations bibliographiques sur la source de pause de page identifiée dans les métadonnées de la publication numérique. Avoir suffisamment d'informations pour identifier la source d'impression assurerait que les étudiants et les éducateurs que la version numérique qu'ils utilisent sont correctement associés à la version imprimée utilisée en classe. L'objectif est de faire en sorte que la fonction aller à la page porte l'utilisateur numérique à la même page que l'utilisateur de la version imprimée.
</p> </div>

<section id="nav-statements">
<h4> afficher les instructions </h4>

<p> Les instructions descriptives et compactes pour la navigation sont les suivantes. </p>

<dl>
<dt> Si une table des matières est fournie: </dt>
<dd>
<p data-localization-id="navigation-toc"
data-localization-mode="compact">Tableau
de contenu </p>
<p data-localization-id="navigation-toc"
data-localization-mode="descriptive">Tableau
de contenu à tous les chapitres du texte via
liens </p>
</dd>

<dt>Si des index (ES) sont fournis: </dt>
<dd>
<p data-localization-id="navigation-index"
data-localization-mode="compact">Index</p>
<p data-localization-id="navigation-index"
data-localization-mode="descriptive">Index
avec des liens vers les entrées référencées </p>
</dd>

<dt>Si une navigation structurelle est fournie: </dt>
<dd>
<p data-localization-id="navigation-structural"
data-localization-mode="compact">Rubriques</p>
<p data-localization-id="navigation-structural"
data-localization-mode="descriptive">Des éléments tels que des titres, des tables, etc. pour
Navigation structurée </p>
</dd>
<dt> si la navigation de page est fournie: </dt>
<dd>
<p data-localization-id="navigation-page-navigation"
data-localization-mode="compact">Allez sur page </p>
<p data-localization-id="navigation-page-navigation"
data-localization-mode="descriptive">Liste des pages pour accéder aux pages de l'impression
Version source </p>
</dd>

<dt> Si aucune métadonnée n'est fournie: </dt>
<dd>
<p data-localization-id="navigation-no-metadata"
data-localization-mode="compact">Aucune information n'est disponible </p>
<p data-localization-id="navigation-no-metadata"
data-localization-mode="descriptive">Aucune information n'est disponible </p>
</dd>
</dl>
</section>

<section id="nav-examples">
<h5> Exemples </h5>

<aside class="example" title="Publication with some navigation features">
<p> L'exemple suivant montre les instructions descriptives et compactes qui afficheraient
pour une publication avec une table des matières et une navigation de page. </p>

<dl>
<dt> Affichage compact </dt>
<dd>
<p class="ex-hd" data-localization-id="navigation-title">Navigation</p>
<ul>
<li data-localization-id="navigation-toc"
data-localization-mode="compact">Tableau de contenus</li>
<li data-localization-id="navigation-page-navigation"
data-localization-mode="compact">Aller à la page</li>
</ul>
</dd>

<dt> Affichage descriptif </dt>
<dd>
<p class="ex-hd" data-localization-id="navigation-title">Navigation</p>
<ul>
<li data-localization-id="navigation-toc"
data-localization-mode="descriptive">Table des matières à tous
Chapitres du texte via des liens </li>
<li data-localization-id="navigation-page-navigation"
data-localization-mode="compact">Liste de pages pour accéder aux pages de
la version de la source d'impression </li>
</ul>
</dd>
</dl>
</aside>
</section>

<section id="nav-techniques">
<h4> Affichage des techniques de support de navigation </h4>

<p> Les techniques spécifiques pour répondre à ce principe sont
défini dans les documents suivants: </p>

<ul>
<li><a
href="../techniques/epub-metadata/index.html#navigation">Époule
Accessibilité:
Navigation </a> </li>
<li> <A
href="../techniques/onix-metadata/index.html#navigation">Onix:
Navigation </a> </li>
</ul>
</section>
</section>
<section id="rich-content">
<h3 data-localization-id="rich-content-title">Rich Content </H3>
<div class="note">
<p> Ce champ d'affichage peut être masqué si les métadonnées sont
manquant. Alternativement, il peut être indiqué que
<span
data-localization-id="rich-content-unknown"
data-localization-mode="descriptive">Aucune information n'est disponible </span>
</p>
</div>
<p> indique la présence de mathématiques, de formules chimiques, de descriptions étendues pour des images riches en information, par exemple, des graphiques, des diagrammes, des figures, des graphiques, et si ceux-ci sont dans un format accessible ou disponibles sous une forme alternative, par exemple, que ce soit les mathématiques et les produits chimiques Les formules sont navigables avec des technologies d'assistance, ou si des descriptions étendues sont disponibles pour les images riches en information. De plus, il indique que la présence de vidéos et si des légendes fermées, des légendes ouvertes ou des transcriptions pour l'audio préenregistré sont disponibles. </p>
<p> Ce groupe ne doit être affiché que si les métadonnées
Indique la présence de mathématiques, de formules chimiques, de descriptions étendues, de vidéos ou de transcriptions de l'audio dans le titre, sinon il peut être caché. </p>
<section id="rc-statements">
<h4> afficher les instructions </h4>

<p> Les instructions descriptives et compactes pour le contenu riche sont les suivantes. </p>

<dl>
<dt> Si les mathématiques sont marqués en mathml: </dt>
<dd>
<p data-localization-id="rich-content-accessible-math-as-mathml"
data-localization-mode="compact">Mathématiques comme mathml</p>
<p data-localization-id="rich-content-accessible-math-as-mathml"
data-localization-mode="descriptive">Formules mathématiques au format accessible (mathml) </p>
</dd>

<DT> Si les mathématiques sont marquées en latex: </dt><dd>
<p data-localization-id="rich-content-accessible-math-as-latex"
data-localization-mode="compact">Mathématiques comme latex </p>
<p data-localization-id="rich-content-accessible-math-as-latex"
data-localization-mode="descriptive">Formules mathématiques au format accessible (latex) </p>
</dd>

<dt> Si les équations mathématiques sont décrites: </dt>
<dd>
<p data-localization-id="rich-content-accessible-math-described"
data-localization-mode="compact">Les descriptions de texte des mathématiques sont fournies </p>
<p data-localization-id="rich-content-accessible-math-described"
data-localization-mode="descriptive">Les descriptions de texte des mathématiques sont fournies </p>
</dd>

<dt> Si les formules chimiques sont marquées en mathml: </dt>
<dd>
<p data-localization-id="rich-content-accessible-chemistry-as-mathml"
data-localization-mode="compact">Formules chimiques en mathml </p>
<p data-localization-id="rich-content-accessible-chemistry-as-mathml"
data-localization-mode="descriptive">Formules chimiques au format accessible (MATHML) </p>
</dd>

<dt> Si les formules chimiques sont marquées en latex: </dt>
<dd>
<p data-localization-id="rich-content-accessible-chemistry-as-latex"
data-localization-mode="compact">Formules chimiques dans le latex </p>
<p data-localization-id="rich-content-accessible-chemistry-as-latex"
data-localization-mode="descriptive">Formules chimiques au format accessible (latex) </p>
</dd>

<dt> Si des descriptions étendues sont fournies pour les images: </dt>
<dd>
<p data-localization-id="rich-content-extended"
data-localization-mode="compact">Les images riches en information sont décrites par des descriptions étendues </p>
<p data-localization-id="rich-content-extended"
data-localization-mode="descriptive">Les images riches en information sont décrites par des descriptions étendues </p>
</dd>

<dt> Si des légendes fermées sont fournies pour les vidéos: </dt><dd>
<p data-localization-id="rich-content-closed-captions" data-localization-mode="compact">
Les vidéos ont des légendes fermées </p><p data-localization-id="rich-content-closed-captions" data-localization-mode="descriptive">
Les vidéos incluses dans les publications ont des légendes fermées </p></dd>

<dt>If open captions are provided for videos:</dt>
<DT> Si des légendes ouvertes sont fournies pour les vidéos: </dt><p data-localization-id="rich-content-open-captions" data-localization-mode="compact">
Les vidéos ont des légendes ouvertes </p>
<p data-localization-id="rich-content-open-captions" data-localization-mode="descriptive">
Les vidéos incluses dans les publications ont des légendes ouvertes </p>
</dd>

<dt> Si des transcriptions sont fournies pour le contenu auditif: </dt>
<dd>
<p data-localization-id="rich-content-transcript" data-localization-mode="compact">Transcrit (s) fourni </p>
<p data-localization-id="rich-content-transcript" data-localization-mode="descriptive">Transcription (s) fournie</p>
</dd>

<dt> si aucune métadonnée n'est fournie: </dt>
<dd>
<p data-localization-id="rich-content-unknown" data-localization-mode="compact">Aucune information n'est disponible </p>
<p data-localization-id="rich-content-unknown" data-localization-mode="descriptive">Aucune information n'est disponible </p>
</dd>
</dl>
</section>

<section id="rc-examples">
<h5> Exemples </h5>

<aside class="example" title="Publication with math and video">
<p> L'exemple suivant montre les instructions descriptives et compactes qui afficheraient
pour une publication avec des équations mathématiques en mathml et des vidéos avec des légendes fermées et
Transcriptions du dialogue. </p>

<dl>
<dt> Affichage compact </dt>
<dd>
<p class="ex-hd" data-localization-id="rich-content-title">Contenu riche </p>
<ul>
<li data-localization-id="rich-content-accessible-math-as-mathml"
data-localization-mode="compact">Mathématiques comme mathml </li>
<li data-localization-id="rich-content-closed-captions"
data-localization-mode="compact">Les vidéos ont des légendes fermées </li>
<li data-localization-id="rich-content-transcript"
data-localization-mode="compact">Transcription (s) fournie) </li>
</ul>
</dd>

<dt> Affichage descriptif </dt><dd>
<p class="ex-hd" data-localisation-id = "riche-content-title"> contenu riche </p><ul>
<li data-localization-id="rich-content-accessible-math-as-mathml"
data-localization-mode="descriptive">Formules mathématiques au format accessible (Mathml) </li>
<li data-localization-id="rich-content-closed-captions"
data-localization-mode="descriptive">Les vidéos incluses dans les publications ont des légendes fermées </li>
<li data-localization-id="rich-content-transcript"
data-localization-mode="compact">Transcription (s) fournie) </li>
</ul>
</dd>
</dl>
</aside>
</section>

<section id="rc-techniques">
<h4> Afficher les techniques de support de contenu riche </h4>


<p> Les techniques spécifiques pour répondre à ce principe sont
défini dans les documents suivants: </p>

<ul>
<li><ahref = "../Techniques /ePub-Metadata /index.html # riche-contenu"> epub
Accessibilité: contenu riche </a>
</li>
<li> <A
href = "../Techniques /Onix-Metadata /index.html # riche-contenu"> ONIX:
Contenu riche </a> </li>
</ul>
</section>
</section>
<section id="hazards">
<h3 data-localization-id="hazards-title">Dangers </h3>

<div class="note">
<p> Ce champ d'affichage peut être masqué si les métadonnées sont
manquant. Alternativement, il peut être indiqué que
<span data-localization-id="hazards-no-metadata"
data-localization-mode="descriptive"> Aucune information n'est disponible</span>
</p>
</div>

<p> identifie tous les dangers potentiels (par exemple, clignoter
éléments, sons et simulation de mouvement)
Cela pourrait affliger les utilisateurs physiologiquement sensibles. </p>

<div class="note"> <p> La recherche n'a pas identifié de source
pour des éclaircissements sur ce qui constitue un danger solide
dans les publications numériques. Quand une meilleure pratique est
Disponible, il sera inclus dans ces directives.
Il est laissé à la discrétion de l'éditeur sur
Quoi d'inclure dans les métadonnées. S'il y a un
danger sonore possible, une option consiste à ajouter
Informations dans le résumé de l'accessibilité. </p>
</div>
<p> Contrairement à d'autres propriétés d'accessibilité, la présence de
les dangers peuvent être exprimés soit positivement, soit
négativement. En effet, les utilisateurs recherchent du contenu
C'est sûr pour eux et je veux savoir
Lorsque le contenu est potentiellement dangereux pour eux. </p>

<p> Le vocabulaire des dangers de la propriété comprend une valeur de
inconnu, ce qui signifie le créateur de contenu du
Les métadonnées reconnaissent explicitement que la ressource a
Pas été vérifié pour les dangers. C'est
différent de ne fournir aucune métadonnée pour cette propriété. </p>

<section id="hazards-statements">
<h4> afficher les instructions </h4>

<p> Les déclarations descriptives et compactes pour les dangers sont les suivantes. </p>

<dl>
<dt> S'il n'y a pas de dangers: </dt>
<dd>
<p data-localization-id="hazards-none"
data-localization-mode="compact">Pas de dangers</p>
<p data-localization-id="hazards-none"
data-localization-mode="descriptive">La publication ne contient aucun danger</p>
</dd>
<dt> S'il y a un risque clignotant: </dt>
<dd>
<p data-localization-id="hazards-flashing"
data-localization-mode="compact">Clignotant
Contenu </p>
<p data-localization-id="hazards-flashing"
data-localization-mode="descriptive">Le
La publication contient du contenu clignotant
ce qui peut provoquer un photosensible
convulsions </p>
</dd>

<dt> S'il y a un risque de simulation de mouvement: </dt>
<dd>
<p data-localization-id="hazards-motion"
data-localization-mode="compact">Mouvement
simulation </p>
<p data-localization-id="hazards-motion"
data-localization-mode="descriptive">Le
La publication contient des simulations de mouvement
qui peut provoquer le mal des transports </p>
</dd>

<dt> S'il y a un risque sonore: </dt>
<dd>
<p data-localization-id="hazards-sound"
data-localization-mode="compact">Sons</p>
<p data-localization-id="hazards-sound"
data-localization-mode="descriptive">Le
La publication contient des sons qui
peut être inconfortable </p>
</dd>

<DT> Si les dangers ne sont pas connus: </dt>
<dd>
<p data-localization-id="hazards-unknown"
data-localization-mode="compact">La présence de dangers est inconnue </p>
<p data-localization-id="hazards-unknown"
data-localization-mode="descriptive">Les cadeaux
des dangers est inconnu </p>
</dd>
<dt> Si aucune métadonnée n'est fournie: </dt>
<dd>
<p data-localization-id="hazards-no-metadata"
data-localization-mode="compact">Aucune information n'est disponible </p>
<p data-localization-id="hazards-no-metadata"
data-localization-mode="descriptive">Aucune information n'est disponible </p>
</dd>
</dl>
</section>

<section id="hazards-examples">
<h4> Exemples </h4>
<aside class="example" title="Publication with no hazards">
<p> L'exemple suivant montre les instructions descriptives et compactes qui afficheraient
pour une publication sans clignotement, simulation de mouvement ou dangers solides. </p>

<dl>
<dt> Affichage compact </dt>
<dd>
<p class="ex-hd" data-localization-id="hazards-title">Dangers</p>
<p data-localization-id="hazards-none"
data-localization-mode="compact">Aucun danger </p>
</dd>

<dt>Descriptive display</dt>
<dd>
<p class="ex-hd" data-localization-id="hazards-title">Dangers</p>
<p data-localization-id="hazards-none"
data-localization-mode="descriptive">La publication ne contient aucun danger </p>
</dd>
</dl>
</aside>
</section>

<section id="hazards-techniques">
<h4> Afficher les techniques de rapport des dangers </h4>

<p> Les techniques spécifiques pour répondre à ce principe sont
défini dans les documents suivants: </p>
<ul>
<li><a
href="../techniques/epub-metadata/index.html#hazards">Époule
Accessibilité:
Dangers </a> </li>
<li> <A
href="../techniques/onix-metadata/index.html#hazards">Onix:
Dangers </a> </li>
</ul>
</section>
</section>
<section id="accessibility-summary">
<h3 data-localization-id="accessibility-summary-title">
Résumé de l'accessibilité </H3>

<div class="note">
<p> Ce champ d'affichage peut être masqué si les métadonnées sont
manquant. Alternativement, il peut être indiqué que
<span
data-localization-id="accessibility-summary-no-metadata"
data-localization-mode="compact">Aucune information n'est disponible </span>
</p>
</div>

<p> Le résumé de l'accessibilité a été prévu (en epub
Accessibilité 1.0) à décrire en lienable humain
prose les fonctionnalités d'accessibilité présents dans le
publication ainsi que toute lacune. En commençant par epub
Accessibilité Version 1.1 Le résumé de l'accessibilité
est devenu un résumé lisible par l'homme du
accessibilité qui complète, mais ne duplique pas,
les autres métadonnées de la découverte. </p>
<p> C'est un champ de forme libre qui permet aux auteurs d'ajouter
informations supplémentaires à l'accessible
propriétés de la ressource. </p>

<p> En raison de sa nature, aucun traitement spécifique du contenu
est requis; il suffit d'extraire le
texte à partir des métadonnées et l'afficher aux utilisateurs finaux. </p>

<section id="sum-examples">
<h4> Exemples </h4>
<aside class="example"
title="An example accessibility summary">
<h4 data-localization-id="accessibility-summary-title">Résumé de l'accessibilité </H4>
<p> Les experts en matière ont été utilisés pour créer le texte ALT.
Les tables sont représentées comme des images, et
Le texte intégral de la table est fourni sous le
image dans l'élément de détails, qui peut
être élargi. Il y a plusieurs courtes vidéos dans
Langue de signe américaine qui explique la clé
concepts. </p>
<p> Aucune information n'est disponible </p>
</aside>
</section>

<section id="sum-techniques">
<h4> Afficher les techniques de support de résumé d'accessibilité
</h4>

<p> Les techniques spécifiques pour répondre à ce principe sont
défini dans les documents suivants: </p>
<ul>
<li><a
href="../techniques/epub-metadata/index.html#accessibility-summary">Époule
Accessibilité:
Résumé de l'accessibilité </a> </li>
<li><a
href="../techniques/onix-metadata/index.html#accessibility-summary">Onix:
Accessibilité
Résumé </a> </li>
</ul>
</section>
</section>
<section id="legal-considerations">
<h3 data-localization-id="legal-considerations-title">Légal
Considérations </h3>

<div class="note">
<p> Ce champ d'affichage doit être masqué si les métadonnées sont
pas présent. </p>
</div>

<div class="note"> Avertissement: rien ici ne peut être interprété
En tant que conseils juridiques fournis par W3C ou tout le
groupes ou individus qui ont contribué à cela
document. Obtenez toujours des conseils juridiques de l'interne
ou votre avocat retenu pour évaluer la conformité légale et
Risque. </div>
<p> dans certaines juridictions, les éditeurs peuvent être en mesure de réclamer un
exemption de la fourniture de
publications, y compris la fourniture d'accessibilité
métadonnées. Cela devrait toujours être soumis à
Clarification par le conseiller juridique pour chaque juridiction.
Un exemple de cela, au moment de l'écriture, est
de la loi européenne sur l'accessibilité (EAA) lorsque
L'éditeur est un micro-enterprise (c'est-à-dire,
les entreprises employant moins de 10 personnes et avec
Le chiffre d'affaires annuel ou le bilan total pas
dépassant 2 millions d'euros). </p>
<p> Autres considérations juridiques actuellement incluses dans l'EAA
peut inclure des exceptions sur l'individu
versions d'un titre, où la juridiction ne nécessitera pas
le titre à être accessible s'il implique un
Altération fondamentale du contenu, ou si elle le fait
accessible placerait une disproportionnée
fardeau pour l'éditeur. (Cela peut varier dans d'autres
juridictions). </p>
<p> Les éditeurs peuvent devoir inclure des informations sur un
Exemption ou exception dans les métadonnées pour légal ou
des raisons de clarté, soit aux corps qui appliquent
législation ou pour d'autres entreprises aux affaires
communication. Cependant, ce ne sont pas des informations qui
doit être affiché sur les sites publics comme il le fait
ne signifie rien pour la plupart des consommateurs et pourrait conduire à
malentendus. Néanmoins, l'objectif
est de fournir autant d'informations d'accessibilité que possible. </p>

<section id="legal-statements">
<h5> afficher les instructions </h5>

<p> Les déclarations descriptives et compactes pour les exemptions légales sont les suivantes. </p>

<div class="note">
<p> Dans de nombreux cas, aucune exception ou exemption légale
Des informations seront présentées. Ce qui suit
L'exemple est fourni comme une explication possible lorsque l'exception légale ou l'exemption
les informations doivent être présentées. </p>

</div>

<dl>
<dt> Si la publication demande une exemption: </dt>
<dd>
<p data-localization-id="legal-considerations-exempt"
data-localization-mode="compact">Réclame une exemption d'accessibilité dans certaines juridictions </p>
<p data-localization-id="legal-considerations-exempt"
data-localization-mode="descriptive">Ce
publication réclame une exemption d'accessibilité dans
Certaines juridictions </p>
</dd>

<dt> Si aucune métadonnée n'est fournie: </dt>
<dd>
<p data-localization-id="legal-considerations-no-metadata"
data-localization-mode="compact">Aucune information n'est disponible </p>
<p data-localization-id="legal-considerations-no-metadata"
data-localization-mode="descriptive">Aucune information n'est disponible </p>
</dd>
</dl>
</section>

<section id="legal-examples">
<h4> Exemples </h4>
<aside class="example" title="Publication with an exemption">
<p> L'exemple suivant montre les instructions descriptives et compactes qui afficheraient
pour une publication qui demande une exemption légale dans l'accessibilité d'une juridiction
exigences. </p>

<dl>
<dt> Affichage compact </dt>
<dd>
<p class="ex-hd" data-localization-id="legal-considerations-title">Considérations juridiques </p>
<p data-localization-id="legal-considerations-exempt"
data-localization-mode="compact">Réclame une exemption d'accessibilité dans certaines juridictions </p>
</dd>

<dt> Affichage descriptif </dt>
<dd>
<p class="ex-hd" data-localization-id="legal-considerations-title">Considérations juridiques </p>
<p data-localization-id="legal-considerations-exempt"
data-localization-mode="descriptive">Cette publication demande une exemption d'accessibilité dans certaines juridictions </p>
</dd>
</dl>
</aside>
</section>

<section id="legal-techniques">
<h4> Afficher les techniques de considérations juridiques </h4>
<p> Les techniques spécifiques pour répondre à ce principe sont
défini dans les documents suivants: </p>
<ul>
<li><a
href="../techniques/epub-metadata/index.html#legal-considerations">EPUB
Accessibilité:
Considérations juridiques </a> </li>
<li><a
href="../techniques/onix-metadata/index.html#legal-considerations">Onix:
légal
Considérations </a> </li>
<ul>
</section>

</section>
<section id="additional-accessibility-information">
<h3 data-localization-id="additional-accessibility-information-title">Accessibilité supplémentaire
Informations </h3>

<div class="note">
<p> Ce champ d'affichage peut être masqué si les métadonnées sont
manquant. </p>
</div>

<p> Cette section répertorie les catégories de métadonnées supplémentaires qui
peut aider les utilisateurs à mieux comprendre le
Caractéristiques d'accessibilité des publications numériques.
Ce sont pour les métadonnées qui ne s'intègrent pas dans
les autres catégories ou sont rarement utilisées dans le commerce
publication. </p>

<p> Les informations d'accessibilité supplémentaires comprennent un large
gamme d'informations liées à la
le contenu de la publication. Par conséquent, les fonctionnalités sont
regroupé ci-dessous pour que la présentation soit plus
compréhensible. Les implémenteurs peuvent choisir de regrouper les informations supplémentaires par ces catégories dans leurs présentations. </p>

<p> Les catégories sont: </p>
<dl>
<dt> Structure </dt>
<dd>
<p> pour plus d'informations sur toute aide structurée qui
Faciliter l'utilisation d'une ressource (par exemple, Aria). </p>
</dd>
<dt> Page Breaks </dt>
<DD> L'inclusion de marqueurs de pause de page d'un imprimé
La source permet aux utilisateurs d'identifier où ils sont
dans une publication numérique par rapport à son imprimé
équivalent. </dd>
<dt> adaptation </dt>
<dd>
<p> pour plus d'informations sur les dispositions du contenu qui
Activer la lecture dans les modes d'accès alternatifs

(par exemple, annotations de rubis, signe
langue, transcriptions). </p>



</dd>


<dt> Clarity </dt>
<dd>
<p> Pour plus d'informations sur les façons dont le contenu a été
amélioré pour l'amélioration de l'auditoire ou du visuel
clarté (par exemple, balisage de prononciation). </p>
</dd>

<DT> TACTILE </DT>
<dd>
<p> pour plus d'informations sur le contenu disponible en
une forme tactile (par exemple, contenu tactile, tactile
graphiques, objets tactiles). </p>
</dd>

<! -Peut-être que nous pouvons supprimer le contenu
<dt> Contenu </dt>
<dd>
<p> pour plus d'informations sur des types spécifiques de contenu
Présent dans la publication numérique (par exemple, texte
sur visuel, musique sur visuelle). </p>
</dd> ->

<dt> autre </dt>
<dd>
<p> pour des informations qui ne tombent pas dans l'un des
les catégories précédentes (par exemple, contrôle de synchronisation). </p>
</dd>
</dl>

<section id="add-info-statements">
<h4> afficher les instructions </h4>

<p> Les instructions descriptives et compactes pour des informations supplémentaires sont les suivantes. </p>

<div class="note"> Il existe de nombreuses fonctionnalités qui peuvent être
présent. Seules certaines des fonctionnalités sont répertoriées ici.
Une liste complète peut être trouvée dans les techniques. </div>

<dl>
<dt> S'il y a des rôles Aria: </dt>
<dd>
<p data-localization-id="additional-accessibility-information-aria"
data-localization-mode="compact">Les rôles Aria incluent</p>
<p data-localization-id="additional-accessibility-information-aria"
data-localization-mode="descriptive">Le contenu est amélioré avec des rôles Aria pour
optimiser l'organisation et faciliter
navigation </p>
</dd>
<dt> S'il y a des marqueurs de pause de page: </dt>
<dd>
<p data-localization-id="additional-accessibility-information-page-breaks"
data-localization-mode="compact">Les pauses de page incluses </p>
<p data-localization-id="additional-accessibility-information-page-breaks"
data-localization-mode="descriptive">Pauses de page incluses de l'impression originale
Source </p>
</dd>
<dt> S'il y a des graphiques tactiles: </dt>
<dd>
<p data-localization-id="additional-accessibility-information-tactile-graphics"
data-localization-mode="compact">Les graphiques tactiles inclus </p>
<p data-localization-id="additional-accessibility-information-tactile-graphics"
data-localization-mode="descriptive">Des graphiques tactiles ont été intégrés à
faciliter l'accès aux éléments visuels pour
aveugles </p>
</dd>
</dl>
</section>

<section id="add-info-examples">
<h5>Exemples</h5>

<aside class="example" title="Publication with ARIA roles and page breaks">
<p> L'exemple suivant montre les instructions descriptives et compactes qui afficheraient
pour une publication qui comprend des rôles Aria et qui a des numéros de page statiques. </p>

<dl>
<dt> Affichage compact </dt>
<dd>
<p class="ex-hd" data-localization-id="additional-accessibility-information-title">Informations sur l'accessibilité supplémentaires </p>
<ul>
<li data-localization-id="additional-accessibility-information-aria"
data-localization-mode="compact">Les rôles Aria inclus </li>
<li data-localization-id="additional-accessibility-information-page-breaks"
data-localization-mode="compact">Les pauses de page incluses </li>
</ul>
</dd>

<dt> Affichage descriptif </dt>
<dd>
<p class="ex-hd" data-localization-id="additional-accessibility-information-title">Additional accessibility information</p>
<ul>
<li data-localization-id="additional-accessibility-information-aria"
data-localization-mode="descriptive">Le contenu est amélioré avec des rôles Aria pour
Optimiser l'organisation et faciliter la navigation </li>
<li data-localization-id="additional-accessibility-information-page-breaks"
data-localization-mode="descriptive">Les pauses de page incluses de la source d'impression originale </li>
</ul>
</dd>
</dl>
</aside>
</section>

<section id="add-info-techniques">
<h4> Affichage des techniques pour une accessibilité supplémentaire
Informations </h4>

<p> Les techniques spécifiques pour répondre à ce principe sont
défini dans les documents suivants: </p>
<ul>
<li><a
href="../techniques/epub-metadata/index.html#additional-accessibility-information">Époule
Accessibilité: informations supplémentaires sur l'accessibilité </a> </li>
<li><a
href="../techniques/onix-metadata/index.html#additional-accessibility-information">Onix:
Informations sur l'accessibilité supplémentaires </a> </li>
</ul>
</section>
</section>
</section>
<section id="discovering-accessible-content">
<h2> Découvrir le contenu accessible </h2>

<p> Les directives pour présenter les métadonnées d'accessibilité détaillées
dans ce document sont destinés à s'améliorer
L'expérience utilisateur lorsque les lecteurs parcourent l'entrée du catalogue
pour une publication. Cependant, l'accessibilité
Les métadonnées ont également un rôle essentiel à jouer pour aider les lecteurs
Découvrez des publications accessibles à
eux. </p>

<p> Les fournisseurs de publication, tels que les vendeurs et les bibliothèques, créent
outils de recherche et de filtrage qui interprètent
métadonnées d'accessibilité pour aider à la découverte. L'ensemble et
la variété des filtres dépend du public, ils
adresse et type de livre qu'ils proposent. </p>

<p> les commentaires de l'utilisateur indiquent qu'en l'absence de spécifique
Filtres d'accessibilité, ils trouvent les détails du produit
comme le format de fichier et les mesures de protection (par exemple, numérique
Gestion des droits) Informations cruciales dans
déterminer l'utilisabilité. </p>

<p> en tenant compte de ces réalités, ce qui suit
Les sections proposent un ensemble minimum et étendu
pour les options de filtrage. La plupart des informations spécifiques pourraient
être ajouté s'il est considéré comme une utilisation pour le
public de la plateforme. </p>

<section id="minimum-filtering-set">
<h3> Ensemble de filtrage minimum </h3>

<p> Systèmes de lecture, commerce et plateformes de distribution
aura généralement un filtrage spécifique
options; avoir l'uniformité pour les aspects clés et la fourniture
Les conseils pour une approche standardisée peuvent
Aidez le processus de découverte pour les utilisateurs à la recherche
titres pertinents. Accomplir cela, cependant,
ne doit pas empêcher les utilisateurs ayant des besoins de lecture spécifiques
de trouver des livres qu'ils recherchent. À
atteindre cet objectif, il est recommandé que toutes les plateformes
présenter deux capacités minimales, centrées
autour des façons de consommer le contenu. Ce sont: </p>

<l>
<li> titres qui prennent en charge les ajustements visuels </li>
<li> Titres qui soutiennent la lecture non visuelle </li>
</l>

<p> Il convient de noter que seules les valeurs positives doivent être utilisées. </p>
<div class="note"> <p> Il est recommandé de filtrer les valeurs des métadonnées d'accessibilité d'origine. Les chaînes présentées à l'utilisateur pour le filtrage peuvent tirer des chaînes orientées utilisateur. </p> </div>

<à part class="example" title = "Options de filtrage minimum">
<ul>
<li> Prise en charge de la lecture non visuelle </li>
<li> prend en charge les ajustements visuels </li>
</ul>
</aside>
</section>

<section id="extended-filtering-set">
<h3> Ensemble de filtrage étendu </h3>

<p> Dans des domaines spécifiques, l'ajout d'autres options
être important pour aider les utilisateurs à trouver du contenu
qui répond à un besoin ou un scénario particulier. Chaque
le cas de domaine entraînerait la sélection
des articles appropriés. Quelques exemples de ces domaines
(non exclusif) sont: </p>

<ul>
<li> Dans un contexte académique, la présence d'imprimés
Les numéros de page peuvent être cruciaux pour s'assurer que le
Lecteur pourra trouver ou faire une citation.
</li>
<li> Dans un contexte technique ou scientifique, des informations sur l'accès à un contenu riche comme les graphiques, les diagrammes, les figures, les graphiques, les mathématiques et les formules chimiques seront importants. </li>
<li> sur les marchés où la conformité à la législation est
requis, la compréhension des informations de conformité peut être obligatoire. </li>
<li> plateformes dédiées à la vente de livres pour enfants et
Le contenu interactif peut vouloir permettre aux utilisateurs
pour sélectionner des livres sans dangers ou les informer sur
La présence d'un audio préenregistré. </li>
</ul>

<à part class="example" title = "Options de filtrage étendues">
<ul>
<li> Accédez à Page </li>
<li> contient des graphiques, des diagrammes, des figures, des graphiques, des mathématiques ou des formules chimiques </li>
<li> Cette publication répond aux normes d'accessibilité acceptées </li>
<li> Pas de dangers </li>
<li> Audio préenregistré </li>
</ul>
</roprows>
</section>
</section>
<section id = "localisation">
<h2> Localisation </h2>

<p>
Un ebook peut être acheté dans n'importe quel pays sans limité
disponibilité ou frais de livraison supplémentaires.
Les lecteurs veulent un affichage cohérent de l'accessibilité
informations, et c'est le rôle principal de l'affichage
guide.
Le libellé proposé dans ce guide a été largement discuté
par un grand groupe représentant différent
acteurs des géographies anglophones. Il a été
amélioré après les implémentations de preuve de concept
et examiné par des panneaux de testeurs. </p>

<p>
Nous comprenons que différents pays ou différents cibles
Les services d'audience peuvent vouloir utiliser un langage spécifique, et nous
ont fourni une flexibilité dans le guide pour s'adapter à ce
tout en maintenant un niveau élevé de compréhension et similaire
Qualité pour aider les utilisateurs d'un pays à trouver des informations également
entre deux librairies ou bibliothèques dans la même langue
zone.
Il ne suffit pas de traduire simplement les cordes; le subtil
Signification des mots et des phrases des concepts d'accessibilité
doit être localisé pour une compréhension maximale. Par conséquent, nous
l'intention de fournir un mécanisme pour la communauté de l'édition
pour fournir des traductions qui localisent les cordes pour
Communication tout aussi efficace dans de nombreuses langues. </p>

<p> le <a href = "../Localizations"> Afficher le guide localisation
Page de cordes </a> Répertoriez les traductions avec
contextualisation du processus de localisation. </p>
<p> Les sous-sections suivantes proposent un cadre de localisation
Pour aider à établir des libellés linguistiques, les libellés ont convenu
entre les acteurs de la zone géographique concernée. </p>

<segction>
<h3> Stratégie de localisation </H3>

<p>
Avec le paysage en évolution rapide des livres électroniques accessibles
Les personnes disponibles, la plupart des personnes concernées découvrent un nouveau
monde. Pour s'assurer que les informations sont largement réparties et
compris, la mise en œuvre des acteurs locaux comme
bibliothèques au service des personnes handicapées et autres
acteurs locaux dans le combat pour mettre fin au livre Famine pour
Les lecteurs ayant des handicaps imprimés sont cruciaux et devraient être
mis en évidence.
</p>
<p>
La localisation du guide d'affichage est un bon
possibilité de faire connaître la riche accessibilité
Caractéristiques offertes par des formats modernes comme EPUB. Dans
De plus, avoir une échelle de projet locale pour écrire un
Le vocabulaire compréhensible pour décrire de telles fonctionnalités est un
approche qualitative précieuse qui bénéficiera à chaque
lecteur dans la chaîne de valeur.
</p>
<p>
Pour construire un projet local et faciliter les commentaires
Comparaisons, vous pouvez utiliser la méthodologie open source,
Ressources et prototypes publiés par Edrlab pour le
Original <A
href = "https://edition-accessble.github.io/signalement/en/index-en.html"> signalation
Projet de livres numériques accessibles </a>
initial <a
href = "https://edition-accessible.github.io/signalament/documents/edrlab-signalement_letrew3c_en.pdf"> commentaires
Lettre (PDF) </a> adressée au début de 2022, et a
déjà été utilisé et adapté à divers endroits.
</p>
<p>
Dans ces projets, l'accent a été mis sur
Implications pour les utilisateurs finaux. Par exemple, les Français
Le libellé proposé par EDRLAB résulte d'un
Enquête sur différents groupes de lecteurs, soigneusement sélectionné
panneaux d'observations individuelles et un
processus de rétroaction via une formule dédiée disponible
sur les 140 premières plateformes d'implémentation.
</p>
<p>
De plus, des entreprises comme Vitalsource qui ont besoin de large
la localisation a proposé d'ouverture
Travail de traduction professionnelle, qui a produit le
la quantité nécessaire et c'est mieux à utiliser que rien
Quand aucun projet national n'a émis une fabrication à la main
vocabulaire.
</p>
<p>
Pour concilier les deux sources de localisation fournies
Matériaux, nous proposons un mécanisme de collecte basé sur un
Identification détaillée de la provenance. Parce que
Personnes et organisations avec différents niveaux de
La technicité doit être en mesure de contribuer, nous acceptons les deux
les fichiers bruts via des demandes de traction et proposent également un convivial
Interface utilisateur de localisation via Gitlocalise.
</p>

</section>
<section>
<h3 id="How-to-contribute">How to contribute?</h3>
<p>First let us know as sooComment contribuer? </h3>
<p> Faites-nous d'abord savoir dès que possible
travailler sur une localisation et souhaiter le soumettre. Que
nous permet de préparer un espace réservé à votre travail. Ce
n'est pas obligatoire mais nous vous invitons à contacter le groupe
et participer à un appel régulier du groupe de travail
Comme ceux-ci sont ouverts à tous. </p>
<p> Lorsque vous êtes prêt à publier votre travail, deux options sont
possible: </p>
<ul>
<li> Si vous ne savez pas ce qu'est un JSON ou une demande de traction,
Vous êtes invités à nous contacter afin que nous puissions attribuer un
rôle de traducteur au <a
href = "https://gitlocalize.com/repo/9555"> gitlocaliser
Page de projet dédiée </a>. </li>
<li> Si vous vous sentez techniquement prêt ou si vous avez un collaborateur
qui peut pousser une demande de traction, le processus est de
Dupliquez le fichier d'origine canonique
UX-Guide-Metadata /Draft /Localizations /En-US /Display_Guide_Vocabulary_W3C_en-us.json,
modifiez-le en modifiant les valeurs devant chaque
Clé et ouvrez une demande de traction afin que nous puissions l'examiner.
Veuillez noter que nous pourrions avoir des questions ou poser
pour la précision dans le processus avant d'accepter et
fusion de votre contribution. </li>
</section>
<section>
<h3 id="How-to-choose-between-localization-files">Comment
Choisissez entre les fichiers de localisation? </h3>

<p> Les premières clés de chaque fichier JSON contiennent descriptif
Informations à ce sujet, y compris: </p>
<ul>
<li> Auteur, nom de l'organisation responsable du
établissement et maintenance de cette localisation
</li>
<li> Langue, est un code de 4 lettres où les deux premiers
Les lettres spécifient la langue selon ISO 639-1 et
les deux autres le pays selon ISO 3166-1 Alpha-2
</li>
<li> Variante, un nom gratuit d'un mot pour identifier votre travail
</li>
<li> Le public décrit le public. Nous vous recommandons d'utiliser
tout vocabulaire du <a
href = "https://ns.editeur.org/onix/en/28/"> Onix
Liste 28 </a>. Plus d'un public peut être
informé d'une virgule séparant chacun. </li>
<li> Description, un champ gratuit comprenant un court
Description de la façon dont cette localisation a été obtenue
</li>
</ul>

</section>
</section>
<section id="implementations">
<h2> implémentations </h2>

<div class="probleme" data-number = "268"> Nous collectons
Informations sur les entreprises et les organisations qui souhaitent
pour éventuellement commettre des exemples de leur mise en œuvre. S'il te plaît
Visitez ce numéro GitHub pour examiner les sociétés
et les organisations qui ont mis leur nom. À
peut-être volontaire une mise en œuvre, veuillez mettre
Le nom de votre entreprise, votre nom et vos coordonnées.
</div>

<p> Ces directives fournissent un cadre général et font
Suggestions sur l'affichage de l'accessibilité
métadonnées. Ce n'est pas une description normative de ce qui doit être
fait. Il est instructif de fournir des exemples
des implémentations de la communauté. </p>

<p> lié ​​ci-dessous sont des pages statiques qui montrent de la vie réelle
implémentations. Nous avons capturé ces exemples de
Sites Web de l'organisation qui ont accepté de nous permettre de
présenter le travail qu'ils ont fait pour afficher
métadonnées d'accessibilité. </p>

<p> Liens TBD </p>
</section>
<div data-include="../common/acknowledgements.html"
data-include-replace="true"></div>
</body>

</html>
