# Contributing to PunchPulse Accessible VR Boxing Game

We welcome contributions to improve the game's accessibility and features. This document outlines the development workflow, coding standards, and contribution process.

## Development Workflow

### Branch Structure

```
main                    # Production-ready releases
develop                 # Integration branch
feature/accessibility  # Accessibility improvements
feature/gameplay       # Gameplay mechanics
hotfix/critical        # Critical bug fixes
```

### Getting Started

1. Fork the repository
2. Create a feature branch from `develop`
3. Make your changes following our coding standards
4. Test your changes thoroughly
5. Submit a pull request

## Code Standards

### C# Conventions

- Microsoft C# Coding Conventions
- XML documentation for public APIs
- Async/await patterns for I/O operations
- SOLID principles adherence

### Unity-Specific Guidelines

- MonoBehavior lifecycle awareness
- Proper object pooling for performance
- ScriptableObject configuration patterns
- Prefab-based architecture

### Accessibility Requirements

All contributions must maintain accessibility standards:

1. **Audio Implementation**

   - Spatial audio with fallback to stereo
   - Configurable audio descriptions
   - Multiple language support preparation

2. **Haptic Design**

   - Consistent vibration patterns
   - Intensity scaling options
   - Battery impact consideration

3. **Navigation Systems**
   - Keyboard/controller navigation
   - Screen reader compatibility
   - Logical tab order implementation

## Pull Request Process

### Pre-submission Checklist

- [ ] Code follows project conventions
- [ ] Accessibility features tested with screen readers
- [ ] Performance impact documented
- [ ] Unit tests added/updated
- [ ] Documentation updated

### Review Criteria

1. **Functionality**: Feature works as specified
2. **Accessibility**: Maintains inclusive design principles
3. **Performance**: No significant frame rate impact
4. **Code Quality**: Readable, maintainable, documented
5. **Testing**: Adequate test coverage

### Pull Request Template

When submitting a pull request, please include:

- Clear description of changes
- Testing methodology
- Accessibility impact assessment
- Performance considerations
- Screenshots/videos if applicable

## Issue Reporting

### Bug Reports

```markdown
**Environment:**

- Unity Version: [version]
- VR Device: [device model]
- OS: [operating system]

**Reproduction Steps:**

1. [Step one]
2. [Step two]
3. [Expected vs actual behavior]
```

### Feature Requests

Include implementation approach and technical specifications.

## Commit Style

We follow a consistent commit message format:

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types

- `feat`: A new feature
- `fix`: A bug fix
- `docs`: Documentation only changes
- `style`: Changes that do not affect the meaning of the code
- `refactor`: A code change that neither fixes a bug nor adds a feature
- `perf`: A code change that improves performance
- `test`: Adding missing tests
- `chore`: Changes to build process or auxiliary tools

### Examples

```
feat(audio): add spatial audio positioning system
fix(haptics): resolve controller vibration timing issue
docs(readme): update build instructions for Quest 3
```

## Testing

### Unit Testing

- Use Unity Test Framework
- Maintain component-level test coverage
- Include accessibility feature validation

### VR Testing Protocol

1. **Headset Verification**: Multi-device compatibility testing
2. **Accessibility Validation**: Screen reader simulation
3. **Performance Profiling**: Frame rate and latency analysis
4. **User Experience Testing**: Validate with accessibility features

## Development Environment

### Required Tools

- Unity 2022.3.x LTS
- Visual Studio or VS Code
- Git
- VR headset for testing

### Recommended Extensions

- Unity Visual Scripting
- XR Interaction Toolkit
- Accessibility Insights (for testing)

## Community Guidelines

- Be respectful and inclusive
- Provide constructive feedback
- Focus on accessibility and user experience
- Document your changes clearly
- Test thoroughly before submitting

Thank you for contributing to making VR more accessible!

- chore: Changes to the build process or auxiliary tools

Example:

```
feat(audio): add spatial audio for opponent position

- Implement 3D audio positioning
- Add distance-based volume adjustment
- Include directional cues for movement

Closes #123
```

## Creating Issues

When creating an issue, please:

1. Provide a clear and descriptive title
2. Describe the issue in detail
3. Include steps to reproduce if it's a bug
4. Add screenshots or videos if applicable
5. Label the issue appropriately

## Code Style

- Follow Unity's C# coding conventions
- Use meaningful variable and function names
- Comment complex logic
- Keep functions focused and single-purpose
- Maintain consistent indentation and formatting

## License

By contributing, you agree that your contributions will be licensed under the project's MIT License.
