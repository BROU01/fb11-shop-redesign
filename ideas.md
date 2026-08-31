# FB11 SHOP — Direction artistique et architecture

## Trois pistes initiales

### 1. Atelier Terre

Une boutique éditoriale, tactile et chaleureuse qui met les matières au premier plan : ivoire, tabac, cuir brun et vert profond. L’expérience doit évoquer un showroom calme plutôt qu’un tableau de bord commercial.

**Probabilité : 0,07**

### 2. Ligne Nocturne

Une direction plus sombre et graphique, inspirée des vitrines de luxe contemporaines, avec de grands aplats noirs et des accents métalliques très mesurés. Elle doit rester sobre et éviter les effets lumineux artificiels.

**Probabilité : 0,03**

### 3. Marché Moderne

Une identité plus directe et locale, avec une composition lumineuse, des blocs d’information pratiques et une forte priorité donnée à la commande WhatsApp. L’accent est mis sur la clarté et la confiance avant le prestige.

**Probabilité : 0,09**

## Direction choisie : Atelier Terre

### Design Movement

**Quiet luxury éditorial** croisé avec l’esthétique des ateliers de maroquinerie : peu d’effets, beaucoup de matière, des compositions asymétriques et une hiérarchie typographique nette.

### Core Principles

1. Les produits et leurs textures passent avant les fonctionnalités.
2. Chaque élément d’interface doit avoir une fonction commerciale compréhensible.
3. Le parcours est court : découvrir, choisir, commander sur WhatsApp.
4. La sophistication vient de l’espace, de la typographie et de la photographie, pas de l’accumulation de badges.

### Color Philosophy

L’ivoire crée un espace respirant et honnête. Le brun tabac rappelle le cuir et donne de la chaleur. Le vert forêt devient la couleur propriétaire de la marque : il apporte confiance et ancrage sans tomber dans le vert « fintech ». Le laiton mat intervient seulement en détail pour signaler la qualité et les finitions.

Palette : ivoire `#F4F0E8`, papier `#FBFAF7`, encre `#17221D`, vert forêt `#17483B`, tabac `#8A5A3B`, laiton `#B8925A`, sable `#DDD1BF`.

### Layout Paradigm

Une structure éditoriale asymétrique : hero en deux colonnes avec image dominante à droite, sections qui alternent entre texte court et visuels, catalogue en grille éditoriale de trois colonnes, fiches produit en split screen, pages catégorie avec intro compacte et filtres réduits. La navigation ne contient que **Boutique**, **Journal de marque**, **Guide des tailles** et **Contact**, avec WhatsApp comme CTA persistant mais discret.

### Signature Elements

- Une ligne verticale fine vert forêt qui accompagne les titres de section.
- Des légendes en petites capitales avec numérotation discrète : `01 / Matière`, `02 / Sélection`.
- Des surfaces ivoire et papier avec de légères ombres froides, sans cartes uniformément arrondies.

### Interaction Philosophy

Les interactions doivent réduire l’incertitude : une fiche produit expose la matière, la taille et la livraison avant le CTA. Les filtres sont peu nombreux et lisibles. Le bouton WhatsApp construit un message contextualisé avec le produit et la taille choisie. Aucun bouton ne doit exister uniquement pour décorer.

### Animation

Entrées douces et rapides : fondu et translation de 16 px, 220 à 280 ms, uniquement à l’arrivée des sections. Survol produit : zoom photographique très léger et déplacement de 4 px. Boutons : réponse tactile immédiate. Aucun effet de défilement spectaculaire, aucune animation en boucle, aucun effet glow. Respect de `prefers-reduced-motion`.

### Typography System

Titres : **DM Serif Display**, avec une présence éditoriale et des contrastes élégants. Interface et paragraphes : **Manrope**, lisible et contemporaine. Les titres utilisent une casse phrase, jamais des blocs criards en capitales. Les labels fonctionnels restent courts en 11–12 px avec espacement de lettres modéré.

### Brand Essence

**FB11 SHOP est une boutique togolaise de chaussures et d’accessoires en cuir qui aide les actifs urbains à choisir une pièce bien faite et à la commander simplement sur WhatsApp.**

Personnalité : **sûre, tactile, attentive**.

### Brand Voice

Les titres sont précis et évocateurs. Les CTA sont directs, jamais agressifs. Les microcopies expliquent ce qui va se passer et évitent les superlatifs non prouvés.

Exemples : « Le cuir se remarque avant même qu’on le touche. » et « Choisir ma pointure — puis commander sur WhatsApp ».

### Wordmark & Logo

Le mot-symbole repose sur une typographie serif personnalisée, avec un espacement généreux et un monogramme `F`/`B` discret inspiré d’une couture de ceinture. Le symbole livré séparément est une boucle abstraite de cuir, utilisable comme favicon et repère de marque sans écrire le nom.

### Signature Brand Color

**Vert Atelier `#17483B`** : un vert forêt profond, calme et distinctif, qui relie le savoir-faire artisanal à la confiance nécessaire au commerce local.

## Architecture multi-page retenue

| Route | Rôle |
|---|---|
| `/` | Page d’accueil : positionnement, hero, sélection courte, preuve de service, CTA WhatsApp. |
| `/boutique` | Catalogue global avec recherche légère et filtres réellement utiles. |
| `/chaussures` | Page catégorie chaussures avec sélection dédiée. |
| `/ceintures` | Page catégorie ceintures et accessoires. |
| `/produit/:slug` | Fiche produit avec tailles, prix, matière et commande contextualisée. |
| `/guide-tailles` | Guide simple pour choisir sa pointure ou sa longueur de ceinture. |
| `/a-propos` | Histoire, sélection des matières et zone de livraison. |
| `/contact` | Contact, horaires, localisation générale et WhatsApp. |

Le suivi GPS, l’accès Direction public, le compte client et le panier complexe sont exclus de cette version. Le paiement et la commande restent volontairement simples et transparents via WhatsApp.
