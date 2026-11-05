---
title: "MC-Generated Auto-Dispose"
date: 2020-04-21
description: "How explicit xtUML associations can enable a model compiler to generate cascading instance cleanup."
permalink: /mc-generated-auto-dispose/
source_url: "https://xtuml.github.io/onefactnet/mc-generated-auto-dispose/"
---

In good object-oriented programming and modeling, instances of classes are linked through associations. This creates powerful interdependence among related classes, but makes cleanup more complex: an instance cannot simply delete itself without considering the other instances linked to it.

Because associations in xtUML are explicit and captured in model data, disposal can be automated. Some associations are unconditional; others are conditional. A model compiler can use this distinction during translation to generate appropriate cleanup behavior. One such model compiler supported a soil-sampling robotics application.

Consider a mission in which a zone is defined by one or more outer boundaries and zero or more inner boundaries (“holes”). A point is in the zone if it lies within any outer boundary and outside every inner boundary.

If a boundary used by a zone containing samples is deleted, deleting the last outer boundary cascades through the unconditional associations: the zone is disposed, followed by its sample zone, sample site, samples, soil cores, core point, and waypoint.

That is a substantial amount of cleanup work the modeler does not have to implement or manage manually.
