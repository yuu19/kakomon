# kakomon

Collection of graduate entrance examination materials gathered from Japanese university admissions sites. Each directory mirrors the structure of the source page so new files can be refreshed easily.

## Collected Archives

- `tohoku/ecei/` — Tohoku University Electrical and Information Engineering graduate entrance exams (基礎・専門・基礎専門総合) covering 2014–2025. Source: https://www.ecei.tohoku.ac.jp/ecei_web/admission/
- `kyodai/info/` — Kyoto University Graduate School of Informatics summer master exams for each course (IST, SI, AMS, AMP, SYS, CCE) 2020–2024. Source: https://www.i.kyoto-u.ac.jp/admission/examarchive/
- `kyodai/math/` — Kyoto University mathematics master general-admission exams from 1989–2026 (English files unavailable for 2024 onward on the source page). Source: https://www.math.kyoto-u.ac.jp/ja/past-exams
- `titech/math/` — Tokyo Tech mathematics graduate entrance exams (Heisei 10 / 1998 through 2025). Source: https://www.math.titech.ac.jp/top/~jimu/Graduate/old-exam/innsi.html
- `titech/info/` — Institute of Science Tokyo (Tokyo Tech) Information Science summer exams grouped by course: `is/` (数理・計算科学系) and `cs/` (情報工学系) for 2019–2024. Source: https://admissions.isct.ac.jp/ja/013/graduate/examination-questions

## Practice Exercises (`practice/`)

The `practice/` directory stores Markdown-based exercise sets that reference the archived PDFs. Each file includes metadata (title, source URL, tags, `last_reviewed`) and is rendered as an HTML page on GitHub Pages. Use `practice/templates/problem-set.md` as a starter when adding a new set, and keep university/subject/year folders aligned with the PDF archive.

## GitHub Pages

- The root of the repository is a Jekyll site that uses the `pages-themes/cayman` theme. `_config.yml` configures the `practice` collection and enables sitemap/SEO plugins.
- Deployment is automated via `.github/workflows/pages.yml`. Pushing to `main` (or running the workflow manually) builds the site and publishes it to GitHub Pages.
- To preview locally: `bundle install` followed by `bundle exec jekyll serve`. Remember to ignore `_site/` and `.jekyll-cache/` when making commits.

## Usage Notes

- Files are provided for personal study; respect each university’s copyright notices before redistribution.
- Some years are intentionally missing where the source site omits a PDF (e.g., 2020 written exams for certain programs, or English sections after 2024).
- When updating, re-run the download scripts or manual retrieval steps against the source URLs above and replace the PDFs in place.
