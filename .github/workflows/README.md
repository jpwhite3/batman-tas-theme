# 🦇 Batman TAS Theme CI/CD Pipeline

This directory contains the complete CI/CD pipeline for the Batman TAS Theme VS Code extension, built with the precision and timeless quality of the 1990s animated series.

## 🚀 Workflows Overview

### 1. **Continuous Integration** (`ci.yml`)
**Triggers**: Push to `main`/`develop`, Pull Requests to `main`

**Jobs**:
- 🔧 **Build & Test**: Validates package structure and builds extension
- 🎨 **Validate Batman TAS Colors**: Ensures theme maintains authentic TAS aesthetic consistency
- ♿ **Accessibility Check**: Validates color blind friendly compliance

**Key Features**:
- Validates `package.json` and theme JSON structure
- Checks for required Batman TAS colors (Gotham Midnight, Joker Purple, TAS Danger Red, Robin Green, Batman Gray)
- Ensures high contrast text colors are maintained for authentic TAS experience
- Uploads build artifacts for 30 days
- Comprehensive error reporting with Batman TAS-themed messages

### 2. **Release Pipeline** (`release.yml`)
**Triggers**: Version tags (`v*`)

**Jobs**:
- 🎯 **Create Release**: Generates GitHub release with Batman TAS-themed description
- 🏗️ **Build & Publish**: Packages extension and uploads to release
- 📢 **Marketplace Publish**: Publishes to VS Code Marketplace (if `VSCE_PAT` secret exists)

**Key Features**:
- Automatic release creation with authentic TAS quotes and Dark Deco feature highlights
- Professional release notes with installation instructions
- Conditional marketplace publishing (only if secrets are configured)
- Automatic VSIX file attachment to releases

### 3. **PR Preview** (`pr-preview.yml`)
**Triggers**: Pull Request events (opened, synchronize, reopened)

**Jobs**:
- 🎨 **Generate PR Preview**: Creates preview build with PR-specific versioning
- 📊 **Theme Statistics**: Analyzes color usage and Batman TAS theme compliance
- 💬 **PR Comments**: Automatically comments with preview info and download links

**Key Features**:
- Preview builds with PR number and commit SHA in version
- Automated theme statistics (color counts, Batman TAS color usage)
- Interactive PR comments with installation instructions
- 7-day artifact retention for PR previews

## 🔧 Setup Instructions

### Prerequisites
1. **Node.js 18+** for build environment
2. **VSCE** (Visual Studio Code Extension manager)
3. **GitHub repository** with Actions enabled

### Required Secrets (Optional)
For marketplace publishing, add to repository secrets:
- `VSCE_PAT`: Personal Access Token from Azure DevOps for VS Code Marketplace

### File Structure
```
.github/
├── workflows/
│   ├── ci.yml                 # Continuous Integration
│   ├── release.yml           # Release Pipeline  
│   └── pr-preview.yml        # PR Preview Builds
├── ISSUE_TEMPLATE/
│   ├── bug_report.yml        # Bug Report Template
│   └── feature_request.yml   # Feature Request Template
├── pull_request_template.md  # PR Template
├── CONTRIBUTING.md           # Contribution Guidelines
└── dependabot.yml           # Dependency Updates
```

## 🎯 Quality Gates

### Build Requirements
- ✅ Valid `package.json` structure
- ✅ Valid theme JSON (parseable)
- ✅ Successful VSCE package creation
- ✅ No build errors or warnings

### Batman TAS Theme Compliance
- ✅ Gotham Midnight background (`#1a1a2e`)
- ✅ Joker Purple accent (`#805ad5`)
- ✅ TAS Danger Red (`#e53e3e`)
- ✅ Robin Green (`#38a169`)
- ✅ Batman Gray text (`#4a5568`)

### Accessibility Standards
- ✅ High contrast TAS text maintained (`#4a5568`, `#e2e8f0`)
- ✅ No problematic red-green combinations
- ✅ Color blind friendly Dark Deco design principles

## 🚀 Release Process

### Automated Release
```bash
# Update version in package.json
npm version patch|minor|major

# Create and push tag
git push origin v2.1.0
```

The release workflow will automatically:
1. Create GitHub release with Batman TAS professional description
2. Build and package extension
3. Upload `.vsix` file to release
4. Publish to VS Code Marketplace (if configured)

### Manual Release Steps
If needed, you can manually trigger releases:
```bash
# Build locally
npm run build

# Create release manually
gh release create v2.1.0 batman-tas-theme-2.1.0.vsix --title "🦇 Batman TAS Theme v2.1.0"
```

## 📊 Monitoring & Analytics

### GitHub Insights
- **Actions**: Monitor workflow success rates and timing
- **Releases**: Track download counts and user engagement
- **Issues**: Monitor bug reports and feature requests
- **Pull Requests**: Review contribution patterns

### Build Metrics
Each workflow provides:
- Build success/failure rates
- Batman TAS theme color statistics
- Accessibility compliance status
- Artifact generation and retention

## 🛠️ Troubleshooting

### Common Issues

**Build Fails**:
- Check `package.json` validity
- Ensure theme JSON is valid
- Verify VSCE can package successfully

**Color Validation Fails**:
- Ensure required Batman TAS colors are present
- Check color hex codes match exactly
- Verify theme maintains authentic TAS aesthetic

**Marketplace Publishing Fails**:
- Verify `VSCE_PAT` secret is set correctly
- Check Azure DevOps token permissions
- Ensure publisher name matches configuration

### Debug Commands
```bash
# Local validation
npm run validate

# Manual build
npm run build

# Check workflow logs
gh run list --workflow=ci.yml
```

## 🦇 Batman TAS Development Philosophy

The CI/CD pipeline embodies the timeless quality of Batman: The Animated Series:
- **Precision**: Every build validated with Dark Deco attention to detail
- **Timeless Quality**: Automated processes ensure consistent excellence
- **Authentic Standards**: Multiple quality gates maintain TAS aesthetic integrity
- **Accessibility**: Inclusive design principles from the legendary series
- **Professional Polish**: Secure processes worthy of Bruce Timm's vision

---

**"The night is darkest just before the dawn. And I promise you, the dawn is coming."** 🦇🌃

*The Batman TAS Theme CI/CD pipeline ensures that every release maintains the timeless standards of excellence that made the animated series legendary.*