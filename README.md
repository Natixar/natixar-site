# [Natixar](https://natixar.netlify.app)

[![Netlify Status](https://api.netlify.com/api/v1/badges/5eff4369-e3e0-4d9e-b9d9-ebbc91bbd27e/deploy-status)](https://app.netlify.com/projects/natixar/deploys)

Ce projet contient le code source du site web de Natixar, une application web développée avec Hugo et déployée sur Netlify. Le site est accessible à l'adresse [natixar.netlify.app](https://natixar.netlify.app).

## Configuration des blocs

Ces éléments de configuration sont pris en charge par un modèle partiel commun à tous les blocs.

### Éléments de contenu (content)

Les éléments de contenu sont liés aux données textuelles et aux métadonnées spécifiques au bloc. Voici les éléments pris en charge :

1. **`$block.content.title`**

- Titre du bloc, affiché dans une balise `<h1>`.
- Peut être transformé avec markdownify et emojify.

2. **`$block.content.subtitle`**

- Sous-titre du bloc, affiché dans une balise `<p>`.
- Peut également être transformé avec markdownify et emojify.

3. **`$block.content.text`**

- Contenu textuel brut du bloc.
- Utilisé pour détecter des shortcodes spécifiques comme gallery via une recherche avec findRE.

### Éléments de style (design)

Les éléments de style définissent l'apparence visuelle du bloc. Voici les propriétés prises en charge :

#### Fond (background)

1. **`$block.design.background.color`**

Couleur de fond du bloc (CSS background-color).
$block.design.background.gradient_start et $block.design.background.gradient_end

Définissent un dégradé linéaire (CSS background-image: linear-gradient).
L'angle du dégradé peut être défini avec $block.design.background.gradient_angle.

2. **`$block.design.background.video.filename`**

Vidéo de fond (fichier dans le dossier media/).
Peut être inversée horizontalement avec $block.design.background.video.flip.

3. **`$block.design.background.image.filename`**

- Image de fond (fichier dans le dossier media/).
- Supporte les formats comme webp et applique des transformations (ex. redimensionnement).
- Gère les propriétés suivantes :
  - size : Taille de l'image (actual, cover, contain).
  - position : Position de l'image (CSS background-position).
  - filters.brightness : Filtre de luminosité (CSS filter: brightness).

#### Espacement (spacing)

1. **`$block.design.spacing.padding`**

- Definit les marges internes (CSS `padding`).

#### Clip Path

1. **`$block.design.clip_path`**
   
- Définit une forme de découpe pour le bloc (CSS clip-path).

#### Style CSS personnalisé

1. **`$block.design.css_style`**

- Ajout de styles CSS personnalisés.

#### Classes CSS

1. **`$block.design.css_class`**
 
- Ajout de classes CSS personnalisées au bloc.

#### Colonnes

1. **`$block.design.columns`**
 
- Définit le nombre de colonnes pour le contenu du bloc (par défaut : 1).

#### Autres fonctionnalités spécifiques

##### Gestion des shortcodes spécifiques

- Détection de gallery pour activer des fonctionnalités comme has_gallery.

##### Gestion des widgets spéciaux

- Exemple : Le type de bloc slider ajoute des classes et attributs spécifiques pour un carrousel.

##### Identifiant unique du bloc

- Généré avec $block.id ou un identifiant par défaut basé sur le type de bloc.

##### Conteneur (container)

- Utilisation conditionnelle d'un conteneur Bootstrap (`<div class="container">`).