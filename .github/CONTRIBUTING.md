# 🦇 Contributing to Darkman Theme

Thank you for your interest in contributing to the Darkman Theme! This guide will help you get started with our Batman-worthy development process.

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ 
- VS Code
- Git

### Development Setup
```bash
# Clone the repository
git clone <your-fork-url>
cd darkman

# Install dependencies
npm install

# Build the extension
npm run build

# Install locally for testing
code --install-extension darkman-theme-1.0.0.vsix
```

## 🦇 Development Guidelines

### Batman Aesthetic Principles
- **Nearly Black Backgrounds**: Use `#050608` to `#0B0C0E` range
- **Super Dark Blue Borders**: `#1A1C2A` for subtle panel separation
- **Navy Button Colors**: `#1E3A8A` with darker hover states
- **Batman Accents**: `#6366F1` (indigo) for highlights and selections
- **Joker Green**: `#7A8650`, `#9FB36B` for success/growth states
- **Villain Purple**: `#4A3666` for debug/special states
- **Dark Red**: `#8B2635`, `#B83A4A` for errors/warnings

### Accessibility Requirements
- ✅ Maintain WCAG AA contrast ratios (4.5:1 for normal text)
- ✅ Avoid red-green only color coding
- ✅ Test with color blind simulators
- ✅ Ensure high contrast for all text elements

### Code Style
- Use meaningful color names in comments
- Group related colors together
- Maintain consistent opacity levels (20, 35, 50, 80 etc.)
- Test across multiple programming languages

## 🔄 CI/CD Pipeline

### Automated Workflows

#### 1. **Continuous Integration** (`.github/workflows/ci.yml`)
Runs on every push and pull request:
- 🔧 **Build & Test**: Validates package structure and builds extension
- 🎨 **Color Validation**: Ensures Batman color consistency
- ♿ **Accessibility Check**: Validates color blind friendly compliance

#### 2. **Release Pipeline** (`.github/workflows/release.yml`)
Runs on version tags (`v*`):
- 🎯 **Create Release**: Generates GitHub release with changelog
- 🏗️ **Build & Upload**: Packages extension and uploads to release
- 📢 **Marketplace Publish**: Publishes to VS Code Marketplace (if configured)

#### 3. **PR Preview** (`.github/workflows/pr-preview.yml`)
Runs on pull requests:
- 🎨 **Preview Build**: Creates PR-specific extension build
- 📊 **Theme Statistics**: Analyzes color usage and theme metrics
- 💬 **PR Comments**: Posts preview info and download links

### Setting Up Marketplace Publishing

To enable automatic publishing to VS Code Marketplace:

1. **Create Azure DevOps Account**: Go to [dev.azure.com](https://dev.azure.com)
2. **Generate Personal Access Token**:
   - Navigate to User Settings → Personal Access Tokens
   - Create token with "Marketplace" scope
3. **Add Repository Secret**:
   - Go to repository Settings → Secrets and variables → Actions
   - Add secret named `VSCE_PAT` with your token

## 🧪 Testing

### Local Testing
```bash
# Validate theme JSON
npm run validate

# Build extension
npm run build

# Install and test locally
code --install-extension darkman-theme-1.0.0.vsix
```

### Test Checklist
- [ ] Theme builds without errors
- [ ] All major programming languages display correctly
- [ ] UI elements maintain Batman aesthetic
- [ ] No accessibility regressions
- [ ] Git decorations work properly
- [ ] Terminal colors are appropriate

### Browser Testing Matrix
Test your changes with:
- **Languages**: JavaScript, Python, HTML, CSS, JSON, Markdown, Go, Rust
- **VS Code Versions**: Latest stable, previous major version
- **Operating Systems**: Windows, macOS, Linux
- **Color Blind Testing**: Use browser extensions to simulate different types

## 📝 Pull Request Process

### Before Submitting
1. **Run CI locally**: `npm run validate && npm run build`
2. **Test thoroughly**: Install and use the theme for actual development
3. **Check accessibility**: Verify contrast ratios and color blind compliance
4. **Update documentation**: Add any necessary documentation changes

### PR Requirements
- ✅ Clear description of changes
- ✅ Screenshots for visual changes
- ✅ All CI checks passing
- ✅ Batman aesthetic compliance confirmed
- ✅ Accessibility requirements met

### Review Process
1. **Automated CI**: All workflows must pass
2. **Visual Review**: Maintainers will test the theme visually
3. **Batman Aesthetic Check**: Ensures changes align with theme philosophy
4. **Accessibility Review**: Validates inclusive design principles

## 🏷️ Release Process

### Version Tagging
```bash
# Update version in package.json
# Commit changes
git add .
git commit -m "🦇 Release v1.1.0"

# Create and push tag
git tag v1.1.0
git push origin v1.1.0
```

### Automatic Release
The release workflow will:
1. Create GitHub release with changelog
2. Build and upload `.vsix` file
3. Publish to VS Code Marketplace (if configured)

## 🐛 Issue Guidelines

### Bug Reports
- Use the bug report template
- Include VS Code version, theme version, and OS
- Provide screenshots when applicable
- List steps to reproduce

### Feature Requests  
- Use the feature request template
- Explain the Batman theme connection
- Describe the problem and proposed solution
- Consider accessibility implications

## 🦇 Community

### Code of Conduct
- Be respectful and inclusive
- Focus on constructive feedback
- Help maintain the Batman theme's sophisticated aesthetic
- Prioritize accessibility and user experience

### Getting Help
- Check existing issues and discussions
- Join community discussions
- Ask questions in pull requests
- Review the documentation

---

## 🌟 Recognition

Contributors who help improve the Darkman Theme will be recognized in:
- Release notes
- Contributors section
- Special Batman-themed acknowledgments

Remember: *"It's not who I am underneath, but what I do that defines me."* - Batman

Every contribution, no matter how small, helps make the Darkman Theme better for developers around the world! 🦇

---

**Happy coding, Gotham!** 🌃