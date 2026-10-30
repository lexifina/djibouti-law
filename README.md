# Djibouti: law history in git

The law of Djibouti as a git history: one file per provision, with the source credited as the author. `git blame` names the source of every paragraph. It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `dj/`.

**What is in it now**

| Folder | Act | Versions | History |
| --- | --- | ---: | --- |
| `constitution/` | The Constitution of the Republic of Djibouti: the Preamble, Titles I to XIII and Articles 1 to 97 | 1 | One version: the text the Presidency of the Republic's website showed on 29 October 2026 |
| `code-civil/` | Code civil (loi n° 003/AN/18/8ème L du 12 avril 2018) | 1 | Oldest version available: the Code as adopted, dated 12 April 2018, with no later amendments (2411 articles) |
| `code-de-commerce/` | Code de commerce (loi n° 134/AN/11/6ème L du 1er août 2012) | 1 | Oldest version available: the Code as adopted, dated 1 August 2012, with no later amendments (2152 articles) |
| `code-penal/` | Code pénal (loi n° 59/AN/94 du 5 janvier 1995), Livres I to IV | 1 | Oldest version available, dated 5 January 1995 by the law; the PDF gives no consolidation date (555 articles) |
| `code-du-travail/` | Code du travail (loi n° 133/AN/05/5ème L du 28 janvier 2006) | 1 | As enacted, dated 28 January 2006, from the Journal officiel; later amendments not applied (299 articles) |
| `code-de-la-famille/` | Code de la famille (loi n° 152/AN/02/4ème L du 31 janvier 2002) | 1 | As enacted, dated 31 January 2002, from the Journal officiel; the 2014 amendment is not applied (222 articles) |
| `code-protection-mineurs/` | Code de protection juridique des mineurs (loi n° 95/AN/15/7ème L du 18 mai 2015) | 1 | As enacted, dated 18 May 2015, from the Journal officiel (90 articles) |

Language: French, the text that prevails under article 93 of the Constitution. The Arabic text is not included.

**What it does not show**

- Only one version exists here. The Presidency's page gives the current consolidated text with no date and no list of the revisions it includes, so the repository is dated from the day the page was read (29 October 2026). It is the oldest version available, not the Constitution as adopted in 1992, and the revisions are not replayed.
- Statutes: only those listed above. Other statutes and decrees are not included yet: the Journal Officiel publishes acts as enacted, with no consolidated text.
- The page's table of contents and analytical index are left out.

- The Code civil is the text as adopted on 12 April 2018; the amending law of 30 April 2019 (n° 47/AN/19/8ème L) is not applied. Headings are left out and paragraph breaks are rebuilt from a PDF line layout.

- The Code de commerce is the text as adopted on 1 August 2012; the amending laws of 2018 (n° 001/AN/18/8ème L) and 2019 (n° 49/AN/19/8ème L) are not applied. Article numbers are kept as printed, including a few misprints in the PDF; headings are left out.

- The Code pénal is the FAOLEX copy of loi n° 59/AN/94, dated by the law (5 January 1995); the PDF states no consolidation date, so later amendments may be in it. Livre V (contraventions) is left out. Headings are left out.

- The Code du travail is the text as enacted by loi n° 133/AN/05/5ème L (Journal officiel n° 3 of 28 February 2006); the laws that amended it later (2010, 2017, 2019, 2020, 2025) are not applied. Headings are left out.

- The Code du travail is the text as enacted by loi n° 133/AN/05/5ème L (Journal officiel n° 3 of 28 February 2006); the laws that amended it later (2009 to 2025) are not applied. Headings are left out.

- The Code de la famille is the French text as enacted by loi n° 152/AN/02/4ème L (Journal officiel n° 1 of 31 January 2002); under its article 220 the Arabic text prevails, and it is not included. The 2014 amending law (n° 56/AN/14/7ème L, Titres 6 and 7) is not applied, because its published text is incomplete. Headings are left out.

- The Code de protection juridique des mineurs is the text as enacted by loi n° 95/AN/15/7ème L (Journal officiel n° 10 of 31 May 2015). Headings are left out.

**Source**

Presidency of the Republic of Djibouti, La Constitution: <https://www.presidence.dj/page/constitution>, read on 29 October 2026.

Code civil: WIPO Lex, DJ026, <https://wipolex-res.wipo.int/edocs/lexdocs/laws/fr/dj/dj026fr.pdf>, read on 30 October 2026.

Code de commerce: WIPO Lex, DJ023, <https://wipolex-res.wipo.int/edocs/lexdocs/laws/fr/dj/dj023fr.pdf>, read on 30 October 2026.

Code pénal: FAOLEX (FAO), <https://faolex.fao.org/docs/pdf/dji244285.pdf>, read on 30 October 2026.

Code du travail: Journal officiel de la République de Djibouti, <https://www.journalofficiel.dj/texte-juridique/loi-n133-an-05-5eme-l-portant-code-du-travail/>, read on 30 October 2026.

Code de la famille: Journal officiel de la République de Djibouti, <https://www.journalofficiel.dj/texte-juridique/loi-n152-an-02-4eme-l-portant-code-de-la-famille/>, read on 30 October 2026.

Code de protection juridique des mineurs: Journal officiel de la République de Djibouti, <https://www.journalofficiel.dj/texte-juridique/loi-n95-an-15-7eme-l-portant-code-de-protection-juridique-des-mineurs/>, read on 30 October 2026.

Nothing here is legal advice; for anything that matters, read the original. How the files were made is in [REPRODUCE.md](REPRODUCE.md).

## Licence

See [LICENSE](LICENSE).
