# Overview

<iframe width="560" height="315" src="https://www.youtube.com/embed/OdqQR27XlQ8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

[Magenta Realtime 2 Plugin for UE](https://vrlab.akiya-souken.co.jp/products/magentart2plugin/) is a plugin that enables running [Magenta Realtime 2](https://magenta.withgoogle.com/mrt2)—a model capable of generating music interactively in real time and playing it like an instrument—within Unreal Engine.

!!! Info "What is Magenta Realtime 2?"

    - A real-time music generation model developed by Google that runs in a local environment.
    - Allows dynamically modifying and blending multiple prompts, as well as manipulating via MIDI input.

## Key features of this plugin

- Optimized for Windows + NVIDIA GPU
- Heavy AI processing runs on a dedicated thread to prevent blocking the Game Thread
- Implemented as a subsystem which can be called from anywhere in C++ and Blueprint (BP)
- Audio output is implemented as a MetaSound node, making it easy to connect with other MetaSound signal processing nodes

!!! Warning "Notes"

    - NVIDIA GPU (RTX 2000 series or later) is required.
    - Among Magenta Realtime 2 models, only the `Small` model is supported. The `Base` model is not supported and is not included in this plugin.
