# Comité Oise de Badminton — site web

Site du Comité départemental de badminton de l'Oise (60), Ligue Hauts-de-France, FFBaD.

Direction artistique « LE TERRAIN » : tout le site est pensé comme un terrain de badminton vu du dessus.
Les lignes du terrain structurent la mise en page, les zones du terrain servent de boutons, les chiffres
s'affichent comme les cotes d'un plan ou le tableau d'affichage d'une salle.

## Pages

| Fichier | Contenu |
| --- | --- |
| `index.html` | Accueil : le terrain, le tableau des rencontres, les quatre couloirs, les 16 clubs |
| `comite/index.html` | Missions, palmarès, assemblées générales, contact |
| `clubs/index.html` | Carte, index A-Z et fiche de chaque club |
| `competitions/index.html` | Calendrier 2026-27, familles de compétitions, inscriptions |
| `competitions/interclubs.html` | Interclubs mixtes D1 à D5, interclubs hommes, interclubs jeunes, documents |
| `competitions/adultes.html` | Championnat de l'Oise sénior, circuits Oise, vétérans, rencontres loisir |
| `jeunes/index.html` | Championnat, circuits départementaux, interclubs jeunes, Minipous, équipe de l'Oise, niveau régional |
| `formations/index.html` | Entraîneurs, arbitres et juges-arbitres |
| `documents/index.html` | Calendriers, règlements, formulaires, classements, comptes rendus d'AG |

Chaque page intérieure s'ouvre sur un demi-terrain : fond de court à gauche, filet à droite, rubriques de la
page dans la zone avant. Sur mobile, le demi-terrain passe à la verticale.

## Fichiers communs

- `css/style.css` : toute la mise en forme, accueil et pages intérieures.
- `js/main.js` : ouverture et fermeture du menu mobile.

Aucune dépendance, aucun outil de build. Les polices « Big Shoulders Display » et « Barlow » sont chargées
depuis Google Fonts. Tous les liens internes sont relatifs : le site s'ouvre aussi bien en double-cliquant
sur `index.html` que depuis un serveur.

L'en-tête et le pied de page sont recopiés dans chaque fichier HTML. Une modification du menu, de l'adresse
ou des partenaires doit être reportée dans les neuf pages.

## Lancer en local

```
py -m http.server 8000
```

puis ouvrir <http://localhost:8000/>. Sous macOS ou Linux, remplacer `py` par `python3`.

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

## Origine des contenus

Les textes, dates, clubs et documents viennent de l'ancien site Wix du comité
(president60bad.wixsite.com/comite60-badminton). Les documents PDF, Word et Excel sont encore hébergés
par Wix : les liens pointent vers ces fichiers. Ils cesseront de fonctionner si le site Wix est supprimé.
Il faudra alors les copier dans un dossier `documents/fichiers/` et mettre les liens à jour.

## Contenus à compléter

Les informations manquantes sont laissées entre crochets dans les pages :

- les dates et lieux 2026-27 des compétitions jeunes, vétérans, rencontres loisir, stages et formations ;
- le lieu du COS 2 et du COD 3 ;
- la salle, le contact ou le site de plusieurs clubs ;
- les membres du bureau du comité et les palmarès depuis 2022-23 ;
- les emplacements `[Photo]` et `[Carte]`.
