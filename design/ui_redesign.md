# Directives complètes de redesign Material You

## 1. Identité visuelle
- **Palette** :
  - Bordeaux profond / rouge vin : `#6F1B2A` (primary) + gradient `#6F1B2A → #8A1F34` pour les fonds héro.
  - Blanc pur `#FFFFFF` pour les zones neutres.
  - Vert nature `#2E6B4E` pour les actions (Live, Don) et états validés.
  - Beige/Or `#D5B27F` pour les détails raffinés, séparateurs et badges.
- **Textures** : aplats lisses + motifs discrets (croix, feuilles) en filigrane beige à 8% d'opacité.
- **Logo** : centré dans la hero card avec halo beige.

## 2. Principes Material 3
- Cartes arrondies **20–24dp** avec ombre niveau 1.
- Espacement système : 8/16/24dp, marges horizontales 24dp, verticales 32dp.
- Typo : Poppins (titres spirituels), Inter (paragraphes), Roboto (labels UI).
- Effets ripple actifs sur chaque composant cliquable.
- App appliquer transitions d'opacité + translation 16dp.

## 3. Accueil (Dashboard premium)
### Hero
- Fond bordeaux gradient + logo EEBB + slogan « Dieu est fidèle ».
- Bouton « Regarder le live » (vert) + icône play, + bouton secondaire « Découvrir l'église » (outline beige).

### Boutons rapides (grille 2x2)
- Live, Calendrier, Don, Prière : cartes 20dp, icônes linettes blanches sur fond bordeaux, labels en Poppins 14sp.

### Carte « Prochain événement »
- Image plein écran arrondie 24dp, overlay noir 30%, titre + date + CTA « Ajouter au calendrier ».
- Badge beige « À venir ».

### Carte « Sermon de la semaine »
- Miniature YouTube, bouton flottant « Regarder » (bordeaux) + icône play blanche.
- Infos : titre, orateur, durée, lien vers playlist.

### Verset du jour
- Cadre beige avec texte centré, typographie Poppins Italic 18sp, citation alignée à droite.

### Moments forts
- Carrousel horizontal de cartes verticales (photo + titre + CTA « Voir plus »). Scroll snap.

## 4. À propos / Église
- Layout scroll vertical, sections sur fond blanc alternant avec panneaux beige.
- **Vision & Mission** : cartes 24dp, iconographie ligne verte.
- **Confession de foi** : timeline verticale bordeaux avec puces dorées.
- **Notre équipe** : grilles de portraits circulaires, carte avec nom, rôle, bouton contact.
- **Ministères** : chips bordeaux (fond) + texte blanc, descriptions sur cartes blanches.
- **Horaires du culte** : card verte + icône horloge.
- **Carte Google** : composant pleine largeur avec arrondi 24dp et bouton « Itinéraire » bordeaux.

## 5. Calendrier / Événements
- Vue mensuelle stylisée : header bordeaux, jours sur fond blanc, date actuelle entourée vert.
- Toggle tabs : **Mois** / **Liste** / **Grille**.
- Cartes événements : photo, date, lieu (icône map), bouton CTA « S'inscrire » (vert) + « Ajouter à mon agenda » (outline).
- Animation d'ouverture : carte se dilate en plein écran avec visuel et description détaillée.

## 6. Médias
- Grille 2 colonnes (cartes 20dp) reprenant les miniatures YouTube, badge série beige.
- Filtres chips alignés haut : Séries, Thèmes, Prédicateurs, Live.
- Page détail : lecteur vidéo intégré, titre, résumé, notes PDF, boutons Partager / Télécharger (outline bordeaux).

## 7. Don / Contact
- Header rassurant bordeaux + verset.
- Bouton principal vert « Faire un don » menant à flow multi-étapes.
- Formulaire : champs outline beige, labels en Poppins 14sp, validations en vert.
- Section contact : cartes action (Appeler, Email, WhatsApp) sur fond blanc, icônes bordeaux.

## 8. Accessibilité & États
- Skeletons, messages d'état, toasts, micro-interactions décrits dans `component_states.md`.
- Tous les boutons >56dp, textes contrastés, support TalkBack.

## 9. Design system
- Réutiliser les tokens `design_tokens.json`.
- Créer styles MaterialTheme (light/dark) à partir de ces valeurs.
- Components : ElevatedCard, FilledButton, TonalButton, Chips, Tabs, BottomNavigation.

## 10. Livraison
- Maquettes Figma recommandées avec auto-layout, contraintes Material 3.
- Dev Android : Compose ou XML (avec Material Components v1.11+).
- Documenter les interactions, couleurs et assets dans un guide d'intégration.
