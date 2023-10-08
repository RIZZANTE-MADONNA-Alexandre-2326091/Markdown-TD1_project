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
La complexité de cette algorithme est de $O(log_{2}(n))$.

### 2<SUP>ème</SUP> Page:


### 3<SUP>ème</SUP> Page:


### 4<SUP>ème</SUP> Page:


### 5<SUP>ème</SUP> Page:
Voici une capture d'écran sur lequel on a testé l'alggorithme:
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
