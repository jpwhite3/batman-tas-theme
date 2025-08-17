# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository contains "Batman TAS Theme" - a professional VS Code color theme extension inspired by Batman: The Animated Series from the 1990s. The theme features an authentic Dark Deco color palette extracted from the original animated series, with sophisticated dark backgrounds, material design elements, color blind friendly colors, and Batman TAS-inspired navy blues, purples, and classic animation accents.

## Repository Structure

- `package.json` - VS Code extension manifest with theme metadata and configuration
- `themes/batman-tas-color-theme.json` - Main color theme definition file with comprehensive UI and syntax coloring
- `vscode_settings.json` - Reference VS Code settings (for development reference only)
- `batmanbngvar.png` - Batman TAS color palette inspiration image from the 1990s animated series
- `buttons.jpg` - Button design reference image for interaction elements
- `icon.svg` - Extension icon
- `LICENSE` - MIT license file
- `README.md` - Extension documentation with full color palette and installation guide
- `CHANGELOG.md` - Version history and changes
- `.claude/settings.local.json` - Claude Code permissions configuration

## Theme Architecture

### Color Philosophy
The Batman TAS Theme follows the authentic "Dark Deco" aesthetic from the 1990s animated series with:
- **Gotham midnight backgrounds** with deep navy blues reminiscent of the animated series
- **Professional art deco design** with unified panel appearance inspired by Bruce Timm's vision
- **Color blind friendly** palette avoiding problematic red-green combinations
- **Classic animation contrast** on interactive elements for authentic TAS feel
- **Batman TAS-inspired colors** using authentic navy blues, deep purples, and strategic animation reds

### Panel Unification
- All panels use consistent background colors (`#1a1a2e` to `#16213e` range) sampled from TAS artwork
- Deep navy borders (`#1e3a5f`) create subtle separation with authentic animation styling
- Darker interaction feedback instead of lighter (true to the Dark Knight aesthetic)

## Key Color Palette

### Primary Colors (Gotham Nights)
- **Gotham Midnight**: `#1a1a2e` (primary editor background from TAS night scenes)
- **Deep Navy Shadow**: `#16213e` (panel backgrounds, sidebars)
- **Batman's Cape**: `#0f3460` (darker accent backgrounds)
- **Twilight Blue**: `#1e3a5f` (border colors, dividers)

### Text Colors (The Dark Knight)
- **Batman Gray**: `#4a5568` (primary text, main content)
- **Cowl Shadow**: `#2d3748` (secondary text, comments)
- **Gotham Fog**: `#e2e8f0` (bright text, keywords)
- **Silver Highlight**: `#cbd5e0` (active selections, highlights)

### Accent Colors (Gotham Signals)
- **Danger Red**: `#e53e3e` (errors, warnings, git deletions from TAS danger scenes)
- **Alert Crimson**: `#c53030` (error highlights, urgent states)
- **Street Light Yellow**: `#ecc94b` (warnings, modified files from Gotham street scenes)
- **Golden Beacon**: `#d69e2e` (constants, numbers, search highlights)

### Success States (Robin's Colors)
- **Emerald Success**: `#38a169` (strings, success states, git additions)
- **Forest Green**: `#2f855a` (darker success states, terminal green)

### Special Elements (Villain Accents)
- **Joker Purple**: `#805ad5` (keywords, special syntax from TAS villain scenes)
- **Royal Villain**: `#6b46c1` (functions, methods, links)

### Terminal & Syntax Colors
- Maintains color blind friendly ANSI colors with TAS palette integration
- Batman TAS color palette integration in syntax highlighting
- Classic animation red errors, purple info, golden yellow warnings

## Working with This Repository

### Extension Development
1. **Theme Modifications**: Edit `themes/batman-tas-color-theme.json` for color changes
2. **Testing**: Use `vsce package` to build the extension
3. **Installation**: Install the generated `.vsix` file in VS Code
4. **Color Consistency**: Maintain the Batman TAS aesthetic and accessibility standards

### Key Design Principles
- **Accessibility First**: Maintain contrast ratios and color blind friendly design
- **Batman TAS Aesthetic**: Authentic 1990s Dark Deco styling with strategic accent colors
- **Art Deco Design**: Unified panels with subtle borders and sophisticated depth
- **Classic Animation Effects**: Subtle highlights that enhance without distraction
- **Professional Polish**: Every element should feel premium and timeless

## Theme Features

### Visual Enhancements
- Classic animation-style highlights on focus states and interactive elements
- Enhanced button styling with TAS navy blues and darker interaction feedback
- Unified panel appearance with barely visible borders inspired by Batcomputer design
- Art deco elevation system from the animated series
- Batman TAS-inspired error and warning states using authentic animation colors

### Accessibility
- Color blind friendly color combinations tested across the spectrum
- High contrast text and UI elements meeting WCAG standards
- No problematic red-green color dependencies
- WCAG compliant contrast ratios maintained throughout

### Developer Experience
- Comprehensive syntax highlighting for all major languages using TAS palette
- Git integration with appropriate status colors from the animated series
- Terminal customization with Batman TAS color palette
- Debug and error states with clear visual hierarchy using animation-inspired colors

## Configuration Management

The repository includes:
- Claude Code permissions in `.claude/settings.local.json`
- Extension packaging configuration in `package.json`
- Complete theme definitions with Batman TAS-inspired naming and descriptions
- Color palette documentation referencing the 1990s animated series

## Extension Installation & Usage

The theme is packaged as a VS Code extension (`batman-tas-theme-2.0.0.vsix`) and can be installed directly in VS Code. Once installed, select "Batman TAS Theme" from the color theme picker for the complete Gotham City coding experience inspired by the legendary animated series.

## Batman TAS Color Reference

All colors in this theme are sampled from or inspired by the original Batman: The Animated Series artwork, particularly the iconic "Dark Deco" style that used black paper with painted highlights. This creates the sophisticated, noir atmosphere that made the show legendary and brings that same timeless quality to your coding environment.