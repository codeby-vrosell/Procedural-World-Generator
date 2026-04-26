<p align="center">
  <img src="IMG/banner.png" alt="Procedural Generator Banner" />
</p>

# PROCEDURAL WORLD GENERATOR

## Project Overview

This repository serves as a showcase for the **Procedural Generator**. This world generator is an integral part of **Project IV**, a tactical roguelike currently in active development. 

While the main system resides in Project IV, this repository provides a **real-time standalone application** of the generator. It allows for the isolated and optimized visualization and dynamic adjustment of biomes, entities, and terrain parameters.

## Scope & Limitations

While the application allows for the deep customization of a vast array of generation parameters in real-time, it is important to note that it remains fundamentally tied to the external project it was built for. 

Because it inherits **Project IV's** unique rules—such as being strictly grid-based and featuring exactly 5 specific biomes **the app does not allow for adding or fundamentally altering the base types of biomes, enemies, entities, or generated objects.** The tool is designed to tweak and visualize *how* these predefined elements are generated and distributed, rather than creating entirely new ones from scratch.

## ⚠️ Important Disclaimer: No Source Code Included

Because **Project IV is currently in active development with a potential future commercial release on Steam**, the source code must remain confidential. 

Therefore, this repository does **NOT** contain any scripts, assets, 3D models, prefabs, UI graphics, or Unity project files. It is strictly dedicated to hosting the **standalone executable build** so users can interact with, visualize, and test the procedural generation logic in real-time.

## System Architecture (Under the Hood)

Although the scripts are not public, the generator is powered by several custom core modules designed by the author:

- **Biome Generator:** The core procedural engine. Handles Perlin noise evaluation, chunk-based seed management, world warping, and the distribution logic for water, obstacles, enemies, and entities.
- **Grid Manager:** Manages the physical grid instantiation. Handles multi-tile object placement, rotation constraints, cell reservation, coordinate mapping, and tracks generation statistics.
- **Camera Control:** Provides an RTS-style camera system. Features zoom and panning mechanics, dynamic boundaries based on the zoom level, and custom cursor management.
- **UI Controller:** The bridge between the user and the procedural engine. Controls real-time UI binding, auto-generation toggles, statistics tables, hover legends, and UI visual transitions.

## How to Use the App

1. Download the standalone build from the **Download & Try** section below.  
2. Extract the downloaded `.zip` file to your preferred location on your computer.
3. Run the executable file (`.exe`) to launch the generator.  
4. Use the in-app UI panels to configure generation settings (noise frequencies, biome sizes, spawn weights) and watch the map update in real-time.
5. Use the mouse to pan the camera and the scroll wheel to zoom in and out of the generated map.

## Technical Highlights

- The systems have been designed with heavy performance optimization in mind, utilizing Unity coroutines for grid building and cache dictionaries for noise evaluation to ensure smooth real-time generation.
- The RTS camera system is built on top of `Unity.Cinemachine` for smooth, bounded navigation.
  
## Watch Procedural Generator

The following screenshots display the procedural generator in action:

<p align="center">
  <img src="IMG/IMG1.png" alt="Generator Screenshot 1" width="30%"/>
  <img src="IMG/IMG2.png" alt="Generator Screenshot 2" width="30%"/>
  <img src="IMG/IMG3.png" alt="Generator Screenshot 3" width="30%"/>
</p>

<p align="center">
  <img src="GIF/GIF1.gif.gif" alt="Demostración del Generador" width="50%" />
  <img src="GIF/GIF1.gif.gif" alt="Demostración del Generador" width="50%" />
</p>

You can watch the tool in action here:

- **Youtube:** [Procedural Generator Showcase] (Available soon)

## Download & Try

You can try the tool directly on your computer by downloading the standalone executable build:

- **Download Release:** [Download Procedural Generator App](https://drive.google.com/uc?export=download&id=1dmT8t50I6hGURDfnvUjexHOfPjOejIZM)

*(Note: Extract the downloaded `.zip` file and run the `.exe` to launch the generator).*

## Author & Contact

**Author:** Víctor Rosell Gascó

- **Gmail:** codeby.vrosell@gmail.com  
- **Portfolio:** [codebyvrosell.com](https://codebyvrosell.com)   
- **Twitter:** [@codeby_vrosell](https://x.com/codeby_vrosell)  
- **GitHub:** [@codeby-vrosell](https://github.com/codeby-vrosell)  
- **LinkedIn:** [in/v-rosell](https://linkedin.com/in/v-rosell)

## License

This repository and its contents are provided under a strict private license.                                    
**Its use, copying, modification, reverse engineering, or distribution is not allowed** under any circumstances without explicit written permission from the author.

All rights reserved.
