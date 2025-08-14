# 🦇 Darkman Theme CI/CD Pipeline

This directory contains the complete CI/CD pipeline for the Darkman Theme VS Code extension, built with Batman-level precision and automation.

## 🚀 Workflows Overview

### 1. **Continuous Integration** (`ci.yml`)
**Triggers**: Push to `main`/`develop`, Pull Requests to `main`

**Jobs**:
- 🔧 **Build & Test**: Validates package structure and builds extension
- 🎨 **Validate Batman Colors**: Ensures theme maintains Batman aesthetic consistency
- ♿ **Accessibility Check**: Validates color blind friendly compliance

**Key Features**:
- Validates `package.json` and theme JSON structure
- Checks for required Batman colors (Navy blue, Indigo, Dark red, Joker green, Villain purple)  
- Ensures high contrast text colors are maintained
- Uploads build artifacts for 30 days
- Comprehensive error reporting with Batman-themed messages

### 2. **Release Pipeline** (`release.yml`)
**Triggers**: Version tags (`v*`)

**Jobs**:
- 🎯 **Create Release**: Generates GitHub release with Batman-themed description
- 🏗️ **Build & Publish**: Packages extension and uploads to release
- 📢 **Marketplace Publish**: Publishes to VS Code Marketplace (if `VSCE_PAT` secret exists)

**Key Features**:
- Automatic release creation with Batman quotes and feature highlights
- Professional release notes with installation instructions
- Conditional marketplace publishing (only if secrets are configured)
- Automatic VSIX file attachment to releases

### 3. **PR Preview** (`pr-preview.yml`)
**Triggers**: Pull Request events (opened, synchronize, reopened)

**Jobs**:
- 🎨 **Generate PR Preview**: Creates preview build with PR-specific versioning
- 📊 **Theme Statistics**: Analyzes color usage and Batman theme compliance
- 💬 **PR Comments**: Automatically comments with preview info and download links

**Key Features**:
- Preview builds with PR number and commit SHA in version
- Automated theme statistics (color counts, Batman color usage)
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

### Batman Theme Compliance
- ✅ Navy blue buttons (`#1E3A8A`)
- ✅ Batman indigo accent (`#6366F1`)  
- ✅ Dark red accents (`#8B2635`)
- ✅ Joker green colors (`#7A8650`, `#9FB36B`)
- ✅ Villain purple (`#4A3666`)

### Accessibility Standards
- ✅ High contrast text maintained (`#babed8`)
- ✅ No problematic red-green combinations
- ✅ Color blind friendly design principles

## 🚀 Release Process

### Automated Release
```bash
# Update version in package.json
npm version patch|minor|major

# Create and push tag
git push origin v1.1.0
```

The release workflow will automatically:
1. Create GitHub release with professional description
2. Build and package extension
3. Upload `.vsix` file to release
4. Publish to VS Code Marketplace (if configured)

### Manual Release Steps
If needed, you can manually trigger releases:
```bash
# Build locally
npm run build

# Create release manually
gh release create v1.1.0 darkman-theme-1.1.0.vsix --title "🦇 Darkman Theme v1.1.0"
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
- Theme color statistics
- Accessibility compliance status
- Artifact generation and retention

## 🛠️ Troubleshooting

### Common Issues

**Build Fails**:
- Check `package.json` validity
- Ensure theme JSON is valid
- Verify VSCE can package successfully

**Color Validation Fails**:
- Ensure required Batman colors are present
- Check color hex codes match exactly
- Verify theme maintains Batman aesthetic

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

## 🦇 Batman Development Philosophy

The CI/CD pipeline embodies Batman's approach to excellence:
- **Precision**: Every build is validated thoroughly
- **Reliability**: Automated processes ensure consistency  
- **Quality**: Multiple quality gates maintain standards
- **Accessibility**: Inclusive design is enforced
- **Security**: Secure secrets management and permissions

---

**"The night is darkest just before the dawn. And I promise you, the dawn is coming."** 🦇

*The Darkman Theme CI/CD pipeline ensures that every release maintains the high standards worthy of the Dark Knight himself.*