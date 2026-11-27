# Structure

| Dossier | Contenu |
| --- | --- |
| `constitution/` | La Constitution de la RÃ©publique de Djibouti |
| `codes/<code>/` | Les codes : `codes/code-penal/`, `codes/code-civil/`, `codes/code-de-commerce/`, `codes/code-du-travail/`, `codes/code-de-la-famille/`, `codes/code-protection-mineurs/` |
| `lois/<annÃ©e>/<nÂ°>-an-<aa>-<objet>/` | Lois, lois organiques et lois de finances, par l'annÃ©e de leur numÃ©ro (`/AN/aa/`), p. ex. `lois/2006/144-an-06-approbation-des-comptes-financiers-delectricite/` |
| `ordonnances/<annÃ©e>/<nÂ°>-<objet>/` | Ordonnances |
| `decrets/<annÃ©e>/<nÂ°>-<objet>/` | DÃ©crets rÃ©glementaires |
| `arretes/<annÃ©e>/<nÂ°>-<objet>/` | ArrÃªtÃ©s rÃ©glementaires |
| `decisions/<annÃ©e>/`, `deliberations/<annÃ©e>/` | DÃ©cisions et dÃ©libÃ©rations rÃ©glementaires |
| `accords/<annÃ©e>/` | Accords, conventions et protocoles publiÃ©s au Journal officiel |
| `rectificatifs/<annÃ©e>/` | Rectificatifs, errata et additifs |

Une annÃ©e qui compte plus de 1 000 textes est divisÃ©e par mois (`arretes/<annÃ©e>/<mm>/`). Aucun dossier ne compte plus
de 1 000 entrÃ©es. Chaque texte a un fichier par article (`art-001.md`, `art-012-bis.md`, `art-unique.md`), un
`preambule.md` pour ce qui prÃ©cÃ¨de le premier article, ou un seul `texte.md` s'il n'a pas d'articles, et un `README.md`
(titre, numÃ©ro du Journal officiel, visas, signature).

Les mesures individuelles (nominations, carriÃ¨res, congÃ©s, dÃ©corations, attributions nominatives) et les circulaires
ne sont pas reprises : ce ne sont pas des rÃ¨gles de droit.

## Dates

Chaque version est un commit datÃ© de 12 h 00 (heure de Djibouti) le jour de son entrÃ©e en vigueur, que rÃ©pÃ¨te le
trailer `In-force:`. `In-force-basis:` dit d'oÃ¹ vient ce jour :

- `fixed-in-text` : le jour que le texte fixe lui-mÃªme (Â« entre en vigueur le â€¦ Â», Â« prend effet Ã  compter du â€¦ Â») ;
- `signature` : la date du texte, quand il entre en vigueur dÃ¨s sa signature ou sa promulgation ;
- `publication` : la date du numÃ©ro du Journal officiel qui le publie (le texte dit Â« dÃ¨s sa publication Â», ou ne dit
  rien et a Ã©tÃ© publiÃ© avant le Code civil de 2018) ;
- `day-after-publication` : le lendemain de cette date, pour les textes publiÃ©s depuis le Code civil de 2018 qui ne
  fixent pas d'autre jour (Code civil, article 1er).

Aucune date de ce dÃ©pÃ´t n'est le jour oÃ¹ nous avons lu une page, sauf le premier commit de `constitution/`, datÃ© du jour
oÃ¹ le texte de la PrÃ©sidence a Ã©tÃ© lu (la page ne donne pas de date). Un texte sans numÃ©ro du Journal officiel ni date
propre est retenu (non publiÃ©). Avant 1970, que git ne sait pas dater, le commit porte le 1er janvier 1970 et le vrai
jour figure dans le titre et le trailer `In-force:`.

# Structure (English)

`constitution/`, `codes/<code>/`, `lois/<year>/<no>-an-<yy>-<subject>/`, `ordonnances/<year>/`, `decrets/<year>/`,
`arretes/<year>/`, `decisions/<year>/`, `deliberations/<year>/`, `accords/<year>/`, `rectificatifs/<year>/`; one file
per article. Dates: noon Africa/Djibouti on the in-force day; `In-force-basis` is `fixed-in-text`, `signature`,
`publication` or `day-after-publication` (Code civil art. 1, for texts published after the 2018 Code civil).
Individual measures (appointments, careers, decorations) and circulars are left out.
