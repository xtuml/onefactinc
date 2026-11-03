# Older One Fact blog archive inventory

Source: `xtuml/onefactnet`, WordPress static capture. This document inventories the blog pagination pages after the ten entries in the captured RSS feed. The page numbers below are source archive pagination, not dates or a recommended migration order.

## Migration priorities

The first three selected articles have now been migrated to `_articles/` with their original publication dates and permalinks. Their content was recovered from the archived WordPress REST API export (`wp-json/wp/v2/posts/{id}`), which includes the original date and rendered post body.

- **Migrated:** [Dawn of Ciera](/dawn-of-ciera/) — February 1, 2020; production release announcement for the Ciera model compiler.
- **Migrated:** [OOA of MASL](/ooa-of-masl/) — January 16, 2020; comparison of the MASL and xtUML metamodels.
- **Migrated:** [Requirement Tracing](/requirement-tracing/) — November 21, 2019; approaches to tracing requirements through models and commits.

Remaining candidates for review:
- Do I need BridgePoint Pro? — explains the distinction between nightly builds and supported releases.
- xtUML in the Field — agricultural robotics, navigation, and model-based control.
- Java and BridgePoint — historical Java runtime configuration note; review for current relevance before publishing.
- AWS Lambda — cloud deployment / serverless topic; review current technical accuracy.
- Continuous Integration — engineering process topic.
- Model-Based Testing of Self-Driving Cars — model-based testing topic.
- Issue Tracking with Redmine — historical tooling note; review before migration.
- Action Language Fundamentals and Action Language — educational content.

## Archive index

The links below are titles discovered in the archived blog pagination. Some may be dated announcements, personal posts, or obsolete product notices; assess each before migration. The archive also contains duplicated or unusual pagination entries, so verify canonical content and paths.

### Page 2
- Dawn of Ciera
- OOA of MASL

### Page 3
- Do I need BridgePoint Pro?
- Requirement Tracing
- xtUML in the Field
- Java and BridgePoint
- Slackline? Slackline!
- x at the Eye

### Page 4
- Modeling Education
- MDD at Shinshu U
- MODELS
- xtUML Days 2019 UK Presentations
- xtUML Days 2019 In Motion
- xtUML Days next week

### Page 5
- Shlaer-Mellor Runtime
- Keynote Speaker
- Find a Bug; Fix a Bug
- xtUML Days 2019 UK
- AUTOSAR
- Saab Coming to West Lafayette

### Page 6
- State Diagram, State Table
- Model Compiler Builders
- Continuous Integration
- Sorting Mail
- We Like AsciiDoc
- One Fact in Wood

### Page 7
- Winter Computer Science Intern
- Amazon Web Services (AWS) Lambda
- BridgePoint Pro v6.16
- 1,3,5+ Application, Dialects, Architectures
- Papyrus Industry Consortium 2019
- xtUML in Portsmouth UK

### Page 8
- Big Machine Big Model
- Sunrise on MODELS
- xtUML at Shinshu 2018
- Debugging Sumo
- C Model Compiler Summer
- Shinshu Class

### Page 9
- Super/Sub
- Eclipse Oxygen
- LEGO in Research
- Easy Chair
- State Save
- xtUML Days 2018 at MODELS

### Page 10
- BeagleBone Black
- Simulated Time
- Chief Software Architect
- Einstein's Riddle Solved
- Einstein's Riddle
- Symmetric Difference

### Page 11
- Difference
- Intersection
- Union
- New Model
- Community Chat
- MT-CPS 18

### Page 12
- xtUML Day 2017 Linköping Presentations
- Doodling
- Cairo to Indiana
- MODELS 2017 EXE and MDETools
- Eclipse Mania
- Model-Based Testing of Self-Driving Cars

### Page 13
- One Fact Etch
- Academy of Global Engineering
- Backslash Seminar Japan
- Gripen E
- Initial State
- xtUML Day 2017 UK

### Page 14
- Jenkins
- Purdue Sunset
- Lafayette Business Expo
- Changing Lanes
- IEEE HKN SLC 2017
- xtUML Resources

### Page 15
- 1F on the Road
- Collapsed Referential
- Modeling Before Programming
- Model API?
- Senior Project
- Eclipse Governance

### Page 16
- Always Advancing: xtUML release 5.3.4
- xtUML.jp
- EclipseCON North America 2016
- Issue Tracking with Redmine
- Action Language Fundamentals
- Action Language

### Page 17
- PIC Members
- xtUML Interfaces
- 2 Views
- Happy New Year 2016
- xtUML 2015 Is History
- Ready for xtUML 2015!

### Page 18
- Good Language
- Escher
- Applications then Models then Tools
- Conference and Attendee
- Announcing xtUML 2015
- Experiment

### Page 19
- UML-RT + xtUML
- Models 2015
- Autosampler
- football (futbol, soccer)
- Stevenson Screen (Weather Station)
- xtUML + UML-RT

### Page 20
- Semantic Steps
- Three Layers
- Incremental, Always Advancing
- Model Translation FAQs
- BridgePoint is moving to Eclipse 4.4 (Luna)
- Let's Chat! Meet the One Fact CEO

### Page 21
- Memorial Day
- Future of Executable UML
- Revision Control
- ISO26262Day
- Qt and Squish and xtUML Together
- State of the One Fact Union

### Page 22
- Collaborative Development using eGit
- Dream
- Modeling Domain Specific Languages
- Returning Strings in C
- Old Testament
- Happy New Year 2015

### Page 23
- Electric Parking Brake Model Snippet
- Getting Started with GitHub
- Blood Pressure Cuff
- Where Does the Name One Fact Come From?
- xtUML on MOdeling LAnguages
- Open Source BridgePoint

## Review notes

- The source archive's pagination contains WordPress-generated query-string links as well as canonical folder-style article paths. Use the canonical article folder when present; do not create new pages from query-string export artifacts.
- Several entries are event announcements, product release notices, personal posts, or old tool instructions. Preserve their historical context and do not silently present old instructions as current guidance.
- Publication dates for the first three migrated articles were verified using the archived WordPress REST API JSON records. Dates for the remaining older set have not yet been verified; do not infer them from pagination order or WordPress post IDs. Verify dates from a reliable source before adding those articles to the dated blog index.
- This is a title-level inventory, not yet a content-completeness audit. Each selected article still needs a review of body text, images, downloads, external links, and original permalink.
