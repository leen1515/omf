# Oh my food

https://leen1515.github.io/omf/
Oh my food est une application en cours de développpement. Ici est l'interface front-end codée avec HTML et CSS. Il est produit avec SASS, postcss, autoprefixer et NODE.js.

## Installation

clonez ou décompressez le fichier dans votre répertoire local, installez node.js et actionnez l'installation des dépendances. Mettre en route SASS si la modification du CSS s'avère nécessaire. Enfin finaliser avec autoprefixer pour la gestion des styles sur tous les navigateurs

```bash
npm i
npm run sass
npm run prefix
```

## Usage
Les fichiers SCSS sont repartis par groupe. Le layout, les composants, les variables, les mixins et les fonctions sont compartimentés dans des dossiers différents. Le main.scss import tous les fichiers utilisés. Le @charset utf-8 est présent pour minimiser les conflits avec les lettres latines et la gestion des accents.

```scss
@charset 'utf-8';

@import './utils/variables.scss';

@import './utils/mixin-function.scss';

@import './layout/base.scss';

@import './layout/head.scss';

@import './layout/form.scss';

@import './layout/guide.scss';

@import './layout/restaurants.scss';

@import './components/cards.scss';

@import './components/loader.scss';

@import './layout/footer.scss';

@import './layout/menu.scss';
```

## Structure HTML
Pour les étiquettes des recettes, une proposition sous forme de balise input de type radio a été réalisé dans l'objectif de faciliter l'accueil des variables.
```html
<div class="menu__recette" id="menu__recette-1">
            <input
              class="recette__validation"
              type="radio"
              id="raviolesD"
              name="entrees"
            />
            <div class="recette__description">
              <h3>Ravioles de foie gras</h3>
              <p class="description__detail">
                Accompagnés de leur crème à la truffe
              </p>
            </div>
            <p class="prix-bouton__prix">25€</p>
            <div class="menu__prix-bouton">
              <div class="back--check">
                <label for="raviolesD" class="border--check">
                  <i class="fa-solid fa-check fa-1x"></i
                ></label>
              </div>
            </div>
          </div>
```
## Contribution

Disponible pour le projet Oh my Food, la partie back-end est en cours de développement et s'intégrera sans difficulté à la partie front-end.  

## License
©openclassrooms