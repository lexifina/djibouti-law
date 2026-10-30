# How this repository was made (Djibouti)

This file is written by the build on 2026-10-30, the day the source data was retrieved.

## Sources

| Source | Address | Retrieved | Licence |
| --- | --- | --- | --- |
| Presidency of the Republic of Djibouti: La Constitution | <https://www.presidence.dj/page/constitution> | 2026-10-29 | Official publication of the Presidency of the Republic of Djibouti |
| FAOLEX (FAO): Code pénal de Djibouti (loi n° 59/AN/94 du 5 janvier 1995) | <https://faolex.fao.org/docs/pdf/dji244285.pdf> | 2026-10-30 | text of law republished by FAOLEX; no licence stated on the PDF |
| WIPO Lex: Code civil (adopté par la loi n° 003/AN/18/8ème L du 12 avril 2018) (DJ026) | <https://wipolex-res.wipo.int/edocs/lexdocs/laws/fr/dj/dj026fr.pdf> | 2026-10-30 | official text of law republished by WIPO Lex; no licence stated on the PDF |
| WIPO Lex: Code de commerce de la République de Djibouti (loi n° 134/AN/11/6ème L du 1er août 2012) (DJ023) | <https://wipolex-res.wipo.int/edocs/lexdocs/laws/fr/dj/dj023fr.pdf> | 2026-10-30 | official text of law republished by WIPO Lex; no licence stated on the PDF |
| Journal officiel de la République de Djibouti: Loi n° 133/AN/05/5ème L portant Code du Travail | <https://www.journalofficiel.dj/texte-juridique/loi-n133-an-05-5eme-l-portant-code-du-travail/> | 2026-10-30 | official text of law published by the Secrétariat général du Gouvernement in the Journal officiel; no licence stated |
| Journal officiel de la République de Djibouti: Loi n° 152/AN/02/4ème L portant Code de la Famille | <https://www.journalofficiel.dj/texte-juridique/loi-n152-an-02-4eme-l-portant-code-de-la-famille/> | 2026-10-30 | official text of law published by the Secrétariat général du Gouvernement in the Journal officiel; no licence stated |
| Journal officiel de la République de Djibouti: Loi n° 95/AN/15/7ème L portant Code de protection juridique des mineurs | <https://www.journalofficiel.dj/texte-juridique/loi-n95-an-15-7eme-l-portant-code-de-protection-juridique-des-mineurs/> | 2026-10-30 | official text of law published by the Secrétariat général du Gouvernement in the Journal officiel; no licence stated |

Every word of law in this repository comes from these sources. Lexifina reads them and records each act's dated versions, and the laws that made each change, in one corpus file. This repository is built from that file.

## What is in it

| Act | Title | Versions | Span |
| --- | --- | ---: | --- |
| `constitution` | Constitution de la République de Djibouti | 1 | 2026-10-29 to 2026-10-29 |
| `code-penal` | Code pénal (loi n° 59/AN/94 du 5 janvier 1995 portant Code pénal) | 1 | 1995-01-05 to 1995-01-05 |
| `code-civil` | Code civil de la République de Djibouti (adopté par la loi n° 003/AN/18/8ème L du 12 avril 2018) | 1 | 2018-04-12 to 2018-04-12 |
| `code-de-commerce` | Code de commerce de la République de Djibouti (loi n° 134/AN/11/6ème L du 1er août 2012) | 1 | 2012-08-01 to 2012-08-01 |
| `code-du-travail` | Code du travail (loi n° 133/AN/05/5ème L du 28 janvier 2006 portant Code du travail) | 1 | 2006-01-28 to 2006-01-28 |
| `code-de-la-famille` | Code de la famille (loi n° 152/AN/02/4ème L du 31 janvier 2002 portant Code de la famille) | 1 | 2002-01-31 to 2002-01-31 |
| `code-protection-mineurs` | Code de protection juridique des mineurs (loi n° 95/AN/15/7ème L du 18 mai 2015) | 1 | 2015-05-18 to 2015-05-18 |

