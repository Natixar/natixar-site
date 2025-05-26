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
  - parallax : l'image ne défile pas avec le bloc en scrollant, mais elle est recouverte par le bloc suivant (vrai par défaut).

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


### Configuration du bloc `contact`

#### Contenu (content)

Ces paramètres définissent les données textuelles et les métadonnées du bloc.

1. **`content.text`**

Texte descriptif affiché au-dessus du formulaire de contact.
Transformé avec emojify et rendu avec `$page.RenderString`.

2. **`content.autolink`**

Transforme en liens l'adresse e-mail et le numéro de téléphone.

3. **`content.email`**

Adresse e-mail affichée dans la section des coordonnées.
Peut être automatiquement transformée en lien `mailto:` si `$autolink` est activé.

4. **`content.phone`**

Numéro de téléphone affiché dans la section des coordonnées.
Peut être automatiquement transformé en lien `tel:` si `$autolink` est activé.

5. **`content.address`**

Adresse physique, composée des sous-paramètres suivants :
- street : Rue.
- city : Ville.
- region : Région.
- postcode : Code postal.
- country : Pays.
Formatée via le partiel functions/get_address.

6. **`content.directions`**

Instructions ou directions supplémentaires, affichées sous forme de texte.

7. **`content.office_hours`**

Horaires d'ouverture.

Peut être une chaîne ou une liste (affichée avec des sauts de ligne).

8. **`content.appointment_url`**

URL pour prendre un rendez-vous.

Affichée sous forme de lien avec le texte par défaut "Book an appointment".

Il est possible de modifier et de traduire ce texte avec l'identifiant i18n `book_appointment`.

9. **`content.contact_links`**

Liste de liens supplémentaires avec des icônes. 

Chaque lien peut inclure :
- icon_pack : Pack d'icônes (ex. fas, fab).
- icon : Nom de l'icône (ex. envelope, phone).
- link : URL du lien.
- name : Texte du lien.


#### Formulaire (content.form)

Ces paramètres configurent le formulaire de contact.

1. **`content.form.provider`**

Fournisseur du formulaire. 

Valeurs possibles :
- netlify : Utilise Netlify Forms.
- formspree : Utilise Formspree.

2. **`content.form.netlify`**

Paramètres spécifiques à Netlify Forms :
- captcha : Active/désactive le reCAPTCHA (par défaut : true).
- success_url : URL de redirection après soumission réussie.

3. **`content.form.formspree`**

Paramètres spécifiques à Formspree :
- id : Identifiant du formulaire Formspree (obligatoire).
- captcha : Active/désactive le reCAPTCHA (par défaut : false).
- captcha_key : Clé API pour le reCAPTCHA (obligatoire si captcha est activé).

4. **`content.form.netlify.attachments`**

Active/désactive la possibilité de joindre des fichiers au formulaire.

#### Design (design)

Ces paramètres définissent l'apparence et la mise en page du bloc.

1. **`design.columns`**
   
Nombre de colonnes pour le formulaire. Valeurs possibles :
- 1 : Une seule colonne.
- 2 : Deux colonnes (par défaut).

#### Carte (features.map)

Ces paramètres permettent d'afficher une carte si activé dans la configuration globale.

1. **`features.map.provider`**

Fournisseur de la carte (ex. Google Maps).

2. **`features.map.api_key`**

Clé API pour le fournisseur de la carte.

3. **`features.map.zoom`**

Niveau de zoom de la carte (par défaut : 15).

4. **`content.coordinates`**

Coordonnées géographiques pour la carte :
- latitude : Latitude.
- longitude : Longitude.

#### Résumé des validations

Si formspree est utilisé comme fournisseur, les paramètres suivants sont obligatoires :
- `content.form.formspree.id` : Identifiant du formulaire.
- `content.form.formspree.captcha_key` : Clé API reCAPTCHA (si captcha est activé).
Si des fichiers sont joints au formulaire, Netlify doit être utilisé comme fournisseur.