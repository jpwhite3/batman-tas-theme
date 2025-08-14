# 🦇 Darkman Theme

[![CI Status](https://github.com/username/darkman/workflows/🦇%20Darkman%20Theme%20CI/badge.svg)](https://github.com/username/darkman/actions)
[![Release](https://github.com/username/darkman/workflows/🚀%20Release%20Darkman%20Theme/badge.svg)](https://github.com/username/darkman/releases)
[![Version](https://img.shields.io/github/v/release/username/darkman?label=version&color=1E3A8A)](https://github.com/username/darkman/releases)
[![License](https://img.shields.io/github/license/username/darkman?color=6366F1)](LICENSE)
[![Batman Approved](https://img.shields.io/badge/Batman-Approved-8B2635?logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZD0iTTEyIDJMMTMuMDkgOC4yNkwyMCA5TDEzLjA5IDE1Ljc0TDEyIDIyTDEwLjkxIDE1Ljc0TDQgOUwxMC45MSA4LjI2TDEyIDJaIiBmaWxsPSJ3aGl0ZSIvPgo8L3N2Zz4K)](https://github.com/username/darkman)

A professional VS Code color theme inspired by Batman and the Batcomputer aesthetic. This sophisticated dark theme features nearly black backgrounds with subtle blue hints, Batman-inspired navy blues and purples, material design elements, and strategic dark red accents. Experience coding like you're in the Batcave with subtle glow effects and premium polish that would make Batman himself envious.

## ✨ Features

- **🦇 Batcomputer Aesthetic**: Nearly black backgrounds with subtle blue hints for that high-tech Batcave feel
- **🎨 Material Design**: Unified panel appearance with barely visible super dark blue borders
- **♿ Color Blind Friendly**: Carefully crafted palette avoiding problematic red-green combinations
- **✨ Subtle Glow Effects**: Premium polish with non-distracting glow on interactive elements
- **🔥 Professional Polish**: Navy blue buttons with darker interaction feedback for Batman-level sophistication
- **🎯 Accessibility First**: WCAG compliant contrast ratios maintained throughout
- **🌃 Batman Color Palette**: Navy blues, deep purples, and strategic dark red "warning light" accents

## 🎨 Color Palette

### Primary Colors
- **Nearly Black Backgrounds**: `#050608`, `#060709`, `#0B0C0E` (with subtle blue hints)
- **Super Dark Blue Borders**: `#1A1C2A` (barely visible panel separation)
- **Main Text**: `#babed8` (excellent contrast and readability)
- **Muted Text**: `#4B526D` (secondary elements)

### Batman-Inspired Accents
- **Primary Accent**: `#6366F1` (indigo/dark blue-purple) - Links, highlights, selections
- **Secondary Purple**: `#8B5FBF` (deep purple) - Syntax highlighting, terminal cyan
- **Navy Buttons**: `#1E3A8A` with darker hover `#1E2951` (premium interaction feedback)

### Dark Red "Batcave Warning Lights"
- **Error States**: `#8B2635` (primary dark red for errors, modified files)
- **Terminal/Text Red**: `#B83A4A` (slightly brighter for visibility)
- **Subtle States**: `#5C1A20` (inactive/muted red elements)

### Syntax & Terminal
- **Blue**: `#82AAFF` (functions, keywords)  
- **Green**: `#C3E88D` (strings, success states)
- **Yellow**: `#FFCB6B` (constants, warnings, cursor)
- **Purple**: `#C792EA` (language keywords, special)

## 📦 Installation

### Method 1: Direct Installation (Recommended)

1. Download the latest `darkman-theme-1.0.0.vsix` file from releases
2. Open VS Code
3. Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac)
4. Type "Extensions: Install from VSIX"
5. Select the downloaded `.vsix` file
6. Go to **File → Preferences → Color Theme** (or `Ctrl+K Ctrl+T`)
7. Select **"Darkman Theme"**

### Method 2: Manual Development Installation

```bash
# Clone the repository
git clone <your-repo-url>
cd darkman

# Install VS Code Extension Manager (if not already installed)
npm install -g vsce

# Package the extension
vsce package

# Install the packaged extension
code --install-extension darkman-theme-1.0.0.vsix
```

### Method 3: Development Mode

1. Clone this repository to your VS Code extensions folder:
   - **Windows**: `%USERPROFILE%\.vscode\extensions\darkman-theme`
   - **macOS**: `~/.vscode/extensions/darkman-theme`
   - **Linux**: `~/.vscode/extensions/darkman-theme`
2. Restart VS Code or run "Developer: Reload Window"
3. Select the theme from **File → Preferences → Color Theme**

## 🛠️ Development

### Quick Start

```bash
# Clone and setup
git clone <repo-url>
cd darkman
npm install

# Build and test locally
npm run build
code --install-extension darkman-theme-1.0.0.vsix
```

### Development Workflow

```bash
# Validate theme JSON
npm run validate

# Build extension
npm run build

# Publish (requires VSCE_PAT)
npm run publish
```

### CI/CD Pipeline

The Darkman Theme uses a comprehensive GitHub Actions pipeline:

#### 🔄 **Continuous Integration**
- **Automated Building**: Every push builds and validates the extension
- **Batman Color Validation**: Ensures theme maintains Batman aesthetic
- **Accessibility Checks**: Validates color blind friendly compliance
- **Multi-language Testing**: Tests syntax highlighting across languages

#### 🚀 **Release Automation**
- **Version Tagging**: `git tag v1.1.0` triggers automatic release
- **GitHub Releases**: Auto-generated with changelog and download links  
- **Marketplace Publishing**: Automatic publishing to VS Code Marketplace
- **Artifact Management**: `.vsix` files uploaded to releases

#### 🎨 **PR Previews**
- **Preview Builds**: Each PR gets a testable preview extension
- **Theme Statistics**: Automated color analysis and metrics
- **Visual Testing**: PR comments with installation instructions

### Theme Development Guidelines

- **Edit**: `themes/darkman-color-theme.json` for color modifications
- **Test**: Install locally and test across multiple languages
- **Validate**: Maintain Batman aesthetic and accessibility standards
- **Document**: Follow design principles in `CLAUDE.md`
- **Contribute**: See `.github/CONTRIBUTING.md` for detailed guidelines

## 💻 Supported Languages

The Darkman Theme provides comprehensive syntax highlighting optimized for:

**Web Development:**
- JavaScript/TypeScript/JSX/TSX
- HTML/CSS/SCSS/LESS
- JSON/YAML/XML
- React/Vue/Angular

**Backend & Systems:**
- Python
- Go/Rust/C/C++
- Java/Kotlin
- C#/.NET
- PHP

**Other Languages:**
- Markdown
- Shell/Bash
- SQL
- Docker
- And 50+ more languages...

## 🎯 What Makes It Special

### Batcomputer Experience
- **Unified Interface**: All panels blend together like a single holographic display
- **Subtle Depth**: Barely visible borders create depth without distraction
- **Premium Interactions**: Button hovers darken instead of brighten (Batman-style)
- **Strategic Accents**: Dark red "warning lights" for errors and modifications

### Developer-Focused Features
- **Git Integration**: Clear visual indicators for file status with Batman colors
- **Error Highlighting**: Dark red error states that don't strain your eyes
- **Terminal Theming**: Complete ANSI color customization with Batman palette
- **Debug Interface**: Purple info states and yellow warnings maintain clarity

### Accessibility Excellence
- **Color Blind Safe**: No red-green color dependencies
- **High Contrast**: Meets WCAG guidelines for text readability
- **Low Eye Strain**: Nearly black backgrounds reduce fatigue during long sessions

## ⚙️ Customization

### Quick Customizations

Add these to your VS Code `settings.json` to customize the theme:

```json
{
  "workbench.colorCustomizations": {
    "[Darkman Theme]": {
      // Make backgrounds even darker
      "editor.background": "#000000",
      // Adjust accent colors  
      "focusBorder": "#1E3A8A80",
      // Customize terminal
      "terminal.background": "#050608"
    }
  },
  "editor.tokenColorCustomizations": {
    "[Darkman Theme]": {
      // Customize syntax colors
      "comments": "#757575",
      "strings": "#4CAF50"
    }
  }
}
```

### Font Recommendations

For the ultimate Batcomputer experience, try these fonts:

```json
{
  "editor.fontFamily": "'Cascadia Code PL', 'JetBrains Mono', 'Operator Mono'",
  "terminal.integrated.fontFamily": "'Cascadia Code PL', 'JetBrains Mono'"
}
```

## 🤝 Contributing

Help make the Darkman Theme even better! Contributions are always welcome.

### How to Contribute

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-improvement`)
3. **Make** your changes following the Batman aesthetic principles
4. **Test** your changes by packaging and installing locally
5. **Submit** a pull request with a clear description

### Contribution Guidelines

- Maintain the **Batman/Batcomputer aesthetic**
- Ensure **accessibility** (color blind friendly, high contrast)
- Keep **color consistency** with the existing palette
- Test across multiple **programming languages**
- Update documentation if needed

### Reporting Issues

Found a bug or have a suggestion? Please open an issue with:
- VS Code version
- Screenshots (if applicable)  
- Steps to reproduce
- Expected vs actual behavior

## 🔧 Advanced Configuration

### Complete Batcave Setup

For the full Batcomputer experience, combine with these settings:

```json
{
  // Theme
  "workbench.colorTheme": "Darkman Theme",
  "workbench.iconTheme": "material-icon-theme",
  
  // Batcomputer feel
  "editor.cursorBlinking": "smooth",
  "editor.cursorSmoothCaretAnimation": "on",
  "workbench.activityBar.location": "top",
  
  // Terminal
  "terminal.integrated.shellArgs.osx": ["-c", "echo '🦇 BATCOMPUTER ONLINE 🦇' && zsh"]
}
```

### Recommended Extensions

Enhance your Batcave coding experience:

- **Material Icon Theme** - Perfect icon complement
- **Bracket Pair Colorizer 2** - Color-coded brackets
- **GitLens** - Enhanced Git integration
- **Error Lens** - Inline error highlighting
- **Power Mode** - Particle effects for ultimate Batman flair

## 📄 License

This theme is released under the [MIT License](LICENSE).

## 🦇 The Batman Philosophy

> *"It's not who I am underneath, but what I do that defines me."* - Batman

The Darkman Theme embodies Batman's approach to excellence: meticulous attention to detail, unwavering commitment to the mission, and the understanding that the right tools make all the difference. Every color choice serves a purpose, every glow effect has meaning, and every interaction is crafted for peak performance.

This theme isn't just about looking good—it's about creating an environment where you can achieve your best work, night after night, with the focus and precision worthy of the Dark Knight himself.

---

**"I am vengeance, I am the night, I am... a developer with excellent taste in themes."** 🦇

*Happy coding, Gotham!*