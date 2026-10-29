# Yang Ye — academic homepage

The redesigned, buildless website is in `docs/`. The root-level Jekyll files are retained as the previous site. No deployment setting has been changed for this redesign.

## Local preview

From the repository root:

```sh
/Users/yeyang/miniforge3/envs/py311/bin/python -m http.server 8000 --bind 127.0.0.1 --directory docs
```

Open http://127.0.0.1:8000/. No package installation or build is needed.

## Editing

- Biography, affiliation, interests and contact: `docs/index.html`.
- Papers, authors, status, presentations and abstracts: `docs/research.html`. Copy an existing `<article class="paper">` for a new entry. Only link to resources that exist.
- Typography, color and responsive layout: `docs/assets/css/style.css`.
- Portrait: `docs/assets/images/profile.jpg`; preserve its aspect ratio and update the HTML dimensions if it changes.
- CV: replace `docs/assets/documents/cv.pdf` and its legacy copy `docs/Documents/CV_YEYANG.pdf` together.
- Navigation/footer appear in both main HTML pages; update both together.

Research entries and both downloadable CV copies were updated from `CV_261029` on October 29, 2026. The CV confirms the Management Science R&R status and the labor paper title “Imperfect Labor Substitution: Implications for Asset Pricing.” The working-paper list follows that CV; abstracts already present are retained. No manuscript links or abstracts were supplied for the two newly listed working papers.

## Compatibility

`home.html` and `cv.html` forward to the new home/CV. The old `/Documents/CV_YEYANG.pdf` and commodity-paper PDF paths and both Google verification files are retained. Other old Jekyll pages remain in the repository root; decide which still warrant migration before switching the publishing source. An HTML 404 page provides navigation back to the main content.

## Review and publish

Work is on `redesign/classic-academic`; tag `before-classic-redesign` records the original version. Review the local website first. **Do not push, merge to the publishing branch, or change Pages settings without the owner's publication approval.**

After approval, confirm the current Pages source, merge/push the reviewed changes, and select the intended branch with `/docs` as the Pages publishing folder. `docs/.nojekyll` disables Jekyll processing for the new static site. Check Home, Research, expandable abstracts, CV, legacy document links and mobile layout after deployment. The root Jekyll site can be restored by reverting the publishing source to its previous branch/folder.

The former template's license remains in `LICENSE`.
