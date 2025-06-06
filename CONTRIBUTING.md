# Contributing to Microsoft PowerToys Assistant

We love your input! We want to make contributing to this project as easy and transparent as possible.

## 🚀 Quick Start

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📋 How to Contribute

### 🐛 Reporting Bugs

Use our bug report template when creating issues. Include:

- **Operating System**: Windows version and build
- **PowerToys Version**: Target version being deployed
- **Steps to Reproduce**: Detailed step-by-step instructions
- **Expected vs Actual Behavior**: What should happen vs what happened
- **Screenshots/Logs**: If applicable

### 💡 Suggesting Features

Feature requests are welcome! Please:

- Use the feature request template
- Explain the problem you're solving
- Describe your proposed solution
- Consider the impact on existing users

### 🔧 Code Contributions

#### Development Setup

```bash
# Clone your fork
git clone https://github.com/YOUR-USERNAME/microsoftpowertoys.git
cd microsoftpowertoys

# Set up upstream remote
git remote add upstream https://github.com/Microsoft-Tools/microsoftpowertoys.git
```

#### Coding Standards

- **PowerShell**: Follow [PowerShell Best Practices](https://docs.microsoft.com/en-us/powershell/scripting/dev-cross-plat/writing-portable-modules)
- **Batch Scripts**: Use consistent indentation and comment complex logic
- **Documentation**: Update relevant docs with your changes
- **Testing**: Test on clean Windows 10 and 11 environments

#### Pull Request Process

1. Update the `CHANGELOG.md` with details of changes
2. Update the `README.md` if you change functionality
3. Ensure any install or build dependencies are documented
4. Your PR will be merged once you have sign-off from maintainers

## 🧪 Testing

### Manual Testing Checklist

Before submitting:

- [ ] Test on clean Windows 10 (latest)
- [ ] Test on clean Windows 11 (latest)
- [ ] Test with Windows Defender enabled
- [ ] Test with limited user account
- [ ] Test in offline environment
- [ ] Verify uninstall process

### Automated Testing

```bash
# Run validation scripts
.\scripts\validate-setup.ps1

# Test deployment
.\scripts\test-deployment.ps1 -Offline
```

## 📝 Documentation

### Writing Guidelines

- Use clear, concise language
- Include code examples where helpful
- Test all instructions before submitting
- Consider different user skill levels

### Documentation Structure

```
docs/
├── setup/          # Setup guides
├── troubleshooting/ # Common issues
├── advanced/       # Power user features
└── api/           # Scripting reference
```

## 🏷️ Versioning

We use [Semantic Versioning](http://semver.org/):

- **MAJOR**: Incompatible API changes
- **MINOR**: Add functionality (backwards compatible)
- **PATCH**: Bug fixes (backwards compatible)

## 📞 Community

- **Issues**: GitHub Issues for bug reports and feature requests
- **Discussions**: GitHub Discussions for questions and ideas
- **Security**: See `SECURITY.md` for reporting security issues

## 🙏 Recognition

Contributors will be recognized in:

- `CONTRIBUTORS.md` file
- Release notes for their contributions
- GitHub contributors graph

## 📄 License

By contributing, you agree that your contributions will be licensed under the MIT License.

---

**Thank you for contributing to Microsoft PowerToys Assistant!** 🎉 