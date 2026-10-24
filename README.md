# QuantumScienceIdea

Simple website for Quantum Sciences we can use for the updated website,
just for brainstorming right now.

A Jekyll site for the Wright State University Quantum Sciences club,
rebuilt from the Millennial-theme site at
<http://wsu-quantum-sciences.github.io>.

## Running it locally

```sh
bundle install
bundle exec jekyll serve --baseurl ""
```

Then open <http://127.0.0.1:4000>.

`--baseurl ""` is there because `_config.yml` sets `baseurl` to the repo
path, which is what GitHub Pages needs. Without the override a local
server mounts the site under `/QuantumScienceIdea/` instead of `/`.

## Where things live

| Path | What it is |
|------|------------|
| `index.md` | Home page (logo and intro) |
| `pages/` | Club, People, Research and Resources |
| `blog/index.html` | Blog index; posts live in `_posts/` |
| `_data/settings.yml` | Nav menu, social links, UI strings |
| `_sass/` | Stylesheet partials, imported by `assets/css/main.scss` |
| `_layouts/`, `_includes/` | Page templates |
| `assets/img/people/_archive/` | Photos kept but not published |

Breakpoints and colours are defined at the top of `assets/css/main.scss`.
Breakpoints must be absolute units — a percentage makes every `@media`
rule invalid and the browser discards it silently.
