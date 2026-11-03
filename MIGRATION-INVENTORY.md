# One Fact site migration inventory

Source archive: [xtuml/onefactnet](https://github.com/xtuml/onefactnet)  
Target site: [xtuml/onefactinc](https://github.com/xtuml/onefactinc)

## Archive profile

The source repository currently contains 1,447 tree entries, including 335 HTML files and 240 image/media files. It is a static capture of a WordPress site, not a clean export of page content. Many HTML files contain repeated theme markup, plugin assets, scripts, navigation, related-post widgets, and footer content.

The capture also contains 143 root-level `index.html?p=...` files. These are WordPress query-string export artifacts and should not be treated as independent clean pages without checking their canonical content and URL.

## Content categories

| Category | Source examples | Migration approach |
|---|---|---|
| Core pages | Home, Our Team, Get in Touch | Rewrite as clean Jekyll pages; retain established paths |
| Services | Training & Consulting, Support | Convert the useful service descriptions into readable sections |
| Editorial content | Individual article directories and Blog archive | Migrate as dated Jekyll posts after extracting original dates, body text, media, and links |
| Historical/event content | xtUML Days, conferences, announcements | Retain useful material in the blog archive; review stale event calls to action |
| WordPress artifacts | Pagination, feeds, comments, query-string exports | Do not migrate as authored content |
| Media | `wp-content/uploads/` | Copy selected original images into a clean assets directory and update references |

## Pages migrated in the first pass

- `/our-team/` — team listing from the archived Our Team page.
- `/training-consulting/` — training courses and consulting services.
- `/support/` — BridgePoint Pro, Service Pro, and custom engineering summary.
- `/get-in-touch/` — contact information, retaining the archived contact path.
- Six editorial articles in the `_articles` collection: Mount Kilimanjaro, Textual Persistence, Model-Driven Test with TAME, Panda – Open Source Development, MC-Generated Auto-Dispose, and HOWTO Connect to xtUML. Each keeps its original root-level URL slug.
- `/blog/` — a generated index of migrated articles.

The team roster and service descriptions are historical source content. Confirm current accuracy before production cutover.

## URL strategy

The original site used folder-style paths such as `/our-team/`, `/training-consulting/`, and `/get-in-touch/`. Jekyll front matter permalinks will retain those paths even when the source Markdown files live at the repository root. This follows Jekyll's documented page permalink mechanism.

The blog archive should retain each article's original slug path where possible. The original publication date should be preserved as metadata, but the permalink should be explicitly set when it differs from the chosen Jekyll post URL convention.

## Article archive implementation

The archive uses a Jekyll collection named `articles`, with each document assigned an explicit original-style permalink. The captured HTML does not consistently expose reliable publication dates, so the collection currently sorts alphabetically by title rather than assigning fabricated dates. Article content is extracted from the original post-content region; WordPress theme wrappers, scripts, and related-post widgets are not copied. Image references currently point to the original WordPress uploads and must be copied into the new repository before the old WordPress host is retired.

## Next migration phases

1. Extract titles, dates, canonical URLs, body text, and image references for all individual article pages.
2. Build a dated post collection and a blog index; exclude WordPress pagination and query-string duplicates.
3. Copy only media referenced by migrated content, preserving descriptive filenames where practical.
4. Review external links, downloadable files, and obsolete calls to action.
5. Check all internal links and generated URLs on the GitHub Pages preview.
6. Confirm current company contact details, team roster, and service offerings before custom-domain cutover.

## Explicitly deferred

- No changes to the WordPress production site.
- No changes to the existing `xtuml/onefactnet` archive.
- No custom-domain or DNS changes.
- No wholesale copying of WordPress, Elementor, HustleFish, or plugin-generated HTML/CSS/JavaScript.
