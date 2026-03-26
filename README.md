<pre align="center">
Glacio is a polished Astro blog template for personal sites, notes, and portfolios.
</pre>

<div align="center">
  <img alt="Template Logo" src="./public/template-mark.svg" width="140px">
</div>

<p align="center">
  Built with Astro, TypeScript, Tailwind CSS, daisyUI, MDX, and Pagefind
</p>

## 📷 Preview

<table>
  <tr>
    <td align="center"><strong>Light</strong></td>
    <td align="center"><strong>Dark</strong></td>
  </tr>
  <tr>
    <td><img alt="Glacio light preview" src="./public/image/white.png"></td>
    <td><img alt="Glacio dark preview" src="./public/image/black.png"></td>
  </tr>
</table>

## ✨ Features

- ✅ Light / dark mode
- ✅ Responsive layout
- ✅ MDX-based blog content
- ✅ Categories, tags, archives, RSS, and sitemap
- ✅ Pagefind local search
- ✅ Iconify icon support
- ✅ Reusable pages for home, about, projects, and links
- ✅ Friendly for template customization

## 🧩 About This Template

This project, Glacio, is a heavily modified derivative of [Frosti](https://github.com/EveSunMaple/Frosti).

It started as a learning reference and was later reworked substantially in structure, pages, styling, and content organization. This repository is intended to be shared as a reusable template rather than as a direct mirror of the original project.

Main differences from the original basis include:

- rewritten homepage and profile content structure
- customized about, project, and friend-link pages
- different default content and template-safe placeholder data
- cleaned repository content for public reuse
- adjusted configuration and asset defaults for easier forking

## ⬇️ Usage

1. Install `pnpm` if you do not already have it.

```sh
npm i -g pnpm
```

2. Clone this repository.

```sh
git clone <your-repo-url>
cd <your-project-folder>
```

3. Install dependencies.

```sh
pnpm install
```

4. Start local development.

```sh
pnpm run dev
```

5. Generate the search index when needed.

```sh
pnpm run search:index
```

6. Build for production.

```sh
pnpm run build
pnpm run preview
```

## 🔧 Configuration

The main site configuration lives in `frosti.config.yaml`.

You can update:

- site title, tab text, description, language, and favicon
- theme settings
- navigation menu and submenus
- user name, avatar, personal site, and social links

Example:

```yaml
site:
  tab: Glacio
  title: Glacio
  description: Glacio is a polished Astro blog template for personal sites, notes, and portfolios.
  language: en
  favicon: /template-mark.svg

user:
  name: Glacio User
  site: "https://example.com/"
  avatar: /template-avatar.svg
```

## ✒️ Article Frontmatter

| Name | Meaning | Required |
| :--- | :------ | :------: |
| `title` | Article title | Yes |
| `description` | Article description | Yes |
| `pubDate` | Publication date | Yes |
| `updated` | Updated date | No |
| `image` | Cover image | No |
| `categories` | Article categories | No |
| `tags` | Article tags | No |
| `badge` | Badge text | No |
| `draft` | Draft status | No |

Sample article files are in `src/content/blog/`.

## 💬 Comments

This template does not ship with a live comment backend enabled by default.

If you want comments:

- connect your own Waline or other comment service
- update the related component configuration before deployment
- verify all external service URLs belong to you

## 🌍 i18n

Interface text is managed in `src/i18n/translations.yaml`.

You can:

- change the default language in `frosti.config.yaml`
- edit existing translations
- add a new language section if needed

## 🚀 Updating

This repository includes `frosti.update.sh` as a convenience script for template maintenance.

Before using it, make sure the upstream repository URL inside the script is changed to your own maintained source if needed.

## 👀 Notes

- The repository has been cleaned to remove prior personal profile content and private-facing materials.
- Placeholder text and assets are included so the template can be forked safely.
- Replace all example links, avatars, and profile copy before publishing your own site.

## 🎉 Acknowledgements

- [EveSunMaple / Frosti](https://github.com/EveSunMaple/Frosti) for the original project that inspired and informed this template
- This repository is not the original Frosti project; it is a substantially modified derivative built for a different use case
