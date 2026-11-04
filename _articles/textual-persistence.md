---
title: "Textual Persistence"
date: 2021-12-28
description: "A proposal for textual semantic xtUML notation, model persistence, and exchange."
permalink: /textual-persistence/
source_url: "https://xtuml.github.io/onefactnet/textual-persistence/"
---

Dear Modelers,

Significant progress has been made on specifications for textual xtUML and, separately, graphics. This note concerns the specification of textual semantic xtUML. The specification serves several purposes:

1. It specifies a full textual notation for structural Shlaer-Mellor.
2. It specifies how models will be persisted under BridgePoint, supplanting the OOA of OOA instance strategy then employed.
3. It defines a textual exchange mechanism.
4. It loosens the coupling between the Method and tooling, opening options for editors, interpreters, and translators.
5. It opens dialogue about additions, deletions, and convergence in Method and tooling features.

The original note invited review of the specification, especially on containment, element identification, scoping and visibility, the type system, state-machine semantics, package inclusion, exclusion of non-executable elements, and action-language agnosticism.

### What textual persistence enables

- More tractable diff and merge.
- Editing models outside BridgePoint and synchronizing them.
- Simultaneous graphical and textual editing.
- Editors, interpreters, and model compilers operating directly on text.
- Different diagram editors and renderers connected to shared semantics.
- Reasoning about model semantics in unambiguous text as well as diagrams.

See the [textual xtUML specification](https://github.com/xtuml/bridgepoint/blob/master/doc-bridgepoint/notes/12330_textual_xtuml/12330_textual_xtuml.adoc) and its [GPS Watch example model](https://github.com/xtuml/bridgepoint/tree/master/doc-bridgepoint/notes/12330_textual_xtuml/example).


