# Comité Oise de Badminton — site web

Page d'accueil du Comité départemental de badminton de l'Oise (60), Ligue Hauts-de-France, FFBaD.

Direction artistique « LE TERRAIN » : tout le site est pensé comme un terrain de badminton vu du dessus.
Les lignes du terrain structurent la mise en page, les zones du terrain servent de boutons, les chiffres
s'affichent comme les cotes d'un plan ou le tableau d'affichage d'une salle.

## Fichiers

- `index.html` : page d'accueil (HTML sémantique, un seul `h1`).
- `css/style.css` : feuille de style, terrain dessiné en CSS aux proportions réglementaires (13,40 × 6,10 m).

Aucune dépendance, aucun outil de build. Les polices « Big Shoulders Display » et « Barlow » sont chargées
depuis Google Fonts.

## Lancer en local

Ouvrir `index.html` dans un navigateur, ou servir le dossier :

```
python3 -m http.server 8000
```

puis ouvrir <http://localhost:8000/>.

## Charte

| Usage | Couleur |
| --- | --- |
| Fond, vert gymnase | `#0E4D36` |
| Surface du terrain | `#125A40` |
| Zones sombres | `#0A3A29`, `#062A1D` |
| Lignes et texte, blanc cassé | `#F4F1E8` |
| Accent unique, jaune-vert volant | `#D7F25C` (texte `#0A3A29` dessus) |

Titres en Big Shoulders Display 800–900, capitales, interlignage 0,88. Texte en Barlow 400–700.
Angles droits partout : les seuls ronds sont les poteaux du filet.

## Contenus à compléter

Les informations manquantes sont laissées entre crochets dans `index.html` : la date et le lieu de la
première étape du circuit départemental jeunes, la ville de deux clubs, et l'emplacement `[Photo]`
de la section clubs. Les liens du menu et des couloirs pointent vers les futures pages du site
(`/comite/`, `/clubs/`, `/competitions/`, `/jeunes/`, `/formations/`, `/documents/`).
