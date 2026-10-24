# WSU Quantum Sciences

Jekyll site for the Wright State University Quantum Sciences club.
Published at <http://wsu-quantum-sciences.github.io>.

## Running it locally

```sh
bundle install
bundle exec jekyll serve
```

Then open <http://127.0.0.1:4000>.

## Where things live

| Path | What it is |
|------|------------|
| `pages/` | The About / Club / People / Research / Resources pages |
| `_posts/` | Blog posts |
| `_data/settings.yml` | Nav menu, social links, UI strings |
| `_sass/` | Stylesheet partials, imported by `assets/css/main.scss` |
| `_layouts/`, `_includes/` | Page templates |

Breakpoints and colours are defined at the top of `assets/css/main.scss`.
Breakpoints must be absolute units — a percentage makes every `@media`
rule invalid and the browser discards it silently.
