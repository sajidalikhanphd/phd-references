# phd-references

> **CADQE PhD — Master Reference Library**

Master BibTeX library (`library.bib`), RIS export, PDF archive of all 97 PRISMA-reviewed papers + key reference papers, per-paper metadata stubs, and Zotero/Mendeley sync exports.

---

## Contents

| Path | Description |
|---|---|
| `library.bib` | Master BibTeX library (seed: 10 entries; target: 97+ PRISMA papers) |
| `library.ris` | RIS export for Zotero/Mendeley import |
| `pdfs/YYYY/` | PDF archive organised by year |
| `metadata/[citekey].md` | Per-paper metadata stubs (title, abstract, key finding, CADQE relevance) |
| `exports/ris/` | RIS exports (Zotero/Mendeley compatible) |
| `exports/csv/` | CSV exports for reference analysis |
| `prisma/cadqe-prisma-97-papers.csv` | All 97 PRISMA-included papers with novelty assessment |

## PDF Naming Convention

```
[NN]_[FirstAuthor]_[ShortKeyword].pdf
# Examples:
# 001_Biamonte_QML_Nature_2017.pdf
# 006_Han_EnQode_2025.pdf
# 009_Tudisco_EncodingDominance_2025.pdf
```

## Adding a New Reference

1. Find/download the PDF → `pdfs/YYYY/[NN]_[Author]_[Keyword].pdf`
2. Add BibTeX entry to `library.bib` (follow existing format)
3. Create metadata stub: `metadata/[citekey].md` (use template from `phd-literature-review/summaries/2026/template-paper-summary.md`)
4. Add RIS entry to `exports/ris/library.ris`
5. Commit:
   ```bash
   git add pdfs/ library.bib metadata/ exports/
   git commit -m "chore(references): add [Author] et al. ([Year]) — [ShortTitle]"
   git push origin main
   ```

## Zotero/Mendeley Sync

Import `library.bib` or `exports/ris/library.ris` directly into your reference manager. Re-export and overwrite these files when the reference manager library is updated.

## Cross-References

- Paper summaries → [`phd-literature-review`](https://github.com/[CANDIDATE]/phd-literature-review): `summaries/YYYY/[citekey].md`
- Citations in chapters → [`phd-drafts-and-versions`](https://github.com/[CANDIDATE]/phd-drafts-and-versions): `full-thesis/bibliography/references.bib` (symlink or copy of `library.bib`)

## Git Commit Convention

```bash
chore(references): <description>
# Examples:
# chore(references): add Tudisco et al. (2025) — encoding dominance finding
# chore(references): convert references.txt seed to BibTeX format
```

---

*Target Repo: phd-references*
