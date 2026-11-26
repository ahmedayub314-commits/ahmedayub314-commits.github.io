# ahmedayub314-commits.github.io

Personal site for Ahmed Ayub — QA engineering and test automation.

`index.html` is generated, not hand-edited. The source of truth is
`job-search/master.json` + `job-search/site.json`, rendered by
`job-search/build_site.py`, which also renders every resume from the same
content so the site and the documents cannot disagree. A checker
(`job-search/verify.py`) refuses any figure that does not trace back to
`master.json`.

To update: edit `master.json` / `site.json`, run `python3 build_site.py`,
then copy `site/standalone.html` here as `index.html` and push.
