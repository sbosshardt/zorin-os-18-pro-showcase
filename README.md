# Zorin OS 18 Pro Software Showcase

A web-based gallery showcasing the software applications that come preinstalled with Zorin OS 18 Pro (but not with Zorin OS 18 Core).

**⚠️ DISCLAIMER:**
This is an unofficial project with no affiliation or relationship with Zorin Ltd., the Zorin OS development team, or any of the showcased software projects. This showcase was created independently for informational purposes only. See also the **Image Usage Notice** at the bottom of this page.

## Overview

This is an interactive showcase webpage that displays 42 software applications organized into five categories:
- **Creative & Design** (10 apps): GIMP, Blender, Darktable, Krita, Inkscape, LibreCAD, Shotwell, Scribus, OpenToonz, FreeCAD
- **Video & Audio** (10 apps): OBS Studio, Kdenlive, HandBrake, Audacity, Ardour, Mixxx, Easy Effects, VLC, Clapper, Valot
- **Productivity** (9 apps): Logseq, Foliate, Minder, Xournal++, Homebank, Planify, NewsFlash, Apostrophe, Deskflow
- **Other Tools** (8 apps): Warp, Gradia, EyeDropper, Blanket, Fragments, Upscaler, Drum Machine, Solanum, Network Displays
- **System Tools** (2 apps): GNOME Maps, Graphviz

## Features

- **Expandable Cards**: Each application is displayed as a card that can be expanded to show detailed information
- **Application Details**: When expanded, each card shows:
  - Application title and tagline
  - Logo/thumbnail image
  - Description paragraph
  - Screenshots (when available)
  - Link to project homepage
  - Copy-pasteable install command
- **Local Assets**: Logos and screenshots are stored locally in `logos/` and `screenshots/` subdirectories
- **Responsive Design**: The webpage adapts to different screen sizes
- **Category Filtering**: Users can filter applications by category

## File Structure

```
zorin-os-18-pro-showcase/
├── index.html          # Main webpage file
├── logos/              # Application logos (PNG/SVG files)
├── screenshots/        # Application screenshots (PNG/JPG files)
├── README.md           # This file
└── notes.txt           # Development notes and summary
```

## Usage

Simply open `index.html` in a web browser. No server or build process required - it's a standalone HTML file with embedded CSS and JavaScript.

## Installation Commands

The webpage displays installation commands for each application. Most use either:
- `sudo apt install <package>` for Debian/Ubuntu packages
- `flatpak install flathub <app-id>` for Flatpak applications

## Current Status

- ✅ All 42 applications have logos (stored locally in `logos/`)
- ✅ All applications have descriptions
- ⚠️ Screenshots: Only Blender has a working screenshot currently (147KB JPEG)
- ⚠️ Many screenshot URLs are outdated or return HTML error pages

## Screenshots

To add screenshots for applications:
1. Download screenshot images to the `screenshots/` directory
2. Name them following the pattern: `<app-name>-1.png` (or `.jpg`)
3. Update the `screenshots` array in `index.html` for the corresponding application
4. Example: `screenshots: ["screenshots/blender-1.jpg"]`

## Source

This showcase was created based on package list comparisons between Zorin OS 18 Core and Zorin OS 18 Pro installations.

## Image Usage Notice
Image files (logos and screenshots) were collected from the web and their inclusion here is believed to be fair use. This project does not grant any licenses or permissions for the use of these images. Users should obtain proper licensing directly from the respective copyright holders if they wish to use these images for any purpose.
