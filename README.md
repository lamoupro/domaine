# Maquette — lieu de réception

Page de démonstration servant d'appui commercial. **Ce n'est pas le site d'un
établissement réel** : les textes, les tarifs, les disponibilités et les témoignages
sont des contenus d'illustration, et les photographies proviennent de Pexels.

## Personnalisation par l'adresse

Un seul fichier, aucune page par prospect. Les paramètres se passent dans l'URL :

| Paramètre | Rôle | Exemple |
|---|---|---|
| `n` | Nom de l'établissement | `?n=Château de Neyran` |
| `v` | Commune | `&v=Blanquefort` |
| `c` | Capacité d'accueil | `&c=180` |
| `t` | Téléphone | `&t=0665760670` |
| `l` | Adresse d'un logo | `&l=https://.../logo.png` |

Sans paramètre, la page affiche « Votre Domaine ».

## Notes techniques

- HTML statique, aucune dépendance, aucun script tiers.
- Police Jost auto-hébergée : passer par Google Fonts coûtait deux connexions
  supplémentaires avant le premier pixel.
- La vidéo d'ouverture n'est pas chargée sous 900 px de large : son décodage
  coûtait près de trois secondes de blocage processeur sur mobile.
- `noindex` dans l'en-tête et `robots.txt` interdisant l'indexation.
