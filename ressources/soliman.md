---
layout: document
title: Quand la préservation culturelle rencontre l'innovation inclusive, retour d'expérience du projet SOLIMAN.
date: 2025-09-04
subtitle: 
orientation: 
audience: services de production
previous: ./traiter.html
# next: ./collecter.html
# titleNext: Renseigner
titlePrev: traiter
# draft: true
---

Les nouvelles lois européennes sur l'accessibilité imposent aux livres numériques de répondre à des normes spécifiques pour les lecteurs atteints de handicaps, avec trois axes principaux : informer le lecteur, permettre une lecture avec un rendu alternatif (tel que l'audio et le braille), et permettre des ajustements de la mise en page visuelle pour répondre aux besoins individuels. L'accessibilité des nouvelles publications peut être réalisée en mettant à jour le flux de travail, mais la mise à jour d'une vaste collection de titres de fonds est une tâche ardue. Avant de s'engager et pour éviter le découragement, il est nécessaire de mieux comprendre l'accessibilité des collections. Cette étape est également une excellente occasion de commencer à se conformer à la législation en fournissant des moyens d'informer les gens sur l'accessibilité de l'ebook. Le projet SOLIMAN nous a permis d'explorer cette voie et de réaliser des avancées significatives en matière de règles et d'outils open source pour traiter de vastes collections.

## Relever le défi pour une collection patrimoniale

Une analyse de situation et des lacunes des collections européennes a été menée en 2024 par le projet ABELab au niveau européen. Le rapport final a souligné deux défis cruciaux. Premièrement, le fonds européen n'est pas homogène, ce qui signifie que l'extraction de statistiques à partir des fichiers est nécessaire pour découper efficacement de vastes collections en ensembles d'ebooks ayant des besoins similaires. Deuxièmement, il y a trop peu d'outils et de documentation open source disponibles pour l'automatisation, ce qui entraîne des efforts redondants lors de la sélection et de l'évaluation de la qualité des opérations de remédiation.

La mission patrimoniale de l'organisation FeniXX, qui lui a été confiée par les éditeurs et le ministère de la Culture depuis 2014, a abouti à la numérisation et à la commercialisation de la collection de livres indisponibles du XXe siècle, inscrits au registre ReLIRE publié par la Bibliothèque nationale de France. Le projet, soutenu notamment par le Centre National du Livre, a permis la réédition sous forme numérique de près de 98 000 ouvrages et leur mise à disposition des lecteurs et usagers des bibliothèques en France et à l'étranger par l'intermédiaire des librairies. La production numérique et la vente de ces ouvrages ont été achevées au premier trimestre 2023.
Dès le début du projet en 2025, FeniXX a choisi l'EPUB 3 comme format de publication, conformément aux recommandations du W3C. 71% du catalogue des livres indisponibles est ainsi disponible au format EPUB 3.

FeniXX a également abordé la question de l'accessibilité numérique depuis 2019. À cette époque, l'entreprise a pris des mesures pour intégrer une partie des normes WCAG dans son flux de production afin d'atteindre un premier niveau d'accessibilité native sur ses EPUB.
En raison de sa taille et de son chiffre d'affaires, FeniXX est exemptée des obligations d'accessibilité des produits et services pour les personnes handicapées. Cependant, en raison de la nature patrimoniale de son catalogue et de sa mission initiale, FeniXX souhaite pouvoir effectuer toutes les adaptations nécessaires dans la limite de ses possibilités.

Les collections FeniXX ont la particularité d'être générées à partir d'un processus automatisé ; bien que deux périodes aient produit des fichiers différents, une base de référence de qualité peut être facilement établie. Les mêmes feuilles de style gèrent l'affichage de tous les ebooks, les logos des financeurs sont les mêmes dans chaque livre, les images décoratives ont été correctement étiquetées avec un rôle présentation sur l'un des deux lots et un texte alternatif standard « Illustration » a été ajouté aux images significatives en attente d'être décrites le jour où la technologie et le budget seraient disponibles.

## Analyse initiale

Initialement, nous avons appliqué la méthode d'analyse ABELab décrite dans le document d'analyse des lacunes (Gap Analysis, disponible en ligne en anglais), ce qui nous a permis de positionner le corpus étudié par rapport aux collections européennes.

Les indicateurs de complexité de remédiation établis par ABELab indiquent que le corpus Fenixx obtient des scores entre 4 et 56, la majorité des fichiers se situant dans la fourchette de 4 à 21. En comparaison, les échantillons ABELab présentaient des scores allant de 4 à 77, la majorité des fichiers se situant entre 10 et 26. Les échantillons Fenixx se situent donc dans la fourchette basse par rapport à l'étude des échantillons représentant les collections européennes étudiées par ABELab.

Pour mieux définir la difficulté de remédiation du corpus FENIXX, nous avons pu établir que certains indicateurs n'étaient pas significatifs compte tenu des connaissances détaillées dont nous disposons sur le corpus. Ainsi nous avons pu établir trois manques principaux en plus des problématiques de description d’images : 

