# Ardiment · suggested repository settings

These are prepared values, not completed external changes. The owner must apply them in GitHub. None require a new domain or account.

## About description

```text
Ardiment (formerly ASCEND) — a personal execution PWA for tasks, study, projects, routines, and progression. English/Arabic, AI-assisted planning, and browser-encrypted sync. Private beta 0.7.1.1.
```

## Website

```text
https://ardiment-beta-nine.vercel.app
```

This is the existing owner-provided application address. Its availability and deployment version are not independently audited by the showcase kit.

## Topics

```text
ardiment
productivity
task-management
personal-progression
study-planner
project-management
pwa
javascript
nodejs
supabase
gemini
arabic
rtl
local-first
ai-assisted-development
```

## Social preview

In the repository **Settings → General → Social preview**, upload:

`docs/assets/social-preview.png`

The included PNG is 1280 × 640 and contains no private account data. It is separate from the live app's own Open Graph metadata and from your account avatar.

## Optional repository-name change

The current inspected URL is `https://github.com/HassanAsali/ASCEND`. The kit works at that path using relative links; renaming is not required to render the updated page.

To align the repository slug with the product, the owner can use **Settings → General → Repository name**, enter `Ardiment`, and select **Rename** if available. Do not create a replacement repository or delete the existing one just to change its name.

After a successful rename, use the actual URL shown by GitHub. For an existing local checkout, update the remote to that confirmed address. For example, only if the resulting slug is exactly `Ardiment`:

```bash
git remote set-url origin https://github.com/HassanAsali/Ardiment.git
```

GitHub documents redirects for ordinary repository traffic after a rename, with exceptions such as project-site URLs and references to actions hosted in the renamed repository. Check existing Pages/deployment/integration references rather than assuming every external URL follows the redirect. Do not reuse the old repository name for a new repository if you depend on the old redirect.

Repository renaming does not change the Vercel app hostname, Supabase URL configuration, PWA identity, or stored recovery keys. Those are separate systems.

## Sources

- [GitHub: renaming a repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/renaming-a-repository)
- [GitHub: social media preview](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/customizing-your-repositorys-social-media-preview)
- [GitHub: repository customization](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository)
