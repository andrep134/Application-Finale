# Architecture de navigation Material 3

## Navigation principale (Bottom Bar Bordeaux)
1. **Accueil** : point d'entrée, dashboard et CTA principaux.
2. **À propos** : informations institutionnelles, vision, mission, équipe, carte.
3. **Calendrier** : agenda mensuel + listes/grilles d'événements.
4. **Médias** : sermons vidéo/audio, filtres par série, détails de lecture.
5. **Don & Contact** : formulaire de don, coordonnées et actions rapides.

La barre utilise un fond bordeaux (`#6F1B2A`) avec icônes outline blanches et étiquettes semi-transparentes (`#FFFFFF` 74%). L'indicateur actif est un pill beige/or (`#D5B27F`) de 48×28dp avec ripple blanc.

## Navigation secondaire
- **AppBar** translucide (bordeaux 92%) avec titre centré et actions (recherche, profil).
- **Drawer plein écran** réservé aux liens secondaires (podcasts, ressources, paramétrage).
- **Tabs** dans les sections Calendrier et Médias pour basculer respectivement entre *Mois / Liste* et *Toutes / Séries / Prédicateurs*.

## Transitions
- Navigation entre destinations principales : fondu + translation 16dp.
- Changement de tab : animation glissante (200 ms) avec soulignement vert.
- Ouverture de détails (événement, sermon) : scale + fade (250 ms) avec ombre niveau 2.

## Flux clé
### Accès au live
Accueil → bouton « Live » → feuille modale présentant la prochaine diffusion YouTube + CTA Regarder.

### Ajout d'événement au calendrier
Calendrier (carte) → bouton « Ajouter à mon agenda » → bottom sheet avec options (Google Calendar, Apple, ICS).

### Parcours de don
Don & Contact → bouton vert « Faire un don » → multi-étapes : montant, coordonnées, confirmation (progress tracker beige/or).

### Demande de prière
Accueil → bouton « Prière » → formulaire modal (nom, sujet, texte) → toast de confirmation.

### Contact rapide
Don & Contact → section « Nous contacter » → boutons icône (téléphone, email, WhatsApp) avec ripple vert.
