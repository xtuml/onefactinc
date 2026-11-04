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

  - Backslash Seminar Japan — publication date not yet verified
  - IEEE HKN SLC 2017 — publication date not yet verified
  - Keynote Speaker — publication date not yet verified
  - Lafayette Business Expo — publication date not yet verified
  - Where Does the Name “One Fact” Come From? — publication date not yet verified
  - PIC Members — publication date not yet verified
  - Saab Coming to West Lafayette — publication date not yet verified
  - xtUML Days 2019 UK (1) — publication date not yet verified


- `/our-team/` — team listing from the archived Our Team page.
- `/training-consulting/` — training courses and consulting services.
- `/support/` — BridgePoint Pro, Service Pro, and custom engineering summary.
- `/get-in-touch/` — contact information, retaining the archived contact path.
- One hundred fifteen editorial articles in the `_articles` collection, each retaining its original root-level slug:
  - Einstein's Riddle — April 26, 2018
  - Union — March 1, 2018
  - Semantic Steps — August 7, 2015
  - Three Layers — July 29, 2015
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
  - Winter Computer Science Intern — publication date not yet verified
  - Shinshu Class — publication date not yet verified
  - Modeling Before Programming — publication date not yet verified
  - Open Source BridgePoint — publication date not yet verified
  - Future of Executable UML — publication date not yet verified
  - Getting Started with GitHub — publication date not yet verified
  - Revision Control — publication date not yet verified
  - Semantic Steps — publication date not yet verified
  - UML-RT + xtUML — publication date not yet verified
  - xtUML on Modeling Languages — publication date not yet verified
  - Model Compiler Builders — publication date not yet verified
  - Simulated Time — publication date not yet verified
  - State Save — publication date not yet verified
  - Symmetric Difference — publication date not yet verified
  - Difference — publication date not yet verified
  - Intersection — publication date not yet verified
  - Union — publication date not yet verified
  - Three Layers — publication date not yet verified
  - Find a Bug; Fix a Bug — publication date not yet verified
  - We Like AsciiDoc — publication date not yet verified
  - Big Machine Big Model — publication date not yet verified
  - Debugging Sumo — publication date not yet verified
  - C Model Compiler Summer — publication date not yet verified
  - Super/Sub — publication date not yet verified
  - LEGO in Research — publication date not yet verified
  - BeagleBone Black — publication date not yet verified
  - AUTOSAR — publication date not yet verified
  - Jenkins — publication date not yet verified
  - Collapsed Referential — publication date not yet verified
  - Model API? — publication date not yet verified
  - xtUML Interfaces — publication date not yet verified
  - 2 Views — publication date not yet verified
  - Good Language — publication date not yet verified
  - Applications then Models then Tools — publication date not yet verified
  - Incremental, Always Advancing — publication date not yet verified
  - Model Translation FAQs — publication date not yet verified
  - BridgePoint is Moving to Eclipse 4.4 (Luna) — publication date not yet verified
  - Qt and Squish and xtUML Together — publication date not yet verified
  - Eclipse Oxygen — publication date not yet verified
  - Eclipse Mania — publication date not yet verified
  - Eclipse Governance — publication date not yet verified
  - Returning Strings in C — publication date not yet verified
  - Initial State — publication date not yet verified
  - Autosampler — publication date not yet verified
  - Gripen E — publication date not yet verified
  - Electric Parking Brake Model Snippet — publication date not yet verified
  - Modeling Education — publication date not yet verified
  - MDD at Shinshu U — publication date not yet verified
  - MODELS — publication date not yet verified
  - xtUML Days 2019 UK Presentations — publication date not yet verified
  - xtUML Days 2019 In Motion — publication date not yet verified
  - BridgePoint Pro v6.16 — publication date not yet verified
  - Papyrus Industry Consortium 2019 — publication date not yet verified
  - xtUML in Portsmouth UK — publication date not yet verified
  - 1,3,5+ Application, Dialects, Architectures — publication date not yet verified
  - Always Advancing: xtUML release 5.3.4 — publication date not yet verified
  - Announcing xtUML 2015 — publication date not yet verified
  - Collaborative Development using eGit — publication date not yet verified
  - Models 2015 — publication date not yet verified
  - MODELS 2017 EXE and MDETools — publication date not yet verified
  - xtUML at Shinshu 2018 — publication date not yet verified
  - xtUML + UML-RT — publication date not yet verified
  - ISO26262Day — publication date not yet verified
  - xtUML Resources — publication date not yet verified
  - xtUML.jp — publication date not yet verified
  - xtUML Day 2017 Linköping Presentations — publication date not yet verified
  - xtUML Day 2017 UK — publication date not yet verified
  - xtUML Days 2018 at MODELS — publication date not yet verified
  - EclipseCON North America 2016 — publication date not yet verified
  - Senior Project — publication date not yet verified
  - Academy of Global Engineering — publication date not yet verified
  - Chief Software Architect — publication date not yet verified
  - Community Chat — publication date not yet verified
  - Escher — publication date not yet verified
  - Experiment — publication date not yet verified
  - MT-CPS’18 — publication date not yet verified
  - xtUML 2015 Is History — publication date not yet verified
  - xtUML Days next week — publication date not yet verified
