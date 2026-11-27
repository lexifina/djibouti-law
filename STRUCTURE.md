# Structure

| Dossier | Contenu |
| --- | --- |
| `constitution/` | La Constitution de la République de Djibouti |
| `codes/<code>/` | Les codes : `codes/code-penal/`, `codes/code-civil/`, `codes/code-de-commerce/`, `codes/code-du-travail/`, `codes/code-de-la-famille/`, `codes/code-protection-mineurs/`, `codes/code-de-procedure-penale/` |
| `constitutions-anterieures/1992/` | La Constitution du 15 septembre 1992 telle que promulguée, avant ses révisions (copie secondaire) |
| `lois/<année>/<n°>-an-<aa>-<objet>/` | Lois, lois organiques et lois de finances, par l'année de leur numéro (`/AN/aa/`), p. ex. `lois/2006/144-an-06-approbation-des-comptes-financiers-delectricite/` |
| `ordonnances/<année>/<n°>-<objet>/` | Ordonnances |
| `decrets/<année>/<n°>-<objet>/` | Décrets réglementaires |
| `arretes/<année>/<n°>-<objet>/` | Arrêtés réglementaires |
| `decisions/<année>/`, `deliberations/<année>/` | Décisions et délibérations réglementaires |
| `accords/<année>/` | Accords, conventions et protocoles publiés au Journal officiel |
| `rectificatifs/<année>/` | Rectificatifs, errata et additifs |

Le Code civil et le Code de commerce, trop longs pour un seul dossier, sont rangés par livre et par titre :
`codes/code-civil/livre-1/` (art. 1 à 649), `livre-2/` (art. 650 à 813) et `livre-3/titre-01/` à `titre-21/`
(art. 814 à 2411), selon les intitulés de livre et de titre du code ; `codes/code-de-commerce/livre-<A>/titre-<B>/`
selon le numéro de l'article, qui porte le livre et le titre (L.2214-1 : livre 2, titre 2 ; les numéros à trois
chiffres, comme L.301-1, sont dans `livre-<A>/`).

La Constitution (`constitution/`) est le texte publié par la Présidence, qui intègre la révision faite par la loi
constitutionnelle n° 192/AN/25/9ème L du 6 novembre 2025 (Journal officiel n° 05 du 6 novembre 2025) : en vigueur le
7 novembre 2025, lendemain de cette publication. Son premier commit portait le jour où la page a été lue
(29 octobre 2026) ; un commit `Kind: correction` donne la vraie date.

Une année qui compte plus de 1 000 textes est divisée par mois (`arretes/<année>/<mm>/`). Aucun dossier ne compte plus
de 1 000 entrées. Chaque texte a un fichier par article (`art-001.md`, `art-012-bis.md`, `art-unique.md`), un
`preambule.md` pour ce qui précède le premier article, ou un seul `texte.md` s'il n'a pas d'articles, et un `README.md`
(titre, numéro du Journal officiel, visas, signature).

Les mesures individuelles (nominations, carrières, congés, décorations, attributions nominatives) et les circulaires
ne sont pas reprises : ce ne sont pas des règles de droit. Les décisions et délibérations ne sont reprises que si
leur intitulé montre une règle (fixant, réglementant, portant création ou organisation, tarifs, budgets, modifiant…) ;
les décisions du Conseil constitutionnel sont dans un dépôt distinct de jurisprudence.

## Dates

Chaque version est un commit daté de 12 h 00 (heure de Djibouti) le jour de son entrée en vigueur, que répète le
trailer `In-force:`. `In-force-basis:` dit d'où vient ce jour :

- `fixed-in-text` : le jour que le texte fixe lui-même (« entre en vigueur le … », « prend effet à compter du … ») ;
- `signature` : la date du texte, quand il entre en vigueur dès sa signature ou sa promulgation ;
- `publication` : la date du numéro du Journal officiel qui le publie (le texte dit « dès sa publication », ou ne dit
  rien et a été publié avant le Code civil de 2018) ;
- `day-after-publication` : le lendemain de cette date, pour les textes publiés depuis le Code civil de 2018 qui ne
  fixent pas d'autre jour (Code civil, article 1er) ;
- `promulgation` : le jour de la promulgation (la Constitution de 1992) ;
- `enactment-of-code` : la date de la loi portant le code, quand la copie ne donne pas de date de consolidation (le
  Code de procédure pénale, comme le Code pénal).

Les textes qui ne viennent pas d'une source officielle portent le trailer `Source-status: secondary copy (...)` ;
`Text-source: publisher OCR` signale une couche texte issue d'un OCR fait par l'éditeur du PDF (jamais par nous).

Aucune date de ce dépôt n'est le jour où nous avons lu une page (le premier commit de `constitution/` l'était ; il est
corrigé, voir ci-dessus). Un texte sans numéro du Journal officiel ni date
propre est retenu (non publié). Avant 1970, que git ne sait pas dater, le commit porte le 1er janvier 1970 et le vrai
jour figure dans le titre et le trailer `In-force:`.

# Structure (English)

`constitution/`, `codes/<code>/` (Code civil and Code de commerce by `livre-N/` and `titre-NN/`, from the code's own
headings and article numbers), `lois/<year>/<no>-an-<yy>-<subject>/`, `ordonnances/<year>/`, `decrets/<year>/`,
`arretes/<year>/`, `decisions/<year>/`, `deliberations/<year>/`, `accords/<year>/`, `rectificatifs/<year>/`; one file
per article. Dates: noon Africa/Djibouti on the in-force day; `In-force-basis` is `fixed-in-text`, `signature`,
`publication` or `day-after-publication` (Code civil art. 1, for texts published after the 2018 Code civil).
Individual measures (appointments, careers, decorations) and circulars are left out.
