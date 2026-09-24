---
target: my website
total_score: 17
max_score: 32
na_heuristics: 7,10
p0_count: 1
p1_count: 3
target_identity: "file:/Users/justinasposiunas/Dev/posiunas.github.io/themes/posiunas/layouts/index.html"
target_fingerprint: "sha256:6a2ae8723d9c020e3b3446ac30b012928477cee4b9818a5c7d3c12b5cc63ecb4"
target_path: /Users/justinasposiunas/Dev/posiunas.github.io/themes/posiunas/layouts/index.html
timestamp: 2026-09-24T22-34-18Z
slug: themes-posiunas-layouts-index-html
---
# Critique: justinas.eu (homepage, posts, /uses/, 404)

## Design Health Score: 17/32 (heuristics 7 and 10 were not applicable)
| # | Heuristic | Score | Key issue |
|---|---|---|---|
| 1 | Visibility of system status | 2 | No indication of where you are on the site. Thumbnails only show colour on hover, which never happens on a touchscreen |
| 2 | Match with the real world | 3 | The "t8" icon means nothing to someone who doesn't already know it |
| 3 | User control and freedom | 1 | Posts end with nothing: no next post, no footer, no way to follow |
| 4 | Consistency and standards | 2 | Date formats differ between pages. The book counter applies to every h3 on the site. The avatar vanishes on mobile |
| 5 | Error prevention | 2 | An unlabelled WhatsApp icon exposes a personal phone number |
| 6 | Recognition rather than recall | 2 | Seven unlabelled icons. Nothing links to /uses/. /posts/ returns a 404 |
| 7 | Flexibility and efficiency | n/a | A static personal site has no expert workflows |
| 8 | Aesthetic and minimalist design | 3 | Calm and restrained, but the 5rem gaps above each h2 look like holes on mobile |
| 9 | Error recovery | 0 | The 404 page and the post list template are empty files |
| 10 | Help and documentation | n/a | A personal site has nothing to document |

## Priority issues
- [P0] Broken states: 404.html, list.html and footer.html are 0-byte files. As a result, /posts/ returns a 404 and any bad link lands on a dead-end page that isn't styled like the site.
- [P1] Dark-mode contrast: --quick-silver #666 on #2e2e2e measures 2.37:1. It is used for the subtitle, dates, h2 labels, icons and time elements. The detector flagged it on every page.
- [P1] The homepage doesn't say who Justinas is: there is no role and no pitch, just 7 unlabelled icons of equal weight. The meta description is "My virtual personal presence starts there!"
- [P1] Sharing and SEO are missing: no og: or twitter: tags, the same description on every page, titles without the site name, no canonical link, and no link to the RSS feed.
- [P2] Mobile bugs: `.mini-profile span` also hides `.mini-avatar`. `#card-subtitle` has nowrap, which causes horizontal scrolling at 360px.

## Minor
- The homepage thumbnails load 635KB (85% of the page weight) to fill three 240×72 slots.
- The supercar hero has a 9.6:1 aspect ratio.
- Hero images have no width/height attributes.
- /uses/ is dated 2021 (iPhone X, Big Sur), which contradicts the Omarchy post.
- The 8 black "Get hardcover" buttons are amzn.to links with no affiliate disclosure.
- In-post links are the same colour as body text.
- The subtitle is marked up as an h2.
- There are no main, nav or footer landmarks.
- The Font Awesome kit is loaded for just 7 icons.
