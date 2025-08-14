# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository contains "Darkman Theme" - a professional VS Code color theme extension inspired by Batman and the Batcomputer aesthetic. The theme features a sophisticated dark color palette with material design elements, color blind friendly colors, subtle glow effects, and Batman-inspired navy blues, purples, and dark red accents.

## Repository Structure

- `package.json` - VS Code extension manifest with theme metadata and configuration
- `themes/darkman-color-theme.json` - Main color theme definition file with comprehensive UI and syntax coloring
- `vscode_settings.json` - Reference VS Code settings (for development reference only)
- `color-pallete.jpg` - Color palette inspiration image used for theme development
- `buttons.jpg` - Button design reference image for interaction elements
- `icon.svg` - Extension icon
- `LICENSE` - MIT license file
- `README.md` - Extension documentation
- `CHANGELOG.md` - Version history and changes
- `.claude/settings.local.json` - Claude Code permissions configuration

## Theme Architecture

### Color Philosophy
The Darkman Theme follows a "Batcomputer" aesthetic with:
- **Nearly black backgrounds** with subtle blue hints for that high-tech feel
- **Professional material design** with unified panel appearance
- **Color blind friendly** palette avoiding problematic red-green combinations
- **Subtle glow effects** on interactive elements for premium polish
- **Batman-inspired colors** using navy blues, deep purples, and strategic dark reds

### Panel Unification
- All panels use consistent background colors (`#050608` to `#0B0C0E` range)
- Super dark blue borders (`#1A1C2A`) create subtle separation without harsh lines
- Darker interaction feedback instead of lighter (Batman-like pressed effects)

## Key Color Palette

### Primary Colors
- **Primary backgrounds**: `#050608`, `#060709`, `#0B0C0E` (nearly black with subtle blue hints)
- **Panel borders**: `#1A1C2A` (super dark blue)
- **Main text**: `#babed8` (maintained from original for excellent contrast)
- **Muted text**: `#4B526D` (secondary text elements)

### Accent Colors (Batman Palette)
- **Primary accent**: `#6366F1` (indigo/dark blue-purple) - replaced teal throughout
- **Secondary purple**: `#8B5FBF` (deep purple) - for syntax highlighting and UI elements
- **Navy buttons**: `#1E3A8A` with darker hover `#1E2951`

### Dark Red Accents (Batcave Warning Lights)
- **Primary dark red**: `#8B2635` - for error states, modified file indicators
- **Secondary red**: `#B83A4A` - for terminal colors and text elements
- **Inactive red**: `#5C1A20` - for subtle states

### Terminal & Syntax Colors
- Maintains color blind friendly ANSI colors
- Batman color palette integration in syntax highlighting
- Dark red errors, purple info, yellow warnings

## Working with This Repository

### Extension Development
1. **Theme Modifications**: Edit `themes/darkman-color-theme.json` for color changes
2. **Testing**: Use `vsce package` to build the extension
3. **Installation**: Install the generated `.vsix` file in VS Code
4. **Color Consistency**: Maintain the Batman aesthetic and accessibility standards

### Key Design Principles
- **Accessibility First**: Maintain contrast ratios and color blind friendly design
- **Batman Aesthetic**: Dark, professional, with strategic accent colors
- **Material Design**: Unified panels with subtle borders and depth
- **Subtle Effects**: Glow effects enhance without distraction
- **Professional Polish**: Every element should feel premium and sophisticated

## Theme Features

### Visual Enhancements
- Subtle glow effects on focus states and interactive elements
- Enhanced button styling with navy blues and darker interaction feedback
- Unified panel appearance with barely visible borders
- Material design elevation system
- Batman-inspired error and warning states

### Accessibility
- Color blind friendly color combinations
- High contrast text and UI elements
- No problematic red-green color dependencies
- WCAG compliant contrast ratios maintained

### Developer Experience
- Comprehensive syntax highlighting for all major languages
- Git integration with appropriate status colors
- Terminal customization with Batman color palette
- Debug and error states with clear visual hierarchy

## Configuration Management

The repository includes:
- Claude Code permissions in `.claude/settings.local.json`
- Extension packaging configuration in `package.json`
- Complete theme definitions with Batman-inspired naming and descriptions

## Extension Installation & Usage

The theme is packaged as a VS Code extension (`darkman-theme-1.0.0.vsix`) and can be installed directly in VS Code. Once installed, select "Darkman Theme" from the color theme picker for the complete Batcomputer coding experience.