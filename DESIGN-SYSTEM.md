# Design System Super Docteurs

## Intention

Une identité médicale contemporaine, claire et énergique. Le bleu profond apporte la confiance et la profondeur, le vert pulse rend l'ensemble vivant, le bleu Méditech porte les actions et le mouvement.

## Couleurs

| Token | Valeur | Usage |
| --- | --- | --- |
| `--navy` | `#0A1C30` | Fond principal, textes foncés, footer |
| `--green` | `#00C796` | Accent humain, mise en avant, CTA secondaire |
| `--blue` | `#007AFF` | Liens, CTA principal, éléments interactifs |
| `--white` | `#F2F5F7` | Fond clair et texte sur fond foncé |
| `--muted` | `#587087` | Texte secondaire |
| `--line` | `#D8E1E8` | Bordures et séparateurs |

Utiliser le bleu profond comme couleur structurelle. Garder le vert pulse et le bleu Méditech pour les accents, les appels à l'action et les repères visuels. Les associations bleu et vert doivent rester ponctuelles pour préserver leur impact.

## Typographie

| Usage | Police | Graisses |
| --- | --- | --- |
| Interface, titres, paragraphes, boutons | Poppins | 400, 500, 600, 700 |
| Logotype uniquement | Alecrim Heavy | Fichier logo seulement |

Poppins est chargée depuis Google Fonts dans `src/styles/global.css`. Alecrim Heavy est réservée au logotype officiel et ne doit pas être utilisée pour les titres ou le texte courant.

## Échelle typographique

| Élément | Taille | Graisse |
| --- | --- | --- |
| H1 | `clamp(3rem, 6vw, 5.7rem)` | 700 |
| H2 | `clamp(2.1rem, 4vw, 3.75rem)` | 700 |
| H3 | `1.35rem` | 600 |
| Corps | `1rem` | 400 |
| Navigation et boutons | `0.82rem` | 600 |
| Eyebrow | `0.72rem`, capitales | 700 |

Les titres utilisent un interlettrage serré (`-0.045em`). Les labels et eyebrows utilisent un interlettrage étendu (`0.14em`).

## Espacements

La grille suit une unité de 4 px. Les espacements les plus courants sont 8, 12, 16, 20, 32, 48, 72 et 112 px.

| Contexte | Valeur |
| --- | --- |
| Padding bouton | 12 x 18 px environ |
| Gouttière desktop | 24 px |
| Gouttière mobile | 16 px |
| Espace entre sections | 112 px desktop, 72 px mobile |
| Rayon carte | 20 px |
| Rayon illustration hero | 40 px |

## Composants

| Composant | Rôle |
| --- | --- |
| `Header.astro` | Navigation principale et appel à l'action newsletter |
| `Footer.astro` | Signature de marque et liens de navigation |
| `SectionTitle.astro` | Eyebrow, titre et texte introductif cohérents |
| `EpisodeCard.astro` | Carte d'épisode réutilisable avec variante `green`, `blue` ou `dark` |

Créer les nouvelles sections à partir de `SectionTitle` et conserver la largeur maximum de contenu de 1216 px (`76rem`).

## Accessibilité

- Le bleu profond sur fond blanc est la combinaison par défaut pour les textes.
- Les liens et boutons conservent des intitulés explicites.
- Les champs de formulaire ont un label visible.
- Les couleurs ne portent jamais seules une information essentielle.