The build made 7 commits:

| Commits | Kind |
| ---: | --- |
| 7 | first version of an act |
| 0 | one law on its in-force day |
| 0 | changes no amendment note explains, credited to the publisher |

Other counts:
- 0 commits on the branch `future`: laws not yet in force on 2026-10-30.
- 0 commits dated 1 January 1970: in force before 1970, with the real day in their `In-force` trailer.
- 3 laws in the record.
- 10 tags.

## Dates

Each commit is dated at noon (Africa/Djibouti) on the day the change took effect. The other dates, enacted and published, are trailers.

When a law gives no date of its own, the default rule applies: The Presidency's page states no date for its text. The record holds one version, the text the page showed on the day it was read (29 October 2026), taken as the Constitution in force that day. https://www.presidence.dj/page/constitution

## How the history is built

`tools/build.py` turns the corpus into this history in one pass: one commit per law, on the day it took effect. The same corpus always gives the same commit hashes. `tools/check_repo.py` reads every version back from git and compares it with the corpus. `tools/on.py` shows the law as it stood on any date. The corpus format is described in `tools/SCHEMA.md`.

- Corpus: sha256 `b920a544fda41d383476612adc449938af9c03bab9d97c5fd4f020b4d0f13a93` (3452494 bytes).
- Builder blob hashes (`git hash-object`): `build.py` `a4faa25af85facb64b956b372f6b528aafdd7ec1`, `check.py` `3d00541d258745461ab52b1b0cb4e1716a27a95d`, `on.py` `644a6c0857fbcc72562032b58d57aa113fee0641`.
- Python 3.12.10; git version 2.46.0.windows.1.

## Checks

7 versions of 7 acts read back from git on the day each took effect and on the day before: 0 mismatches. Trailers: 0 commits whose trailers git cannot parse. Health: 0 merge commits on main, 0 commit dates that go backwards, 0 commits dated after the build.

A second build from the same corpus into an empty folder gave identical hashes for all 7 history commits and 10 tags (history tip `8723b8e3d292ab3cab18ca7f30f40aeab19293aa`).

## Decisions made by hand

