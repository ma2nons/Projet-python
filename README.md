Projet Python pour la Data Science
Autrices et auteur : Margaux Gibault, Manon Neau, Gauthier Viviès (2026).

Sujet : Influence de l'emploi sur les résultats scolaires à l'échelle départementale.

Les résultats scolaires sont un sujet fréquemment étudié en sociologie, dans la mesure où ils reflètent l'adéquation entre un individu et l'institution de l'Ecole. 
Ces résultats scolaires sont doublement liés à l'emploi : d'une part, de meilleurs résultats scolaires sont en général corrélés à une plus grande facilité à trouver un emploi et à s'insérer dans le monde professionnel.
D'autre part, on pourrait envisager que l'accès à l'emploi des parents d'un élève ait un impact sur les résultats scolaires de ce dernier, via la transmission d'un capital culturel et économique (Bourdieu, La reproduction sociale). Il s'agit de considérer par exemple, qu'avoir un parent au chômage ou bénéficiant du RSA, influe sur les résultats d'un enfant. 

Nous décidons ici de laisser de côté la première partie, c'est-à-dire l'impact des résultats scolaires sur l'employabilité pour nous concentrer sur la deuxième partie : l'impact de l'emploi sur les résultats scolaires.

Problématique : L'emploi des actifs influe-t-il sur les résultats scolaires des lycéens ?

Ici, nous mesurons les résultats scolaires comme les résultats au baccalauréat général et technologique par lycée. Nous sommes pleinement conscients que ces informations ne reflètent que partiellement le niveau scolaire des élèves, notamment car tout le monde ne passe pas un baccalauréat général ou technologique : une partie des étudiants arrête les études avant cela, et une autre partie s'oriente vers des filières plus techniques : certificat d'aptitude professionnelle (CAP) ou baccalauréat professionnel. 
Néanmoins, une proportion non négligeable des français passe un baccalauréat technologique ou général, et nous avons été également contraints par la disponibilité des données : nous avons pu trouver des données précises de grande qualité surtout sur cet examen. 

OU INTRO 2 (PROPOSITION)

Sujet: Influence de l’emploi sur les résultats au baccalauréat à l’échelle départementale

Depuis les années 1950 et plus particulièrement depuis les années 1960-1970 avec la sociologie bourdieusienne (Les Héritiers (1964), La Reproduction (1970)), la massification scolaire a posé des questions d’égalité des chances et de démocratisation. Cette démocratisation fut impressionnante, et s’observe notamment à travers les chiffres du baccalauréat: comme le mentionne Marie Duru-Bellat dans son ouvrage L’inflation scolaire: Les désillusions de la méritocratie, alors qu’en 1950 5% d’une classe d’âge obtenait son baccalauréat, 69% de la classe d’âge actuelle l’obtient. Néanmoins, comme l’autrice le souligne, cette démocratisation s’est accompagnée d’une inflation du diplôme, dévalorisant le baccalauréat. 
A l’heure de cette dévalorisation du baccalauréat - diplôme qui cependant reste important selon Eric Maurin qui dans son ouvrage La peur du déclassement rappelle qu’en 2008, parmi les jeunes sortis de l’école depuis moins de 5 ans, 47% des non-diplômés étaient au chômage contre 7% des diplômés du supérieur (bac +2)-  une question se pose: 

le capital économique des parents joue-t-il encore dans l’obtention du baccalauréat? 

Nous choisissons dans notre étude d’approximer le capital économique par des variables telles que le taux d’activité, ou encore le taux de bénéficiaires du RSA par département. Nous nous intéresserons aux résultats du baccalauréat général, technologique et professionel.



Parcoursup ? @Gauthier 

Nous avons choisi l'échelle départementale car cette échelle nous permettait d'obtenir le plus juste équilibre possible entre exhaustivité et hétérogéneité.

L'échelle académique ou régionale aurait fait disparaitre trop de spécificités et aurait trop lissé les résultats. De plus, nous aurions eu très peu de valeurs car il existe seulement 30 académies (dont 5 académies d'outre mer, que nous sommes parfois contraints d'exclure du fait de leurs valeurs extrêmes).

A contrario, une échelle plus restreinte telle que le bassin de vie ou la commune était compliquée à mettre en place, notamment du fait d'un complexe croisement des bases de données : il est notamment complexe d'établir une correspondance des lycées à des bassin de vie ou des communes. En effet, étant donné qu'un lycée situé dans une ville possède un secteur bien plus large que cette ville et que nous ne disposions pas de données précises sur les cartes scolaires (qui par ailleurs, connaissent de nombreuses dérrogations, du fait de choix d'options, d'internat...), nous ne pouvions pas mettre chaque lycée en parallèle du niveau d'emploi de son bassin ou de ses communes. Nous ne pouvions ainsi, par exemple, pas comparer des espaces ruraux et urbains.

Nous mesurons l'emploi de plusieurs manières : nous nous sommes penchés sur le taux de chômage, sur le nombre de bénéficiaires du RSA, sur le revenu médian, mais également sur la composition de l'emploi d'un département.
Nous ne disposons malheureusement pas de données liant à l'échelle individuelle le parcours de vie professionnel de parents et les résultats scolaires des enfants. Nous comparons donc l'emploi moyen d'un département et les résultats moyens des lycéens de ce même département.

Données
Nous exploitons des données de trois types :

résultats au baccalauréat général au niveau départemental (par lycée - entre 2012 et 2023) ;
répartition des allocataires du RSA par département (2023);
principaux indicateurs de population active et chômage;
résultats et choix d'orientations à la fin de parcoursup (2023);
indicateurs de revenus par département;

COMPLETER

Ces données sont obtenues par plusieurs sources différentes, respectivement :

les données publiques du Ministère de l'éducation nationale,
les données publiques de Insee;
les données publiques de la Caisse Nationale des Allocations Familiales;
les données publiques parcoursup 2023;
les données publiques Filosfi 2023 de l'INSEE;

COMPLETER

Ces données sont issues du site data.gouv.fr 

Reproduction du projet
Installation. Cloner le projet.
git clone https://github.com/username/Projet-python.git
cd Projet-python

Lire "Téléchargement_données_info" pour plus de précisions sur la manière de télécharger les données si vous souhaitez faire tourner le code. 

Installer les dépendances Python à l’aide de la commande :

!pip install pandas fiona shapely pyproj rtree 
!pip install contextily
!pip install geopandas
!pip install topojson
!pip install py7zr geopandas openpyxl tqdm s3fs ipywidgets --quiet
!pip install PyYAML --quiet
!pip install cartiflette --quiet
!pip install statsmodels

COMPLETER

Lancement. 

Ouvrir le notebook synthèse.ipynb, qui constitue le rapport analytique principal du projet.

Structure du repo
dossier data : dossier contenant les données brutes et receptionnant les données nettoyées,

COMPLETER (structure prise sur un autre repo)