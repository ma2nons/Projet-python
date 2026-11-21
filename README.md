Projet Python pour la Data Science
Autrices et auteur : Margaux Gibault, Manon Neau, Gauthier Viviès (2026).

Sujet : Influence de l'emploi sur les résultats scolaires à l'échelle départementale

blablabla pourquoi on a choisi ce sujet

Problématique : Un  ?

Ici, nous mesurons les résultats scolaires comme les résultats au baccalauréat général et technologique par lycée. Nous sommes pleinement conscients que ces informations ne reflètent que partiellement le niveau scolaire des élèves, notamment car tout le monde ne passe pas un baccalauréat général ou technologique : une partie des étudiants arrête les études avant cela, et une autre partie s'oriente vers des filières plus techniques : certificat d'aptitude professionnelle (CAP) ou baccalauréat professionnel. 
Néanmoins, une proportion non négligeable des français passe un baccalauréat technologique ou général, et nous avons été également contraints par la disponibilité des données : nous avons pu trouver des données précises de grande qualité surtout sur cet examen.

Parcoursup ?

Nous sommes également conscients que les résultats d'un examen passé autour de 18 ans sont probablement plus teintés socialement les résultats d'un examen passé, par exemple, autour de 6 ans. Comme le suggère la sociologie, notamment Bourdieusienne, l'Ecole renforce les inégalités, notamment en promouvant une culture légitime. Ainsi, de moindres résultats au baccalauréat n'impliquent pas de moindres capacités cognitives.

Nous mesurons l'emploi de plusieurs manières : nous nous sommes penchés sur le taux de chômage, sur le nombre de bénéficiaires du RSA, mais également sur la composition de l'emploi d'un département.

Données
Nous exploitons des données de trois types :

résultats au baccalauréat général au niveau départemental (par lycée) entre 2012 et 2023 ;


Ces données sont obtenues par  sources différentes, respectivement :

fichiers CSV fournis par l'Injep (
requête via l'API Melodi de l'INSEE.
La base de données de l'INJEP a l'avantage de présenter une classification fine des licenciés selon leurs caractéristiques socio-démographiques (âge, sexe, département d'exercice).

Reproduction du projet
Installation. Cloner le projet.
git clone https://github.com/username/nom_du_repo.git
cd nom_du_repo 

 Installer les dépendances Python à l’aide de la commande :

pip install -r requirements.txt
Lancement. Ouvrir le notebook main.ipynb, qui constitue le rapport analytique principal du projet.

Structure du repo
dossier data : dossier contenant les données brutes et receptionnant les données nettoyées,
dossier jo: package permettant la visualisation interactive des données,
dossier traitement: package permettant la récupération et le nettoyage des données,
dossier model: package permattant la modélisation des données,
fichier main.ipynb : notebook principal servant de rapport analytique et de support de restitution.