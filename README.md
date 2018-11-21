# projetdusemestre     
1.	Architecture globale de l’application :
Qu'est-ce qu'un service Web ?
La technologie des services Web est un moyen rapide de distribution de l'information entre clients, fournisseurs, partenaires commerciaux et leurs différentes plates-formes. Les services Web sont basés sur le modèle SOA .
D'autres technologies telles que RMI, DCOM et CORBA ont précédemment adopté ce style architectural mais ont généralement échoué en raison de la diversité des plates-formes utilisées dans les organisations et aussi parce que leur usage n'était pas adapté à Internet (problème de passage à travers des FireWalls, etc.) d'où la lenteur, voire l'absence de réponses sur ce réseau. Les applications réparties fondées sur ces technologies offrent des solutions caractérisées par un couplage fort entre les objets. Les solutions proposées par les services Web, permettent néanmoins un couplage moins fort. De plus, l'utilisation des technologies standards du Web telles HTTP et XML par les services Web facilite le développement d'applications réparties sur Internet, et permet d'avoir des applications très faiblement couplées. L'intégration est sans doute le facteur essentiel qui favorise l'utilisation des services Web.
Definition :
Un service Web est un composant logiciel identifié par une URI, dont les interfaces publiques sont définies et appelées en XML. Sa définition peut être découverte par d'autres systèmes logiciels. Les services Web peuvent interagir entre eux d'une manière prescrite par leurs définitions, en utilisant des messages XML portés par les protocoles Internet.
Les caractéristiques d'un service Web
La technologie des services Web repose essentiellement sur une représentation standard des données (interfaces, messageries) au moyen du langage XML. Cette technologie est devenue la base de l'informatique distribuée sur Internet et offre beaucoup d'opportunités au développeur Web.
Un service Web possède les caractéristiques suivantes :
•	il est accessible via le réseau ;
•	il dispose d'une interface publique (ensemble d'opérations) décrite en XML ;
•	ses descriptions (fonctionnalités, comment l'invoquer et où le trouver ?) sont stockées dans un annuaire ;
•	il communique en utilisant des messages XML, ces messages sont transportés par des protocoles Internet (généralement HTTP, mais rien n'empêche d'utiliser d'autres protocoles de transfert tels : SMTP, FTP, BEEP... ) ;
•	l'intégration d'application en implémentant des services Web produit des systèmes faiblement couplés, le demandeur du service ne connaît pas forcément le fournisseur.
Ce dernier peut disparaître sans perturber l'application cliente qui trouvera un autre fournisseur en cherchant dans l'annuaire.


2.	Architecture de la couche donnée :
MVC (Model-View-Controller) est un style d’architecture de logiciel très populaire vous permettant d’être efficace & structuré lors du développement d’un projet.
![370px-modelemvc](https://user-images.githubusercontent.com/44054584/48837438-a802f700-ed85-11e8-8f24-8bfd1f4b4cbf.png)

Le M, modèle (model) représente les données et ne fait rien d’autre, il ne dépend donc pas des vues & des contrôleurs.
Le V, vue (view) affiche les données que le modèle contient à l’utilisateur, ex : formulaire, bouton, etc... (Un modèle peut contenir plusieurs vues)
Le C, contrôleur (controller) traite les données de l’utilisateur, il dépend et interagit avec le modèle ainsi que la vue (Dans certains cas il est possible que la vue & le contrôleur soient le même objet).
Pourquoi utiliser le modèle MVC ?
Le modèle MVC vous permet d’être plus efficient en vous donnant la possibilité de réutiliser le même code plusieurs fois dans d’autres applications similaire à celle que vous avez et ainsi que de séparer votre structure en multiple calques. Cette combinaison vous offre une meilleure maintenance de votre projet et vous facilite la tâche durant les tests unitaires & vous permet de travailler à plusieurs sur un même projet (ex : Le développeur back-end peut mettre en place la structure sans intervenir sur le front-end, vice-versa).
Un autre avantage est le fait qu’il y a peu d’accrochage entre les vues, les modèles et les contrôleurs, ce qui vous permet d’avoir un code propre où les fonctions & les classes peuvent être facilement réécrite & optimisé.
 



3.	La maniére de gestion des demandes des clients :
 ![capture](https://user-images.githubusercontent.com/44054584/48837631-2364a880-ed86-11e8-8f7c-f67fb1379b86.PNG)



4.	Les technologies choisies :
JAVA : 
 
Le langage Java est un langage de programmation informatique orienté objet créé par James Gosling et Patrick Naughton, employés de Sun Microsystems, avec le soutien de Bill Joy (cofondateur de Sun Microsystems en 1982), présenté officiellement le 23 mai 1995 au SunWorld. La particularité et l'objectif central de Java est que les logiciels écrits dans ce langage doivent être très facilement portables sur plusieurs systèmes d’exploitation tels que UNIX, Windows, Mac OS ou GNU/Linux, avec peu ou pas de modifications. Pour cela, divers plateformes et frameworks associés visent à guider, sinon garantir, cette portabilité des applications développées en Java.
NetBeans :
 
NetBeans est un environnement de développement intégré (EDI), placé en open source par Sun en juin 2000 sous licence CDDL (Common Development and Distribution License) et GPLv2. En plus de Java, NetBeans permet la prise en charge native de divers langages tels le C, le C++, le JavaScript, le XML, le Groovy, le PHP et le HTML, ou d'autres (dont Python et Ruby) par l'ajout de greffons. Il offre toutes les facilités d'un IDE moderne (éditeur avec coloration syntaxique, projets multi-langage, refactoring, éditeur graphique d'interfaces et de pages Web).
Compilé en Java, NetBeans est disponible sous Windows, Linux, Solaris (sur x86 et SPARC), Mac OS X ou sous une version indépendante des systèmes d'exploitation (requérant une machine virtuelle Java). Un environnement Java Development Kit JDK est requis pour les développements en Java.
NetBeans constitue par ailleurs une plate forme qui permet le développement d'applications spécifiques (bibliothèque Swing (Java)). L'IDE NetBeans s'appuie sur cette plate forme.
L'IDE Netbeans s'enrichit à l'aide de greffons.

SQL : 
 
SQL (sigle de Structured Query Language, en français langage de requête structurée) est un langage informatique normalisé servant à exploiter des bases de données relationnelles. La partie langage de manipulation des données de SQL permet de rechercher, d'ajouter, de modifier ou de supprimer des données dans les bases de données relationnelles.













architecture monolithique
   Une architecture monolithique représente le modèle traditionnel unifié de conception d'un programme informatique.
Dans ce contexte, « monolithique » signifie formé d'un seul bloc. Un logiciel monolithique est conçu pour être autonome ; ses composants sont interconnectés et interdépendants plutôt qu'associés de manière flexible comme dans le cas des programmes modulaires. Dans ce type d'architecture étroitement intégrée, chaque composant et ceux qui lui sont associés doivent être présents pour permettre l'exécution ou la compilation du code.
De plus, pour mettre à jour un composant du programme, il faut réécrire toute l'application, tandis que dans une application modulaire, chaque module (un microservice, par exemple) peut être modifié sans que cela se répercute sur les autres parties du programme. Dans une architecture modulaire, une modification apportée à un élément a moins de risque d'entraîner des changements non prévus au sein d'autres éléments, puisque les modules sont relativement indépendants. Les programmes modulaires se prêtent aussi plus facilement à des processus itératifs que les programmes monolithiques.
Cependant, les architectures monolithiques comportent également des avantages. En général, elles offrent un meilleur rendement que les approches modulaires, telles que l'architecture de microservices (MSA, MicroService Architecture), et peuvent être plus faciles à tester et à déboguer, car avec moins d'éléments, le nombre de variables à prendre en compte est moins élevé.

Microservices

Sauter à la navigationSauter à la recherche
En informatique, les microservices sont un style d'architecture logicielle à partir duquel un ensemble complexe d'applications est décomposé en plusieurs processus indépendants et faiblement couplés, souvent spécialisés dans une seule tâche. Les processus indépendants communiquent les uns avec les autres en utilisant des API langage-agnostiques.
Des API REST sont souvent employées pour relier chaque microservice aux autres. Un avantage avancé est que lors d'un besoin critique en une ressource, seul le microservice lié sera augmenté[pas clair], contrairement à la totalité de l'application dans une architecture classique, par exemple une architecture trois tiers. Cependant, le coût de mise en place, en raison des compétences requises, est parfois plus élevé.

Détails
•	Les services individuels sont simples à remplacer
•	Les services sont conçus pour leur utilité spécifique (par exemple la facturation, la chaîne logistique, l'interface...)
•	L'architecture est plus symétrique que hiérarchique (passage d'une architecture client-serveur à une architecture de plusieurs entités communicantes)
•	L'architecture facilite le déploiement continu du code

