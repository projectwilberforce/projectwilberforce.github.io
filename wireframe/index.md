---
layout: wireframe
title: Wilberforce Wireframe Unity Plugin User Guide
---
# Contents
- [Introduction](#introduction)
- [Requirements](#requirements)
- [Installation](#installation)
- [Parameters](#parameters)
- [How to](#how-to)
- [Contact Information](#contact-information)

# Introduction

Wilberforce Wireframe (WW) is a Material Shader for Unity 5 (5.3.6 or higher)

You can buy Wilberforce Wireframe at [Unity Asset Store](https://www.assetstore.unity3d.com/#!/content/81663).

- Blending between wirecolor and fillcolor
- Supports Transparent Render Queue
- Option for removing diagonal edges
- Option for perspective display of lines (line appears thinner as distance from camera increases)
- Flat shading of the fill color

See [forum for discussion]() and contact us at <projectwilberforce@gmail.com> for additional support.
 
# Requirements

- Unity 5 (5.3.6 or higher; all editions including Personal)
- Shader Model 3.0:  
*NVIDIA cards since 2004 (GeForce 6)*  
*AMD cards since 2005 (Radeon X1300)*  
*Intel cards since 2006 (GMA X3000)* 
- Works on desktop platforms: DirectX 9.0c(TODO) and higher, OpenGL
- Windows, Mac, Linux

# Installation

1. Import from Asset Store.
2. Create new material (image)
3. Select created material
4. In inspector window set shader property to `Wilberforce/Wireframe` (image)
5. Apply material to mesh by drag&dropping to desired object or choosing it in the mesh inspector


# Parameters

WW material behaviour is controlled by following parameters:

(inspector image)

**Wire Thickness**
How thick the line appears.

**Wire Color**
Color of the line (can be transparent)

**Fill Color**
Color of the rest of the face (can be transparent)

**Remove Diagonals**
Skips certain triangle edges to create a quad wireframe

**Apply Flat Shading**
Faces are shaded

**Calculate in Object Space (Perspective)**
Perspective display - line appears thinner as distance from camera increases.

**Show Line Caps (beta)**
Switch on to display line caps (making the line thicker in the corners)

**Line Caps Size**
How thick the line caps are.

**Apply to faces**
`Front`: default option; `Back`: use to make a backface material for doublesided mesh.

# How to
## Transparency intermeshional
## Double-sided mesh

# Contact Information
In case of questions or further issues, please contact us at <projectwilberforce@gmail.com>

