---
title: "xtUML in the Field"
date: 2019-11-11
description: "A case study of xtUML in an agricultural soil-sampling robot, including navigation, guidance, and model-based control."
permalink: /xtuml-in-the-field/
source_url: "https://xtuml.github.io/onefactnet/xtuml-in-the-field/"
thumbnail: "/assets/images/image-1024x577-6913326.png"
---

[ROGO Ag](https://www.rogoag.com/) developed automated soil-sampling systems for agriculture. Its application-specific robot gathers soil samples quickly and precisely according to predefined criteria, improving data quality, repeatability, and efficiency compared with manual sampling.

A [video of the robot in action](https://youtu.be/CbQcSAcrw88) accompanied the original article.

xtUML was used in the enhanced GPS navigation, inertial guidance, and robotic control sequencing. The original post showed models for the mission and navigation subsystems, as well as a model-based model compiler that generated ROS-aware Python and provided a Shlaer-Mellor-compliant software architecture.

![xtUML design model]({{ '/assets/images/image-1024x577-6913326.png' | relative_url }})

*Design model.*

![Mission subsystem model]({{ '/assets/images/image-1-1024x577-9950624.png' | relative_url }})

*Mission subsystem.*

![Navigation subsystem model]({{ '/assets/images/image-2-1024x578-1908639.png' | relative_url }})

*Navigation subsystem.*

![Model compiler for ROS-aware Python]({{ '/assets/images/image-3-1024x576-4395604.png' | relative_url }})

*Model compiler (MC-ROS).*

The original presentation is available from the [xtUML website](https://xtuml.org/xtumlinthefield/).

*Historical note: this case study was published in November 2019. Company offerings and project details may have changed since publication.*
