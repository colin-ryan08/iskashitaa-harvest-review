# Iskashitaa Gleaning Program — Framework & Implementation Reference

A static, multi-page reference site covering the case for change, the operating and data framework, onboarding requirements, role definitions, and the Salesforce evaluation and proposal for Iskashitaa's gleaning program. Built for GitHub Pages — no build step, no dependencies.

## Pages

| Page | Covers |
|---|---|
| `index.html` | Landing page with links to all five sections |
| `case-for-change.html` | The opportunity, the gaps, research, comparable organizations, vision |
| `framework.html` | Harvest flow, data model, success metrics |
| `onboarding.html` | Entry requirements, gear, progression mechanics, open items |
| `roles.html` | All 11 progression roles + 3 supporting roles |
| `salesforce.html` | Current-state audit, gap list, data-capture strategy, build order |

Shared styling lives in `assets/style.css`; diagrams are in `assets/images/`.

## Publishing to GitHub Pages

1. Push this folder's contents to a GitHub repository (the contents of `github-pages-site/`, not the parent folder — `index.html` should sit at the repo root, or at the root of whichever branch/folder you publish from).
2. In the repository, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to "Deploy from a branch."
4. Choose the branch (commonly `main`) and the folder (`/` if these files are at the repo root, or `/docs` if you placed them in a `docs` folder instead).
5. Save. GitHub will publish at `https://<username>.github.io/<repo-name>/` within a few minutes.
6. Optional — custom domain: add a `CNAME` file containing your domain (e.g., `framework.iskashitaa.org`) to this folder, and point your DNS at GitHub Pages per [GitHub's custom domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

No Jekyll configuration, build process, or external dependencies are required — every page is plain HTML/CSS.

## Updating content

Each page pulls from the source documents in the parent `Iskashitaa Gleaning Framework` folder (the wiki, Executive Summary, Role Definitions) and the `Iskashitaa Salesforce inspection and implementation` folder (the field/object audit, data capture strategy). If those source documents change, the corresponding section of the site should be updated to match — each page cites its source at the bottom.
