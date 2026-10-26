# Publish the Ardiment showcase

This kit updates the presentation of the existing repository. It does **not** deploy the app or upload its complete current private source.

## Required files

Upload the **contents** of this kit into the repository root:

- `README.md`
- `docs/` with its supplied `assets/`, `media/`, `brand/`, and reference documents
- `UPLOAD.md`, `UPLOAD-AR.md`, and `REPOSITORY-SETTINGS.md` for maintainer instructions

The README depends on relative asset/document paths. Do not upload only the README, rename asset files, or place the entire kit inside an extra parent folder. Merge the supplied `docs` contents with the existing folder; retain unrelated files and historical source.

No `.env`, account data, recovery files, passwords, provider keys, or complete current app source belong in this showcase upload.

## Through GitHub in a browser

1. Open the existing repository root: <https://github.com/HassanAsali/ASCEND>.
2. Select **Add file → Upload files**.
3. Drag in the extracted kit's root files and `docs` folder, preserving their paths. Upload the extracted files, not the ZIP itself.
4. Check the file paths in the upload list. `README.md` must be at the root and the banner must be under `docs/assets/`.
5. Commit with a message such as `Rebrand showcase to Ardiment 0.7.1.1`.
6. Open the rendered README and check the banner, mobile/desktop images, collapsible sections, diagrams, and document links.

GitHub's documented browser limit is 100 files per upload and 25 MiB per file. This kit is kept below those limits. If the browser upload workflow is inconvenient, use an existing local checkout instead.

## Through an existing local checkout

Copy the kit's files into your already configured local repository, then review only these paths:

```bash
git status --short
git add README.md UPLOAD.md UPLOAD-AR.md REPOSITORY-SETTINGS.md docs/
git diff --cached --stat
git diff --cached --name-only
git commit -m "Rebrand showcase to Ardiment 0.7.1.1"
git push
```

Inspect the staged file list before committing. Existing unrelated modifications inside `docs/` should not be accidentally included.

## Finish the repository presentation

Use [REPOSITORY-SETTINGS.md](REPOSITORY-SETTINGS.md) for the proposed About text, website, topics, and social preview. The repository name is controlled separately in GitHub Settings. A README heading does not change the repository URL.

If a GitHub-connected deployment exists, check its deployment rules before committing; adding showcase files can still trigger configured automation even though this kit contains no runtime changes.

## Evidence and image handling

The README's product captures are actual 0.7 app UI with synthetic content, clearly labeled as fixture captures. Do not replace them with private user/account screenshots without redaction. The known Cloudflare overlap is documented without publishing the user's screenshot.

The banner has a static PNG fallback for reduced motion. SVG sources, local images, native details sections, relative links, and Mermaid keep the page compatible with GitHub's supported rendering. Custom CSS/JavaScript is not required. Final GitHub rendering must be checked after upload.

## Official references

- [Adding files to a repository](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)
- [About READMEs and relative links](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
- [Creating Mermaid diagrams](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-diagrams)
- [Collapsed sections](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-collapsed-sections)
- [Social media preview](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/customizing-your-repositorys-social-media-preview)
- [Renaming a repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/renaming-a-repository)
