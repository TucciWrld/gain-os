# Contributing to Gain OS

Thank you for your interest in contributing to Gain OS! This document outlines our contribution guidelines and process.

## Code of Conduct

We are committed to providing a welcoming and inclusive environment. Please read and follow our [Code of Conduct](CODE_OF_CONDUCT.md).

## How to Contribute

### Reporting Bugs

1. **Check existing issues** to avoid duplicates
2. **Use a clear title** that describes the problem
3. **Provide detailed description** with:
   - Steps to reproduce
   - Expected behavior
   - Actual behavior
   - System information (OS version, hardware)
   - Screenshots/logs if applicable

### Suggesting Features

1. **Search existing issues** for similar suggestions
2. **Clearly describe** the feature and use cases
3. **Explain benefits** to the project
4. **Provide examples** or mockups if helpful

### Submitting Pull Requests

#### Setup Development Environment

```bash
# Clone the repository
git clone https://github.com/TucciWrld/gain-os.git
cd gain-os

# Create a new branch
git checkout -b feature/your-feature-name

# Install development dependencies
./scripts/setup-dev-environment.sh
```

#### Development Guidelines

1. **Follow code style**: Use consistent formatting (see `.editorconfig`)
2. **Write tests**: All new features need tests
3. **Update documentation**: Keep docs in sync with code
4. **Commit messages**: Use clear, descriptive messages

```
Format: [type] Brief description

Types:
- feat: New feature
- fix: Bug fix
- docs: Documentation
- style: Code style
- refactor: Code refactoring
- test: Test additions
- chore: Build process
```

#### Submit Your PR

1. **Push to your fork**: `git push origin feature/your-feature-name`
2. **Create pull request** with:
   - Clear title
   - Detailed description
   - Reference related issues
   - Checklist of changes
3. **Respond to feedback** and iterate

### Areas We Need Help With

#### High Priority
- [ ] Application development (any of the Gain suite)
- [ ] Kernel optimizations
- [ ] Security hardening
- [ ] Performance improvements

#### Medium Priority
- [ ] UI/UX design and implementation
- [ ] Internationalization (i18n)
- [ ] Testing and QA
- [ ] Documentation

#### Lower Priority
- [ ] Additional themes
- [ ] Community applications
- [ ] Translation improvements
- [ ] Community guides

## Development Workflow

### Branch Naming

```
feature/short-description     # New feature
fix/issue-number-description  # Bug fix
docs/description              # Documentation
refactor/description          # Code refactoring
```

### Commit Workflow

```bash
# Make changes
git add .

# Commit with clear message
git commit -m "feat: Add dark theme support to Gain Hub"

# Push to remote
git push origin feature/dark-theme
```

### Testing Before Submit

```bash
# Run all tests
make test

# Run specific test suite
make test-applications
make test-kernel

# Build locally
make build

# Create ISO for testing
make iso
```

## Review Process

1. **Automated checks**: CI/CD pipeline runs
2. **Code review**: Maintainers review code
3. **Testing**: QA team tests functionality
4. **Feedback**: Address comments and suggestions
5. **Merge**: Approved PRs are merged

## Contributor Levels

### Level 1: Contributor
- Can submit PRs
- Can review code (non-binding)
- Can contribute to discussions

### Level 2: Reviewer
- 5+ merged PRs
- Can review and approve PRs
- Can label and triage issues

### Level 3: Maintainer
- 20+ merged PRs or significant contributions
- Can merge PRs
- Can manage repository settings
- Can release versions

## Licensing

By contributing, you agree that your contributions will be licensed under the same licenses as the Gain OS project:
- GPL v3 for kernel/system components
- MIT for applications
- Apache 2.0 for developer resources

## Resources

- [Developer Guide](docs/development.md)
- [Architecture Overview](docs/architecture.md)
- [API Reference](docs/api/)
- [Style Guide](docs/style-guide.md)

## Questions?

- **GitHub Discussions**: Start a discussion
- **Discord**: Join our community server
- **Issues**: Ask in related issue

---

Thank you for contributing to Gain OS!
