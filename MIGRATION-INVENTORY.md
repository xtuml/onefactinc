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
- Twenty-five editorial articles in the `_articles` collection, each retaining its original root-level slug:
  - Mount Kilimanjaro — January 13, 2026
  - Textual Persistence — December 28, 2021
  - Model-Driven Test with TAME — January 25, 2021
  - Panda – Open Source Development — May 12, 2020
  - MC-Generated Auto-Dispose — April 21, 2020
  - HOWTO Connect to xtUML — April 15, 2020
  - Diagram and Element Types — April 7, 2020
  - xtUML Days 2020 Save-the-Date — April 1, 2020
  - OAL, MASL and now ASL — April 1, 2020
  - Color Your Model — March 20, 2020
  - Dawn of Ciera — February 1, 2020
  - OOA of MASL — January 16, 2020
  - Shlaer-Mellor Runtime — August 21, 2019
  - Requirement Tracing — November 21, 2019
  - xtUML in the Field — November 11, 2019
  - Java and BridgePoint — October 22, 2019
  - State Diagram, State Table — April 10, 2019
  - Continuous Integration — April 3, 2019
  - Amazon Web Services (AWS) Lambda — December 19, 2018
  - Model-Based Testing of Self-Driving Cars — August 1, 2017
  - Issue Tracking with Redmine — February 18, 2016
  - Action Language Fundamentals — February 17, 2016
  - Action Language — February 16, 2016
  - Modeling Before Programming — July 4, 2016
  - Modeling Domain Specific Languages — January 12, 2015
- `/blog/` — generated newest-first index of migrated articles, with publication dates and short descriptions.

The ten newest article dates came from the archived WordPress RSS feed. Dates for the older migrated articles were verified against the archived WordPress REST API records. Additional candidates remain inventoried from blog pagination pages 2–23 in [OLDER-ARTICLE-INVENTORY.md](OLDER-ARTICLE-INVENTORY.md).

The team roster and service descriptions are historical source content. Confirm current accuracy before production cutover.

## URL and article strategy

The original site used folder-style paths such as `/our-team/`, `/training-consulting/`, and `/get-in-touch/`. Jekyll front matter permalinks retain those paths even when source files live elsewhere in the repository.

The article collection uses explicit original-style permalinks. Publication dates are stored as metadata and displayed in the blog index and article headers. Article content is cleaned and rewritten as readable HTML/Markdown; WordPress theme wrappers, scripts, and related-post widgets are not copied.

All 25 migrated articles retain their original paths and display their source publication dates. Twenty-six image assets used by these articles have now been copied into this repository under `assets/images/`, and article image references have been updated to use Jekyll's `relative_url` filter. One source image for the xtUML in the Field article was a zero-byte file in the archive and has been omitted; the other four model images are local. The two linked research/project PDFs (the self-driving-car paper and Panda requirements specification) are not present in the static archive. Their links temporarily point to the original WordPress media URLs; recover and store these files locally before retiring WordPress. YouTube embeds remain intentional third-party dependencies.

## Next migration phases

1. Review and migrate selected older editorial content from the title-level inventory. Recover reliable publication dates before adding entries to the dated blog index, and avoid duplicate feed/pagination artifacts.
2. Recover the Panda project PDF and any other required downloadable files; store them locally under `assets/downloads/`.
3. Review external links, downloadable files, and obsolete calls to action.
4. Check all internal links, images, embeds, and generated URLs on the GitHub Pages preview.
5. Confirm current company contact details, team roster, and service offerings before custom-domain cutover.

## Explicitly deferred

- No changes to the WordPress production site.
- No changes to the existing `xtuml/onefactnet` archive.
- No custom-domain or DNS changes.
- No wholesale copying of WordPress, Elementor, HustleFish, or plugin-generated HTML/CSS/JavaScript.
