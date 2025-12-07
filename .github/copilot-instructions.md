<!-- Copied guidance for AI coding agents tailored to this Jekyll portfolio repo -->
# Copilot Instructions — JoseJVV.github.io

Purpose: concise, actionable notes to help an AI agent work productively in this repo.

- **Project type**: A GitHub Pages portfolio built with Jekyll using the `mmistakes/minimal-mistakes` remote theme. See `_config.yml`.
- **Source of truth**: `_config.yml` configures theme, skin (`minimal_mistakes_skin: "dark"`), plugins and SASS dir (`assets/css`).

- **Where content lives**: Markdown pages at the repo root and top-level folders (`ilustracion/`, `3d/`, `contacto/`). Home page: `index.md`.
- **Assets**: images and SASS live under `assets/` — `assets/images/` and `assets/css/main.scss` is the primary stylesheet.

- **Styling conventions**:
  - `assets/css/main.scss` contains front-matter so Jekyll processes it (the leading `---` block). Do not remove that front-matter.
  - The file imports the theme SASS (`@import "minimal-mistakes/skins/dark"` and `@import "minimal-mistakes"`). Adjust local variables (e.g. `$brand-color`) here to change the color palette.

- **Layout defaults**: `_config.yml` sets default page layout to `single` with `classes: wide`. New pages normally do not need explicit `layout` unless deviating from defaults.

- **Build & preview**:
  - This repository relies on GitHub Pages' `remote_theme`. There is no `Gemfile` in the repo, so CI/build is expected to happen on GitHub Pages.
  - To preview locally, either add a `Gemfile` (preferred) with `github-pages` or install Jekyll and the Minimal Mistakes theme manually.
  - Typical local preview commands (run in a Windows PowerShell with Ruby/Jekyll installed):

    - `jekyll serve --livereload`  # if Jekyll and the theme are globally available
    - `bundle exec jekyll serve`   # if you add a `Gemfile` and use Bundler

  - If local build fails because the remote theme is missing, add a minimal `Gemfile` or install the `minimal-mistakes` gem locally.

- **Content conventions**:
  - Pages and sections are written in Spanish (see `index.md` and `_config.yml` `locale: "es-ES"`). Keep new copy consistent with locale.
  - The README documents a `PROYECTOS/` convention for storing project resources (images). Use `assets/images/` when you want the site to reference images via `/assets/images/...` as the theme expects.

- **When editing theme-related files**:
  - Avoid changing the `remote_theme` setting unless you also add a `Gemfile` and vendor or pin the theme. Theme SASS imports in `main.scss` depend on the theme being available.
  - To change skin, edit `_config.yml` (`minimal_mistakes_skin`) or override variables in `assets/css/main.scss` before the `@import` lines.

- **Common quick tasks examples**:
  - Add a project page: create `PROYECTOS/ilustracion/my-project/index.md` or a page under `ilustracion/` with front matter (title, date optional). Content will inherit `layout: single`.
  - Update the avatar: replace `assets/images/avatar.png` and keep the same path referenced in `_config.yml`.

- **Plugins & performance**:
  - `_config.yml` lists `jekyll-include-cache`. Keep this in mind when editing included partials — changes to includes may be cached during builds.

- **Diagnostics & debugging**:
  - If CSS changes don't appear, ensure the SASS front-matter remains and that the theme SASS is available to Jekyll.
  - If pages look different locally vs GitHub, check for a missing `Gemfile` or theme dependency; GitHub Pages provides the remote theme during build.

- **Safety / do not change**:
  - Do not remove the top YAML front matter from `assets/css/main.scss` (Jekyll uses it to process the stylesheet).
  - Avoid renaming `_config.yml` keys unless you understand the impact on theme behavior (skin, plugins, sass_dir).

If anything here is unclear or you want additional examples (local `Gemfile`, Docker preview snippet, or content templates), tell me which part to expand. 