- `/blog/` — generated index of migrated articles, dated articles newest-first followed by undated articles alphabetically.

The ten newest article dates came from the archived WordPress RSS feed. Dates for the older migrated articles were verified against the archived WordPress REST API records. Additional candidates remain inventoried from blog pagination pages 2–23 in [OLDER-ARTICLE-INVENTORY.md](OLDER-ARTICLE-INVENTORY.md).

The team roster and service descriptions are historical source content. Confirm current accuracy before production cutover.

## URL and article strategy

The original site used folder-style paths such as `/our-team/`, `/training-consulting/`, and `/get-in-touch/`. Jekyll front matter permalinks retain those paths even when source files live elsewhere in the repository.

The article collection uses explicit original-style permalinks. Publication dates are stored as metadata and displayed in the blog index and article headers. Article content is cleaned and rewritten as readable HTML/Markdown; WordPress theme wrappers, scripts, and related-post widgets are not copied.

All 111 migrated articles retain their original paths. Articles with verified dates display those dates; articles whose dates have not yet been verified are kept in a separate undated section of the blog index. The repository currently contains 143 files under `assets/images/`, including the logo, article illustrations and photographs, and four team portraits integrated into the Our Team page. Article image references have been converted to local paths using Jekyll's `relative_url` filter; the latest full article scan found no remaining references to WordPress-hosted image files. The six newly migrated technical articles also have their selected images copied into `assets/images/` and use local `relative_url` paths. One source image for the xtUML in the Field article was a zero-byte file in the archive and has been omitted; the other four model images are local. The Panda requirements PDF and self-driving-car paper references have been removed from their respective articles at the user's request. YouTube embeds remain intentional third-party dependencies.

## Next migration phases

1. Review and migrate selected older editorial content from the title-level inventory. Recover reliable publication dates before displaying them in the dated blog index, and avoid duplicate feed/pagination artifacts.
2. Resolve the one remaining document link that still points to a WordPress upload: the xtUML + UML-RT presentation PDF. That binary is not present in the archived GitHub capture and will need to be obtained from another source before it can be stored locally under `assets/documents/`. The Japanese Backslash Seminar presentation link now points to the public SlideShare copy. The Einstein's Riddle class diagram and all available illustrations for Union, Three Layers, and Semantic Steps are stored locally. Two original full-size image files linked from Three Layers and Semantic Steps were absent from the archive; the locally preserved article thumbnails are used instead. The Panda requirements PDF and self-driving-car paper references remain removed as requested.
3. Review external links, downloadable files, and obsolete calls to action.
4. Check all internal links, images, embeds, and generated URLs on the GitHub Pages preview.
5. Confirm current company contact details, team roster, and service offerings before custom-domain cutover.

## Explicitly deferred

- No changes to the WordPress production site.
- No changes to the existing `xtuml/onefactnet` archive.
- No custom-domain or DNS changes.
- No wholesale copying of WordPress, Elementor, HustleFish, or plugin-generated HTML/CSS/JavaScript.
