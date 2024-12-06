---
layout: page
title: Dynamic Guitar Amp
description: Developing in a "smart" plugin with JUCE
img:
importance: 3
category: coursework
---

In a group of four, we created a guitar amp simulator plugin with multiple amp models. We utilized the SmartGuitarAmp project as a base for our ML-based tone models, and we created a cabinet simulator with an IR loader. We also created an effects chain that allowed for user presets.

# Individual Contribution
Although we worked as a team, I worked on the GUI, effects chain, and the system architecture.
I designed the GUI initially in Figma, then built the functional version using the JUCE visual library. The GUI was connected using JUCE's value state tree to control the preset, efffect, and model states.
On the effects chain, we used the JUCE built in effects packages, but I also developed a unique EQ effect.
Finally, I took a leadership role in developing the system architecture. Because we wanted a variable signal chain, we used a high level value state tree to maintain the parameters and modular instances of each item on the chain. This led to the use of a high level processing node with sub-nodes for the models and effects that are instantiated each time the chain is set.