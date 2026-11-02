RF & EMF LAB — QUARTO / GITHUB PAGES STARTER
Prepared for fribas001 on 1 November 2026.

WHAT IS INCLUDED
11 Quarto pages, original dark/teal styling inspired by MolecularNodes,
real project images, two timestamped YouTube embeds, a local comparison MP4,
search/navigation, and a GitHub Actions deployment workflow.

Repository: https://github.com/fribas001/fribas001.github.io
Publication status is shown by the repository Actions and Pages settings.

RECOMMENDED ADDRESS
Repository: fribas001.github.io
Website after deployment: https://fribas001.github.io/
Keep the software in its existing repositories and use this repository
as the main research/documentation site.

LOCAL PREVIEW
Install Quarto from https://quarto.org/docs/get-started/.
Open a terminal in this folder and run:
    quarto preview
For a complete build:
    quarto render
The generated site is written to _site/. Do not commit that directory.
The accompanying _site/index.html is a rendered local preview; search and
video behavior are best checked over HTTP using quarto preview.

PUBLISH TO GITHUB PAGES
1. Create a PUBLIC repository named exactly fribas001.github.io under
   fribas001. Start with an empty repository (no generated README/license).
   If this repository already exists, review and merge with its contents;
   do not replace the existing site blindly.
2. In that repository, open Settings > Pages > Build and deployment.
   Select Source: GitHub Actions.
3. From this website folder, run the following commands ONLY for the new
   empty repository. Authenticate to GitHub using your normal Git client:

    git init -b main
    git add .
    git commit -m "Add RF and EMF research website"
    git remote add origin https://github.com/fribas001/fribas001.github.io.git
    git push -u origin main

4. Open Actions and inspect "Build and deploy website". A push to main
   renders the pages and deploys _site using GitHub's Pages artifact flow.
   No personal access token needs to be added to the workflow.
5. When the deployment succeeds, open https://fribas001.github.io/.
   GitHub may take a few minutes to serve the update.

ALTERNATIVE: PROJECT SITE
For a repository named rf-emf-lab, use
    site-url: https://fribas001.github.io/rf-emf-lab/
in _quarto.yml and use that repository's remote URL. Relative links in this
starter work under a project subpath. Re-render after changing configuration.

EVERYDAY WORKFLOW
1. Continue simulations in the existing Codex project folders.
2. Copy selected, final preview images into assets/.
3. Create or update an examples/*.qmd page with the question, model,
   software versions, results, limits and reproduction links.
4. Add the page to the sidebar in _quarto.yml and examples/index.qmd.
5. Preview, render, commit and push. GitHub Actions rebuilds the site.

FILES TO EDIT
_quarto.yml                 Site identity, menu, sidebar, URL and theme
index.qmd                   Visual landing page
software.qmd                Software availability and project links
tutorials/first-scene.qmd    Starting workflow
tutorials/publish-results.qmd How to add reproducible studies
examples/*.qmd              Gallery and case studies
talks.qmd                   Your two Blender videos
reproducibility.qmd         Experiment metadata and validation guidance
about.qmd                   Attribution and content status
theme.scss, styles.css      Colors, typography and responsive layout
.github/workflows/pages.yml Build/deployment automation

CONTENT NOTES
The local DiffeRT and Mobility work is labeled as local development.
The Antwerp illustration is explicitly the 0.6 demo, while the software
page acknowledges the inspected 0.9 local source. Numerical equivalence
claims are scoped to their fixture. No unsupplied public download links
or blanket tissue-dosimetry claims are invented.

The site includes selected media, not Blender scenes, raw simulation caches,
private manuscript drafts, or the whole Codex folder. Put large reproducible
bundles in versioned Releases or a published research archive, and link them.

REFERENCES
https://bradyajohnston.github.io/MolecularNodes/
https://quarto.org/docs/publishing/github-pages.html
https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages
https://docs.github.com/en/pages/quickstart
