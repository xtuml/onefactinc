# One Fact site migration inventory

Source archive: [xtuml/onefactnet](https://github.com/xtuml/onefactnet)  
Target site: [xtuml/onefactinc](https://github.com/xtuml/onefactinc)

## Archive profile

The source repository contains 1,447 tree entries, including 335 HTML files and 240 image/media files. It is a static capture of a WordPress site, not a clean export of page content. Many HTML files contain repeated theme markup, plugin assets, scripts, navigation, related-post widgets, and footer content.

The capture also contains 143 root-level `index.html?p=...` files. These are WordPress query-string export artifacts and should not be treated as independent clean pages without checking their canonical content and URL. Blog pagination, feeds, comments, and generated WordPress artifacts are likewise not authored content.

## Content categories

| Category | Source examples | Migration approach |
|---|---|---|
| Core pages | Home, Our Team, Get in Touch | Rewrite as clean Jekyll pages; retain established paths |
| Services | Training & Consulting, Support | Convert useful service descriptions into readable sections |
| Editorial content | Individual article directories and Blog archive | Migrate as dated Jekyll collection documents after extracting original dates, body text, media, and links |
| Historical/event content | xtUML Days, conferences, announcements | Retain useful material in the blog archive; review stale event calls to action |
| WordPress artifacts | Pagination, feeds, comments, query-string exports | Do not migrate as authored content |
| Media | `wp-content/uploads/` | Copy selected original images into a clean assets directory and update references |

## Pages migrated

- `/our-team/` — team listing from the archived Our Team page.
- `/training-consulting/` — training courses and consulting services.
- `/support/` — BridgePoint Pro, Service Pro, and custom engineering summary.
- `/get-in-touch/` — contact information, retaining the archived contact path.
- Six editorial articles in the `_articles` collection, each retaining its original root-level slug:
  - Mount Kilimanjaro — January 13, 2026
  - Textual Persistence — December 28, 2021
  - Model-Driven Test with TAME — January 25, 2021
  - Panda – Open Source Development — May 12, 2020
  - MC-Generated Auto-Dispose — April 21, 2020
  - HOWTO Connect to xtUML — April 15, 2020
- `/blog/` — generated newest-first index of migrated articles, with publication dates and short descriptions.

The dates above come from the archived WordPress RSS feed, rather than guesses based on file names. The feed exposes only its ten most recent entries; six of those have been migrated so far. Older articles remain to be inventoried and prioritized.

The team roster and service descriptions are historical source content. Confirm current accuracy before production cutover.

## URL and article strategy

The original site used folder-style paths such as `/our-team/`, `/training-consulting/`, and `/get-in-touch/`. Jekyll front matter permalinks retain those paths even when source files live elsewhere in the repository.

The article collection uses explicit original-style permalinks. Publication dates are stored as metadata and displayed in the blog index and article headers. Article content is cleaned and rewritten as readable HTML/Markdown; WordPress theme wrappers, scripts, and related-post widgets are not copied.

Some migrated articles still reference images or downloadable files on the original `onefact.net` WordPress host. Those dependencies must be copied into the new repository and checked before the old host can be retired. The YouTube embed remains an intentional third-party dependency.

## Next migration phases

1. Inventory and migrate the remaining editorial archive, using WordPress RSS metadata where available and avoiding duplicate feed/pagination artifacts.
2. Copy only media referenced by migrated content, preserving descriptive filenames where practical.
3. Review external links, downloadable files, and obsolete calls to action.
4. Check all internal links, images, embeds, and generated URLs on the GitHub Pages preview.
5. Confirm current company contact details, team roster, and service offerings before custom-domain cutover.

## Explicitly deferred

- No changes to the WordPress production site.
- No changes to the existing `xtuml/onefactnet` archive.
- No custom-domain or DNS changes.
- No wholesale copying of WordPress, Elementor, HustleFish, or plugin-generated HTML/CSS/JavaScript.
