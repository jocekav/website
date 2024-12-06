---
layout: page
title: turn-taking
description: turn-taking
img: 
importance: 1
category: work
related_publications: false
---

Turn-taking is an important part of improvisational, collaborative music, and it can be likened to human conversation. However, in the robotic musicianship space, turn-taking is typically fixed to straight-ahead schemes. My research aims to develop a new musical turn-taking model based on conversational analysis and observations of free improvisation and jam bands.

# Studying Improvisation
Before development, I studied group improvisation by annotating live performance videos, conducting ethnomusilogical interviews, and reading jazz literature.
I developed an initial turn-taking taxonomy to annotate videos of improvisers and jam bands. The videos were validated for improvisation using their title and comments, and they covered the genres of free jazz, straight ahead jazz, rock, soul, and free improvisation. Annotate.TV was used to facilitate the annotations, and the annotations were marked at turn transition points. Additionally, annotations included notes on specific physical gestures related to turn transitions.
I interviewed members of the Atlanta Improvisor Orchestra on their perspectives on improvisation. Interviews focused on the musical features performers listen for when improvising in a group, how individuals construct musical phrases, and how physical gestures impact performance.

# The System
I developed a new model for dynamic leader-follower turn-taking, using the insights gained from the annotations, interviews, and reading improvisation journals. The musician interacts with Shimon, a robotic marimba player, via MIDI keyboard. The system was built with Python and Max/MSP.
The system is a state machine with 2 states: leader and follower. In the leader state, Shimon improvises and introduces new themes and ideas. In the follower state, Shimon primarily listens and echoes the user's phrases. The state transitions are determined by varying probabilities set by the length of time in a state and features of the user input including similarity, dynamics, note density, and key.
I also developed a genetic algorithm for the musical output during each state. The algorithm uses jazz solos and licks as the initial population and a weighted aggregate function based on similarity for the fitness function.
Finally, I created physical gestures for Shimon. The turn-taking interaction is led by Shimon's gestures. Each state has its own gestures that are based on observations from the video annotations.
