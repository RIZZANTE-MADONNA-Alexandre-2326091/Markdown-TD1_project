# Projet de 1<SUP>ère</SUP>:
Je vais présenter mon **projet** de NSI en _première_.
  
C'était un projet à deux dans lequel il fallait faire un site web sur un alogrithme travaillé durant l'année. J'ai choisi de faire un site Web sur la recherche dichotomique. Ce site est composé de 5 pages:index: la page d'acceuil, présentation:la page de présentation du projet, auteurs: la page de renseignements sur les auteurs du projet, rapport: rapport de projet et algorithme qui est la page de test de l'algorithme. Il ya aussi un dossier pour le fichier CSS et un dossier pour les fichiers Javascript.
Sur ce projet, on a utilisé 3 langages:
|           HTML           |              CSS               |                Javascript               |
|--------------------------|--------------------------------|-----------------------------------------|
|Créer le squelette du site|Réaliser la mise en page du site|Pour insérer un script, ici un algorithme|
# Sommaire:
[Page1](https://github.com/RIZZANTE-MADONNA-Alexandre-2326091/Markdown-TD1_project/blob/main/README.md#1%C3%A8re-page)
[Page2](https://github.com/RIZZANTE-MADONNA-Alexandre-2326091/Markdown-TD1_project/blob/main/README.md#2%C3%A8me-page)
[Page3](https://github.com/RIZZANTE-MADONNA-Alexandre-2326091/Markdown-TD1_project/edit/main/README.md#3%C3%A8me-page)
[Page4](https://github.com/RIZZANTE-MADONNA-Alexandre-2326091/Markdown-TD1_project/edit/main/README.md#4%C3%A8me-page)
[Page5](https://github.com/RIZZANTE-MADONNA-Alexandre-2326091/Markdown-TD1_project/edit/main/README.md#5%C3%A8me-page)
[CSS + JS](https://github.com/RIZZANTE-MADONNA-Alexandre-2326091/Markdown-TD1_project/edit/main/README.md#css--js)
### 1<SUP>ère</SUP> Page:
Sur cette page d'acceuil, on présente le contenu du site. On présente comment naviguer sur le site, l'ordre des pages à visiter et on conseille aussi les utilisateurs quelle navigateur est-il recommandé.

### 2<SUP>ème</SUP> Page:
Cette page présente le projet et l'algorithme. On explique le fonctionnement de l'algorithme ainsi que l'éfficacité de l'algorithme.

L'algorithme se passe dans un tableau trié et on cherche une valeur dedans. On prend le milieu et on compare cette valeur au nombre cherché. Si le milieu est inférieur, le max devient le milieu ou le min devient le milieu et on continu jusqu'à trouver la valeur ou non.

La complexité de cette algorithme est de $O(log_{2}(n))$, en effet:
>floor(log2(1024)+1) = 11
>
>floor(log2(2048)+1) = 12
### 3<SUP>ème</SUP> Page:
Cette troisième page présente les auteurs du site. On se présente, donne nos goûts et pourquoi avoir choisi la spécialité NSI car nous étions en première générale.

### 4<SUP>ème</SUP> Page:
Cette page est le rapport. Dedans, on peut lire comment nous nous sommes répartis les tâches, quel est l'utilité de chaque document, le peuso-code des fonctions Javascript, les tests éffectués durant la création du projet et enfin la conclusion critique des membres du projet où l'in donne notre avis sur le projet, sur ce qu'il pourrait être amélioré.

### 5<SUP>ème</SUP> Page:
Voici une capture d'écran sur lequel on a testé l'algorithme:
On demande à l'utilisateur d'entrer la taille du tableau choisi et le nombre à chercher dans ce tableau. L'utlisateur doit valider son choix, sinon, les valeurs ne sont pas enregistrées. Enfin, l'utilisateur clique sur le bouton **"Activer l'algorithme"** et l'algorithme se lance. L'utilisateur pourra voir le déroulement étape par étape de l'algorithme.
![Capture d'écran de la page pour tester l'algorithme.](https://github.com/RIZZANTE-MADONNA-Alexandre-2326091/Markdown-TD1_project/blob/main/Recherche%20dico.PNG)
> [!WARNING]
> Si la taille du tableau est supérieur à 100, l'algorithme plante.

### CSS + JS:
Dans le fichier CSS, on a mis une photo sur la page d'acceuil. Sur tout le site, on a mis une bordure noire avec une couleur d'arrière ~~plane~~ plan en vert clair. Les bordures sont arrondis. Nous avons donc indenté tout le texte au centre dans la partie verte et le menu sur la bordure haute. On a mis aussi un bouton pour afficher ou non le menu grâce à un script Javascript et les liens pour naviguer sur le site.

Avec Javascript, j'ai réalisé l'algorithme. J'ai créer tout d'abord une fonction générant un nombre aléatoire entre 0 et 100, puis une fonction qui permet de récupérer la taille du tableau entrée par l'utilisateur dans le formulaire, puis une fonction qui permet de récupérer le nombre à chercher entrée par l'utilisateur dans le formulaire. Enfin, dans la fonction de l'algorithme, je génère un tableau de longueur de la fonction pour la taille du tableau avec des nombres aléatoires entre 0 et 100, puis je trie la liste. Enfin, je calcule le minimum, maximum et le milieu et je compare si le milieu est égale au nombre recherché, sinon le minimum ou le maximum devient le milieu en fonction du nombre recherché jusqu'à trouver le nombre et le nombre est bien présent, ou la boucle for s'arrête et le nombre n'est pas présent.

Voici le code de la boucle for de l'algorithme:


` for (var index = 0; index <= liste.length; index++){
        while (debut <= fin){
            milieu = Math.floor((debut + fin) / 2);
            index += 1;
            if (liste[milieu] == nombre_demande){
                affichage__etape_algorithme.innerHTML += "L'algorithme a trouvé que le nombre du milieu est égale au nombre recherché:(" + nombre_demande + ") au bout de " + index + " itérations. La recherche dichotomique s'arrête donc.<br/>";
				return
			}
            else{
                if (nombre_demande < liste[milieu]){
                    fin = milieu - 1;
					affichage__etape_algorithme.innerHTML += "L'algorithme a divisé la liste en deux. Le nombre du milieu est " + liste[milieu] + ", supérieur au nombre recherché:" + nombre_demande + ". L'algorithme continue.<br/>";
				}
                else{
                    debut = milieu + 1;
					affichage__etape_algorithme.innerHTML += "L'algorithme a divisé la liste en deux. Le nombre du milieu est " + liste[milieu] + ", supérieur au nombre recherché:" + nombre_demande + ". L'algorithme continue.<br/>";
				}
			}
		}
       affichage__etape_algorithme.innerHTML += "L'algorithme n'a pas trouvé le nombre recherché égal à " + nombre_demande + " au bout de "+ index +" itérations. La recherche dichotomique s'arrête donc.<br/>";
	   return`.

Voici mon projet de première sur un site web. J'ai apprécié de le faire car j'ai vraiment appris comment en crée un.