- One version only. The Presidency's page gives the current consolidated text with no date and no amendment history, so this is the oldest version available (first_law null), dated from the day the page was read.
- The text is the French text; article 93 provides that the French text prevails over the Arabic. The Arabic text is not included.
- Text is the Preamble, the Titles and Articles 1 to 97 as the page prints them; the page's table of contents and analytical index are left out.
- Titre headings are kept as their own files (titre-01 and so on).
- Code pénal: one version, dated 1995-01-05 (the date of loi n° 59/AN/94, which the Code is cited by); first_law null, oldest version available. The FAOLEX PDF gives no consolidation date or amendment list, so later amendments may or may not be in the text.
- Code pénal units: one per article (art-001 to art-555, Livres I to IV); Livre V (contraventions, Art. R.1 onward, with the regulatory articles) is not built; Livre, Titre, Chapitre and Section headings are left out; paragraph breaks are rebuilt from the PDF line layout. Two headings in the PDF read "Articles 5" and "Articles 478" for "Article 5" and "Article 478"; they are read as such.
- Code civil: one version, the Code as adopted (first_law null, oldest version available), dated 2018-04-12, the day of promulgation; article 2 of the adopting law makes it in force on promulgation. Loi n° 47/AN/19/8ème L of 30 April 2019, which amends it, is not applied.
- Code civil units: one per article (art-001 to art-2411); Livre, Titre, Chapitre and Section headings and the table of contents are left out; paragraph breaks are rebuilt from the PDF line layout.
- Code de commerce: one version, the Code as adopted, dated 2012-08-01 (promulgation and entry into force per WIPO Lex); first_law null, oldest version available. The 2018 and 2019 amending laws are not applied.
- Code de commerce units: one per article marker "Art. L.NNNN-N" as printed (key art-l-NNNN-NNN); headings and the table of contents are left out. A few markers in the PDF are misprinted (for example a three-digit number or a repeated number); they are kept as printed and any repeat gets a -dupN key. Where a marker is too garbled to read (for example "Art.2 L.2213-203"), its text stays inside the preceding article.
- Code du travail: one version, the Code as enacted (first_law loi n° 133/AN/05/5ème L), dated 2006-01-28, the date of the law (its promulgation), which the Journal officiel gives as the date of the text and later amending laws cite ("loi n° 133/AN/05/5ème L du 28 janvier 2006"). Under the Code civil article 1 then in force, a law was executory by virtue of its promulgation; the Journal officiel edition carrying it is n° 3 of 28 February 2006.
- Code du travail: later amending laws (among them n° 61/AN/09/6ème L, n° 109/AN/10/6ème L, n° 221/AN/17/8ème L, n° 51/AN/19/8ème L, n° 98/AN/20/8ème L and n° 168/AN/25/9ème L) are not applied.
- Code du travail units: one per article (art-001 to art-299, with -bis suffixes as printed), each paragraph or line break of the Journal officiel text on its own line; the centred Titre, Chapitre, Section and Paragraphe headings, the visas and the signature are left out.
- Code de la famille: one version, the Code as enacted (first_law loi n° 152/AN/02/4ème L), dated 2002-01-31: article 222 orders its publication in the Journal officiel on promulgation, and the Journal officiel gives both the text and its edition (n° 1) that date.
- Code de la famille: the French text is built; article 220 provides that the law is published in Arabic and French and that the Arabic version prevails in case of conflict. The Arabic text is not included.
- Code de la famille: loi n° 56/AN/14/7ème L (Journal officiel n° 18 of 30 September 2014), which amends Titres 6 and 7, is not applied: its Journal officiel page gives new articles 77 to 83 and 87 to 92 but not its operative article or articles 84 to 86, so the resulting text cannot be established.
- Code de la famille units: one per article (art-001 to art-222), each paragraph or line break of the Journal officiel text on its own line; the centred headings, the visas and the signature are left out.
- Code de protection juridique des mineurs: one version, the law as enacted (first_law loi n° 95/AN/15/7ème L), dated 2015-05-18, the date the Journal officiel gives the law. Its article 90 orders publication in the Journal officiel on promulgation; under the Code civil article 1 then in force a law was executory by virtue of its promulgation. The Journal officiel edition carrying it is n° 10 of 31 May 2015.
- Code de protection juridique des mineurs units: one per article (art-001 to art-090), each paragraph or line break of the Journal officiel text on its own line; the centred headings, the visas and the signature are left out.

## What AI did and did not do

The scripts that read the sources and build this repository were written by Claude Code running Claude Opus 5.5 (`claude-opus-5-5`) under Lexifina's direction.

No model wrote, translated or corrected legal text. No model runs at build time. Every word of law in this repository comes from the official sources above.

The commit messages are written by `build.py` from the source data.

Model use at data-build time:
- Claude Code (Claude Sonnet 5.5) wrote the parser. No model wrote, edited or summarised legal text.
- Claude Code wrote the code and chose the source; it did not write or alter any legal text. The code is deterministic and runs no model.
- Claude Code wrote the code and chose the source; it did not write or alter any legal text. The code is deterministic and runs no model.
- Claude Code wrote the code and chose the source; it did not write or alter any legal text. The code is deterministic and runs no model.
- Claude Code wrote the code and chose the source; it did not write or alter any legal text. The code is deterministic and runs no model.
- Claude Code wrote the code and chose the source; it did not write or alter any legal text. The code is deterministic and runs no model.
- Claude Code wrote the code and chose the source; it did not write or alter any legal text. The code is deterministic and runs no model.
