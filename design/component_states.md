# Micro-interactions et accessibilité

## États de chargement
- **Skeleton cards** : blocs arrondis 20dp, dégradé beige/or animé (1200 ms) pour toutes les cartes (événements, sermons, moments forts).
- **Boutons** : shimmer bordeaux semi-transparent + icône désactivée.
- **Listes vides** : illustration linéaire beige + message inspirant (par ex. « Restez connectés, de nouveaux contenus arrivent »).

## États d'erreur / vide
- Fond très clair `#FDF9F4`, pictogramme vert feuille et CTA « Réessayer » bordeaux.
- Messages en typographie Poppins Medium 16sp, alignés au centre.

## Accessibilité
- Contraste minimum 4.5:1 (bordeaux sur blanc, blanc sur bordeaux, vert sur beige).
- Touch targets ≥ 56×56dp, boutons principaux 72dp de large min.
- Support du mode sombre : inversion (background bordeaux profond, cartes anthracite, accents beige).
- Textes adaptatifs (Dynamic Type) et descriptions TalkBack pour icônes.

## Ripple et feedback
- Ripple blanc sur surfaces bordeaux, ripple bordeaux 24% sur surfaces blanches.
- Press states assombrissent la carte de 8% et augmentent l'élévation de 4dp.
- Switch/Checkbox utilisent vert nature comme couleur active, avec animation de ressort (180 ms).

## Animations
- Hero section : gradient animé (bordeaux → prune) de 6s en boucle subtile.
- Scroll : AppBar se condense avec animation de 120 ms et affiche l'ombre niveau 1.
- Navigation bottom bar : icône active se remplit avec un morphing 200 ms + label apparait.
