# Danish Yaqoob — academic homepage

A complete, responsive, static website for **https://danish-yaqoob.github.io/**.
which uses the CC0 Minimal Light theme. No installation, build step, JavaScript,
Jekyll, or API keys are required.

## Publish on GitHub Pages

1. Sign in to GitHub as **danish-yaqoob**.
2. Create a **public** repository named exactly **danish-yaqoob.github.io**.
3. Upload the **contents** of this folder to the repository root. `index.html`
   must be at the root, not inside another `danish-yaqoob.github.io` folder.
   Include `assets/`, and `.nojekyll` if your upload method shows hidden files.
4. Commit your files to the `main` branch.
5. Open the repository's **Settings → Pages**. Under **Build and deployment**,
   choose **Deploy from a branch**, select **main** and **/ (root)**, then **Save**.
6. Wait for GitHub's Pages deployment to finish. Your homepage will be at
   **https://danish-yaqoob.github.io/**. Check the repository's Actions tab if
   deployment fails. A first deployment can take several minutes.

Alternatively, after creating the empty repository, run these commands from
this website folder (GitHub will request authentication through your Git setup):

```sh
git init -b main
git add .
git commit -m "Add academic homepage"
git remote add origin https://github.com/danish-yaqoob/danish-yaqoob.github.io.git
git push -u origin main
```

Then complete step 5 above. Never put access tokens in website files.

## Edit your content

- **Biography, title, institution, profile links, news, publications:** edit
  `index.html`. The page contains comments at the main editing points.
- **Photo:** replace `assets/img/profile.png` with your own square portrait,
  keeping the filename, or update the image path in `index.html`.
- **Email:** add `<a href="mailto:YOUR_EMAIL">YOUR_EMAIL</a>` below your affiliation.
- **CV:** save your PDF as `assets/cv.pdf` and uncomment the example CV link.
- **Colors, font sizes, spacing:** edit `assets/css/style.css`.
- **Social previews:** update the `og:` metadata in `index.html` if your URL or
  image changes. Google Fonts is optional; Georgia is the local fallback.

The current page uses your confirmed portrait, title, institution, public email,
and public GitHub bio, plus all 15 entries extracted from your Google Scholar profile. No supervisor, awards,
or unverified service roles have been inserted. Send newer paper URLs to expand
the selected list.

## Preview locally

Open `index.html` directly in a browser, or run:

```sh
python -m http.server 8000
```

Visit http://localhost:8000. Press Ctrl+C in that terminal to stop the server.
The layout stacks on small screens, supports system dark mode, and has a print
stylesheet. All content and links work without JavaScript.

## Content sources

Checked on November 10, 2026:

- User-supplied Scholar, LinkedIn, and GitHub URLs.
- Public GitHub profile: https://api.github.com/users/danish-yaqoob
- Portrait: https://avatars.githubusercontent.com/u/293824700?v=4
- Publication metadata: https://pubmed.ncbi.nlm.nih.gov/39579125/
- Publication metadata: https://pubmed.ncbi.nlm.nih.gov/38894886/
- Equal-author contribution: https://pmc.ncbi.nlm.nih.gov/articles/PMC11185247/
- Publication metadata: https://pubmed.ncbi.nlm.nih.gov/35341979/
- University media coverage: https://www.sdmpu.edu.cn/2022/0402/c2013a97082/page.htm
- Reference design: https://ruoqi-liu.github.io/
- Theme: https://github.com/yaoyao-liu/minimal-light (CC0; see THEME-LICENSE.txt).

Google Scholar was successfully retrieved on November 10, 2026. All 15 entries
are included, newest first; two entries have no year. This list includes
manuscripts and a book entry as well as journal articles. Truncated author
lists remain abbreviated, and missing metadata is not invented. The original
extracted metadata is in `assets/data/publications.json` and `publications.csv`.
This is a static snapshot: edit the HTML to add future publications.

Google Scholar, LinkedIn, and GitHub logos are bundled locally from
Simple Icons v11 (CC0): https://github.com/simple-icons/simple-icons/tree/11.0.0.
The brand names and logos remain the property of their respective owners. This package has not been
published to GitHub; publication requires access to your GitHub account.
