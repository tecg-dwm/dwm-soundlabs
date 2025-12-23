# Soundlabs

> UX/UI exercise given at [HEPL](https://hepl.be)

* * *

**Soundlabs** is an educational project, which will be used for `UX`/`UI` courses.

**Note:** the school where the course is given, the [HEPL](https://hepl.be/fr/art560) from Liège, Belgium, is a french-speaking school. From this point, the instruction will be in French.

* * *

## L'objectif de l'application

**Soundlabs** est un magasin de disques numériques où l’écoute est intentionnelle, limitée et orientée vers l’achat, avec en option un accès en streaming permettant d’explorer certains titres (tous les artistes ne donnent pas nécessairement accès à l’ensemble de leur catalogue en streaming).

Le nom de l’application est temporaire. Vous êtes libres de le conserver ou de le personnaliser.
Pensez à utiliser [Namelix](https://namelix.com/) pour explorer d'autres pistes.

Je vous invite à vous approprier le projet et à l’aborder avec un angle personnel.
Si vous êtes fan de rock / rap / techno, réalisez une application pensée pour les amoureux de rock / rap / techno.

Les utilisateurs de ces différents genres ne consomment pas la musique de la même manière : les personas et les expériences proposées ne seront donc pas identiques.

### Mise en garde et précisions diverses

- Ce cahier des charges définit un cadre et un ensemble de fonctionnalités attendues, mais ne garantit en aucun cas la qualité du produit final. Votre application doit rester utilisable, compréhensible et accessible, y compris lorsque vous faites des choix au-delà ou en-deçà des fonctionnalités décrites.
- Soundlabs **n’est pas** une application de streaming généraliste. Il ne s'agit pas de reproduire Spotify ou Apple Music.
- Les informations techniques **sont secondaires (mais nécessaires)** par rapport à la compréhension des parcours et des décisions utilisateur.
- Vous devrez être capable de **justifier chacun de vos choix** par rapport aux objectifs de Soundlabs. ⚠️ Je suis susceptible de vous interroger si vos productions ne reflètent pas votre travail personnel (je vous évalue **vous**, pas une IA, pas un template, ni le travail d’une autre personne).
- Une interface visuellement réussie ne compense pas un manque de hiérarchie ou des parcours confus. La clarté des intentions et des actions prime sur le style graphique.
- Le streaming donne accès à l’écoute, mais ne crée pas de collection. L’achat reste le seul moyen de constituer une bibliothèque personnelle durable.
- L’évaluation porte sur la qualité et la cohérence du produit dans son ensemble, et non sur la quantité de pages ou d’écrans conçus. Produire 50 écrans différents à partir d’un même modèle (par exemple une page album) n’augmentera pas la qualité de votre travail. Qualité > quantité.

## Délivrables attendus
- Un moodboard
- Un prototype focalisé sur l'UX (Priority Guide)
- Un prototype designé (UI)

## Les pages et fonctionnalités

### Onboarding

Expliquez le principe de l’application et ses **deux modes de fonctionnement** : achat et streaming.

### Connexion / Inscription

Il doit être possible d’accéder à l’application **sans compte**, mais il est indispensable d’en créer un pour acheter et/ou streamer de la musique.

Les utilisateurs doivent pouvoir :
- s'inscrire / se connecter à l'aide d'une adresse email et d'un mot de passe&nbsp;;
- récupérer leur mot de passe en cas d’oubli.

Les modes de connexion via des applications tierces sont facultatifs.

Lors de l’inscription, l’utilisateur doit pouvoir choisir son profil (Achat et/ou Streaming).
Il est important que la différence entre ces deux modes soit clairement expliquée.

Si l’utilisateur opte pour un abonnement de streaming, il peut choisir entre trois options&nbsp;:

- Streaming Normal (MP3)&nbsp;: 
  - 320 Kb/s
- Streaming Lossless (Qualité CD)&nbsp;: 
  - 16-bit
  - 44,1kHz
  - 1411 Kb/s
- Streaming Hi-Res&nbsp;: 
  - 24-bit
  - jusqu'à 192 kHz
  - 9200 Kb/s

L'utilisateur doit alors encoder une carte de crédit pour continuer.

### Homepage

Sur la page d’accueil, on peut retrouver différents types de contenus, par exemple&nbsp;:
- Une liste des dernières sorties classées par ordre chronologique&nbsp;;
- les sorties les plus populaires&nbsp;;
- une sélection personnalisée pour l’utilisateur (par exemple en fonction des genres précisés lors de l’onboarding)&nbsp;;
- une sélection d’albums, morceaux ou sorties provenant des artistes favoris de l’utilisateur&nbsp;;
- ...

À vous de définir ce qui est le plus pertinent en fonction des différents états :
- Utilisateur inscrit / non inscrit&nbsp;;
- présence ou non d’artistes favoris&nbsp;;
- etc.

Cela ne signifie pas qu’il faille créer des modèles de pages très différents, mais plutôt adapter le contenu affiché en fonction du flux.

Depuis cette page d’accueil, l’utilisateur doit pouvoir se diriger vers n’importe quelle sous-page.
Cela ne signifie pas qu’il faille obligatoirement repasser par la homepage pour naviguer, mais qu’il s’agit de la première page affichée après l’inscription ou la connexion.

### Toute la musique / Catalogue

Sur cette page, l’utilisateur doit avoir une vue d’ensemble de toute la musique disponible sur l’application.

Le catalogue étant conséquent (des milliers d’albums et de titres), l’utilisateur doit pouvoir filtrer et trier le contenu.

La base minimale est la suivante : 

- Filtrer par :
  - Format : Album / EP / Single / Compilation / &hellip;
  - Genre et sous-genre : Rock / Punk / Rap / Boom Bap / &hellip;
  - Pays d'origine
  - Période : Dates précises / années / mois / &hellip;
- Trier par :
  - Du plus récent au plus ancien
  - Titre / Album / EP de A à Z et de Z à A
  - Les plus écoutés / recherchés / streamés / &hellip;

En fonction du style musical choisi, vous pouvez également envisager d’autres méthodes de filtre ou de tri (BPM, instrumental, tonalité, etc.).

### Page Artiste

Sur la page artiste, on retrouve toute la musique d'un seul artiste. Un peu comme sur la page *Catalogue*.

#### Exemples 
- [Bandcamp](https://backxwash.bandcamp.com/)
- [Rate Your Music](https://rateyourmusic.com/artist/backxwash)
- [Discogs](https://www.discogs.com/artist/7356913-Backxwash)
- [Last.fm](https://www.last.fm/fr/music/Backxwash)

### Page Album / EP / Single / Compilation / ...

Sur cette page, on retrouve l’ensemble des titres de l’album / EP / single / compilation.

- Titre
- Durée totale
- Année
- Genre
- Disponible pour le streaming (Oui/Non)
  - MP3 ?
  - Lossless ?
  - Hi-Res ?
- Prix

Qu’il soit connecté ou non, l’utilisateur doit pouvoir **lancer une écoute** de l’album.
S’il est connecté et dispose d’un abonnement de streaming, il peut écouter les morceaux complets selon les conditions définies.

La lecture se fait via un lecteur audio indiquant clairement quelle partie du morceau est en cours de lecture.

Contrôles minimaux attendus&nbsp;:
- Lecture
- Pause
- Suivant
- Précédent
- Position de la tête de lecture
- Volume

La lecture peut être représentée par&nbsp;:
- [une ligne](https://perceval.bandcamp.com/track/attention-les-chaises) 
- [un spectre sonore (Waveform)](https://soundcloud.com/yanissmusic2/naza-on-va-yaniss-remix)

L'utilisateur doit pouvoir ajouter un ou plusieurs éléments (un ou plusieurs morceaux, l'album complet) en favoris ou dans son panier. Il peut décider de payer directement son achat ou de l'ajouter simplement à son panier.

L'utilisateur doit pouvoir&nbsp;:
- ajouter un ou plusieurs éléments (morceaux ou album complet) en favoris ou dans son panier ;
- payer directement ou ajouter les éléments au panier.
- souscrire à un abonnement de streaming s'il n'en a pas.

Si l’utilisateur est connecté, il peut voir si le contenu fait partie de sa bibliothèque (achats / téléchargements). Dans ce cas, il peut lire le contenu librement, sans restriction, et ne peut plus ajouter un élément déjà acheté à son panier.

Il est possible qu’un seul morceau soit présent sur la page (cas d’un single).

Depuis cette page, il doit être possible&nbsp;: 
- d'accéder aux autres productions du même artiste&nbsp;;
- d'accéder aux productions du même label (comme sur toute la musique mais avec un contenu filtré)&nbsp;;
- d'accéder vers une catégorie de contenu similaire (même genre)&nbsp;;
- et évidemment, de naviguer vers les autres pages de l’application.

#### Exemples : 
- [Bandcamp](https://backxwash.bandcamp.com/album/only-dust-remains)
- [Rate Your Music](https://rateyourmusic.com/release/album/backxwash/only-dust-remains/)
- [Discogs](https://www.discogs.com/master/3987361-Backxwash-Only-Dust-Remains)
- [Last.fm](https://www.last.fm/fr/music/Backxwash/Only+Dust+Remains)

### Page résultat de recherche

La page de résultats de recherche présente les résultats classés par type de contenu.
Par exemple, si un utilisateur recherche *Magugu*, il peut obtenir différents type de résultats : 
- un ou plusieurs artistes
- des albums / EP / singles / compilations ;
- des labels

#### Exemple : 
- [Bandcamp](https://bandcamp.com/search?q=Magugu&item_type)
- [Beatport](https://www.beatport.com/fr/search?q=magugu)
- [Last.fm](https://www.last.fm/fr/search?q=magugu)
- [Discogs](https://www.discogs.com/fr/search?q=magugu&type=all)

### Page Panier et Checkout

Le panier présente un résumé des produits que l’utilisateur souhaite acheter, avec :
- un prix par élément&nbsp;;
- un prix total.

Il est important que l’utilisateur comprenne clairement s’il achète :
- un ou plusieurs morceaux&nbsp;;
- ou l’album complet.

L’utilisateur peut&nbsp;:
- ajouter un code promotionnel&nbsp;;
- payer au prix libre&nbsp;;
- supprimer un élément du panier&nbsp;;
- relancer l’écoute d’un morceau afin de vérifier qu’il s’agit bien du bon contenu.

Si l’utilisateur n’a pas encore de compte, il doit en créer un pour finaliser l’achat.

S’il possède un compte mais n’a pas encore enregistré de moyen de paiement, il doit pouvoir le faire sans quitter le processus de checkout.

### Page profil / Paramètres

Sur cette page, l'utilisateur peut&nbsp;: 

- écouter ses achats&nbsp;;
- télécharger ses achats&nbsp;;
- modifier son adresse email&nbsp;;
- changer son mot de passe&nbsp;;
- supprimer son compte&nbsp;;
- ajouter, modifier ou supprimer un moyen de paiement&nbsp;;
- ajouter, modifier ou supprimer un abonnement de streaming.

Il est probablement pertinent de séparer la page Profil et la page Paramètres.

## Documentation

### Exemples
- [Rate Your Music](https://rateyourmusic.com/)
- [Discogs](https://www.discogs.com)
- [Beatport](https://www.beatport.com)
- [Decks](https://www.decks.de/)
- [Bandcamp](https://bandcamp.com/)
- [Traxsource](https://www.traxsource.com/)
- [Soundcloud](https://soundcloud.com/)
- [Juno](https://www.junodownload.com/)
- [Last.fm](https://www.last.fm/fr/)
- [Youtube Music](https://music.youtube.com/)
- [Qobuz](https://www.qobuz.com/fr-fr/discover)
- [Tidal](https://tidal.com/)
- [Record Club](https://record.club/)
- [Deezer](https://www.deezer.com/fr/)

### Articles
- [Web Ecommerce guidelines (NN Group)](https://www.nngroup.com/articles/web-ux-study-guide/#toc-web-ecommerce-13)
- [Les diviseurs visuels](https://medium.muz.li/ux-details-visual-dividers-in-user-interfaces-8afec368535d)

### Conseils
- Travaillez d’abord en basse fidélité (UX Flow)
- Rendez les pages importantes facile d'accès.
- Pensez à envisager des barres de progression ou un autre moyen de situer la progression lors des processus complexes qui pourraient justifier ce genre d'éléments (onboarding, checkout, etc.)
- Pensez à utiliser des modes d'affichages adaptés au contenu et à sa densité (grille, liste, etc.).
- Pensez systématiquement aux différents états de l’utilisateur : non connecté, connecté sans abonnement, abonné, acheteur, acheteur + abonné. Une même page peut (et doit) se comporter différemment selon ces états.
- Essayez de limiter le nombre de composants d’interface différents (cartes, listes, boutons, lecteurs).
Un petit nombre de composants bien maîtrisés vaut mieux qu’une grande variété mal cohérente.
- Soignez la hiérarchie de l’information. Posez-vous systématiquement la question : Qu’est-ce qui est le plus important sur cet écran ? Qu’est-ce qui peut passer au second plan ?
- Inspirez-vous, mais ne copiez pas. Les références fournies sont là pour nourrir votre réflexion, pas pour être reproduites à l’identique.
- Un test utilisateur simple (1 ou 2 personnes -> pas un autre membre de la classe) peut suffire à révéler des problèmes importants.
  