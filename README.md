Projet Python pour la Data Science
Autrices et auteur : Margaux Gibault, Manon Neau, Gauthier Viviès (2026).

Sujet : Influence de l'emploi sur les résultats scolaires à l'échelle départementale.

Les résultats scolaires sont un sujet fréquemment étudié en sociologie, dans la mesure où ils reflètent l'adéquation entre un individu et l'institution de l'Ecole. 
Ces résultats scolaires sont doublement liés à l'emploi : d'une part, de meilleurs résultats scolaires sont en général corrélés à une plus grande facilité à trouver un emploi et à s'insérer dans le monde professionnel.
D'autre part, on pourrait envisager que l'accès à l'emploi des parents d'un élève ait un impact sur les résultats scolaires de ce dernier. Il s'agit de considérer par exemple, qu'avoir un parent au chômage ou bénéficiant du RSA, influe sur les résultats d'un enfant. 

Nous décidons ici de laisser de côté la première partie, c'est-à-dire l'impact des résultats scolaires sur l'employabilité pour nous concentrer sur la deuxième partie : l'impact de l'emploi sur les résultats scolaires.

Problématique : L'emploi des actifs influe-t-il sur les résultats scolaires des lycéens ?

Ici, nous mesurons les résultats scolaires comme les résultats au baccalauréat général et technologique par lycée. Nous sommes pleinement conscients que ces informations ne reflètent que partiellement le niveau scolaire des élèves, notamment car tout le monde ne passe pas un baccalauréat général ou technologique : une partie des étudiants arrête les études avant cela, et une autre partie s'oriente vers des filières plus techniques : certificat d'aptitude professionnelle (CAP) ou baccalauréat professionnel. 
Néanmoins, une proportion non négligeable des français passe un baccalauréat technologique ou général, et nous avons été également contraints par la disponibilité des données : nous avons pu trouver des données précises de grande qualité surtout sur cet examen. 

Parcoursup ? @Gauthier 

Nous avons choisi l'échelle départementale car cette échelle nous permettait d'obtenir le plus juste équilibre possible entre exhaustivité et hétérogéneité.

L'échelle académique ou régionale aurait fait disparaitre trop de spécificités et aurait trop lissé les résultats. De plus, nous aurions eu très peu de valeurs car il existe seulement 30 académies (dont 5 académies d'outre mer, que nous sommes parfois contraints d'exclure du fait de leurs valeurs extrêmes).

A contrario, une échelle plus restreinte telle que le bassin de vie ou la commune était compliquée à mettre en place, notamment du fait d'un complexe croisement des bases de données : il est notamment complexe d'établir une correspondance des lycées à des bassin de vie ou des communes. En effet, étant donné qu'un lycée situé dans une ville possède un secteur bien plus large que cette ville et que nous ne disposions pas de données précises sur les cartes scolaires (qui par ailleurs, connaissent de nombreuses dérrogations, du fait de choix d'options, d'internat...), nous ne pouvions pas mettre chaque lycée en parallèle du niveau d'emploi de son bassin ou de ses communes. Nous ne pouvions ainsi, par exemple, pas comparer des espaces ruraux et urbains.

Nous mesurons l'emploi de plusieurs manières : nous nous sommes penchés sur le taux de chômage, sur le nombre de bénéficiaires du RSA, mais également sur la composition de l'emploi d'un département.
Nous ne disposons malheureusement pas de données liant à l'échelle individuelle le parcours de vie professionnel de parents et les résultats scolaires des enfants. Nous comparons donc l'emploi moyen d'un département et les résultats moyens des lycéens de ce même département.

Données
Nous exploitons des données de trois types :

résultats au baccalauréat général au niveau départemental (par lycée - entre 2012 et 2023) ;
répartition des allocataires du RSA par département (2023);
principaux indicateurs de population active et chômage;

COMPLETER

Ces données sont obtenues par plusieurs sources différentes, respectivement :

les données publiques du Ministère de l'éducation nationale,
les données publiques de Insee;
les données publiques de la Caisse Nationale des Allocations Familiales;

COMPLETER

Ces données sont issues du site data.gouv.fr 

Reproduction du projet
Installation. Cloner le projet.
git clone https://github.com/username/Projet-python.git
cd Projet-python


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