* 49 % de la collection manquait de métadonnées d'accessibilité, même avec les règles d'inférence de pointe.
* 29 % de la collection avait plus de 20 informations de langue probablement erronées pour les phrases de plus de deux mots.
* 10 % de la collection manquait d'identification appropriée sur les colonnes et les en-têtes de lignes des tableaux.

La connaissance détaillée du corpus nous a aussi permis d'identifier des indicateurs supplémentaires, notamment le nombre d'images par livre ; le nombre de livres contenant une ou deux images ; le nombre de fichiers contenant des images récurrentes identifiées (comme les logos) ; le nombre d'images dont le texte alternatif peut être considéré comme significatif, c'est-à-dire contenant un texte alternatif de plus d'un mot ; le nombre d'images explicitement déclarées comme décoratives.

Le corpus comprend 1 029 739 images, dont 7 % sont des couvertures, 6 % sont les logos des financeurs, 1 % sont marquées comme décoratives et 6 % ont un texte alternatif de plus d'un mot, ce qui les rend suffisamment longues pour être considérées comme significatives. Cela signifie qu'un total de 20 % des images ne nécessitent pas de remédiation.

D'autre part, 49 % du corpus a moins de trois images, et 28 % a plus de 100 images. En croisant les deux indicateurs, nous comprenons que près de la moitié du corpus est lisible en texte, ce qui lui permet d'être rendu en voix de synthèse et en braille. Un quart contenant moins de 11 images devrait être rapide à améliorer avec des descriptions d'images significatives, tandis que le dernier quart nécessitera un effort plus important.

Enfin, une analyse experte du CSS n'a révélé aucun blocage particulier à la transformabilité de l'affichage, du moins pour les applications utilisant Readium CSS. Une liste détaillée des améliorations potentielles a été compilée pour améliorer l'expérience utilisateur.

## Extractions, inférences et métadonnées 

Fort de ces données, une feuille de route de développement a été établie. Il a été choisi d'améliorer un outil existant, déjà utilisé dans certaines parties de l'industrie, au lieu de construire un outil séparé qui aurait dû être adopté. Le Readium Go Toolkit a été le point de départ, mais ces fonctionnalités ont été regroupées dans un toolkit distinct, appelé Readium CLI, un ensemble d'utilitaires en ligne de commande qui répondent à un large éventail de cas d'utilisation.

En termes pratiques, le Readium CLI ingère les fichiers EPUB et génère un Readium Web Publication Manifest (RWPM), un format ouvert destiné à représenter et distribuer des publications. Le processus extrait et infère également des informations telles que les métadonnées d'accessibilité et les détails sur les images (comme la taille et l'identification) qui peuvent être utilisées pour l'optimisation et la compatibilité, et aide à identifier les images décoratives.

Un outil d'écriture complémentaire sera disponible pour tirer parti de l'analyse et des inférences pour enrichir le fichier. Cet outil permettra aux utilisateurs de mettre à jour les fichiers EPUB et de générer une liste lisible par l'homme des points d'attention à aborder lors des opérations de remédiation ultérieures.

À la fin du projet, nous nous attendons à ce que 50 % de la collection soit identifiée comme explicitement accessible. L’autre moitié recevra des métadonnées mises à jour indiquant ce qui manque, et FeniXX disposera de données précises pour envisager la prochaine étape.

Conçu pour l’automatisation et l’intégration, l’outil Readium CLI est idéal pour les développeurs et les créateurs de contenu qui souhaitent automatiser les pipelines de publication ou améliorer les flux de travail d’accessibilité. 

## Héritage : un outil et un modèle pour l’industrie de l’édition

Le projet SOLIMAN marque une avancée substantielle dans l’évaluation et l’information sur l’accessibilité des livres numériques. Il offre un avantage immédiat et ouvre des voies pour des travaux futurs.

D’une part, il élargit l’accès à la littérature en rendant disponibles les informations d’accessibilité de cette vaste collection, permettant aux utilisateurs d’identifier facilement quels ebooks de cette collection sont les mieux adaptés à leurs besoins. C’est un avantage direct pour les personnes handicapées ou ayant des exigences de lecture spécifiques.

D’autre part, FeniXX sait désormais quels efforts sont nécessaires pour rendre davantage d’ebooks de la collection pleinement accessibles et, par conséquent, comment hiérarchiser les prochaines étapes.

Étant donné que l’outil est disponible en open source et déjà utilisé par des acteurs majeurs de l’industrie comme De Marque, les deux aspects ont un impact non seulement sur les collections FeniXX, mais aussi sur un nombre significativement plus important d’ebooks, et l’effet continuera de se propager au cours des prochaines années. Nous nous attendons à une adoption significative de l’outil par d’éminents acteurs de la préservation du patrimoine, tels que les bibliothèques nationales, et espérons que cela s’accompagnera de nouvelles améliorations du Readium CLI ou de solutions dérivées.

L’engagement de FeniXX à sauvegarder le patrimoine culturel est démontré par cet effort, car il s’efforce activement d’éliminer les barrières au contenu numérique et de garantir qu’un lectorat plus large et plus diversifié puisse pleinement découvrir et apprécier ses riches ressources littéraires. Cette entreprise souligne le rôle vital de la conception inclusive dans la promotion d’un accès équitable à la connaissance et à la culture à l’ère numérique.

</div>