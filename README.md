# Hannah Clarke — Portfolio

A small, framework-free portfolio site. Plain HTML, CSS and JavaScript with its
own design-token system and light/dark theming — no build step, no dependencies.
Open `index.html` in a browser, or host the folder anywhere static.

## Structure

```
portfolio/
├── index.html                 # Landing: hero, capabilities, work grid, about, contact
├── work/
│   ├── design-system.html     # Case study — component library
│   ├── icon-library.html      # Case study — icon library
│   ├── create-app-cli.html    # Case study — scaffolding CLI
│   └── ds-assistant.html      # Case study — design-system AI assistant
├── css/
│   ├── tokens.css             # Design tokens + light/dark themes (the site's "design system")
│   ├── base.css               # Reset, typography, layout helpers, scroll-reveal
│   └── components.css         # Nav, buttons, cards, timeline, footer, etc.
├── js/
│   └── main.js                # Theme toggle, scroll reveals, nav state (no dependencies)
└── assets/                    # (reserved for images/exports)
```

## Run it

```bash
# Just open it:
open index.html

# …or serve it (any static server works):
python3 -m http.server 8000   # then visit http://localhost:8000
```

To deploy: drag the folder onto Netlify, push to GitHub Pages, or upload to any
static host. There is nothing to build.

## Before you publish — optional polish

Contact details are now wired in from your profile (personal email
`hc.hannahclarke@gmail.com`, LinkedIn, GitHub). Remaining optional touches:

- **Photo / OG image**: optional. There's an `assets/` folder if you want to add
  a headshot or a social-share image.
- **Tone**: copy is written to be confident but not inflated. Adjust to taste.
- **Podcast link**: the "Listen" link points at the podcast hub — swap in the
  direct episode URL when you have it (and confirm the episode number).

## A note on accuracy & sanitisation

Every contribution claim was derived from the **git history of your repositories**
(filtered to your authorship), not guessed. Work is framed as *yours within a team
effort*, and I deliberately did **not** claim things the history doesn't support
(e.g. icon artwork, or teammates' components bundled into release commits).

Because this is a **public** site, it has been sanitised of employer-internal detail
— while keeping the things that are already public:

- **Employer named** (Intapp) in the intro and in recommendation attributions —
  this is public information that appears on any CV.
- **Recommendations are named** — these are public LinkedIn recommendations whose
  authors chose to attach their names to them.
- No internal repository names, ticket IDs, or PR numbers.
- Internal infrastructure generalised (e.g. internal registry → "a private package registry").
- Project case studies still use descriptive titles ("Component Library",
  "create-app") rather than internal product names.
- Public third-party tools are named as-is (Figma, Storybook, Chromatic, Slack,
  Azure, Anthropic SDK, MCP, etc.).

If you later want internal product/repo names woven back in too, that's a quick change.
```
