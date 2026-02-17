# Contributing to Form Strength

First off, thank you for considering contributing to Form Strength! 🎉

It's people like you that make Form Strength such a great tool. Following these guidelines helps to communicate that you respect the time of the developers managing and developing this open source project.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Getting Started](#getting-started)
- [Development Process](#development-process)
- [Style Guidelines](#style-guidelines)
- [Commit Messages](#commit-messages)
- [Pull Request Process](#pull-request-process)

## Code of Conduct

By participating in this project, you are expected to uphold our Code of Conduct:

- **Be respectful**: Treat everyone with respect and kindness
- **Be constructive**: Provide helpful feedback and suggestions
- **Be collaborative**: Work together to improve the project
- **Be patient**: Remember that everyone is here to learn and contribute

## How Can I Contribute?

### Reporting Bugs 🐛

Before creating bug reports, please check existing issues to avoid duplicates. When creating a bug report, include:

- **Clear title and description**
- **Steps to reproduce** the issue
- **Expected behavior** vs **actual behavior**
- **Screenshots** if applicable
- **Browser and OS** information
- **Any error messages** from the console

**Template:**
```markdown
**Bug Description:**
A clear description of what the bug is.

**To Reproduce:**
1. Go to '...'
2. Click on '....'
3. Scroll down to '....'
4. See error

**Expected Behavior:**
What you expected to happen.

**Screenshots:**
If applicable, add screenshots.

**Environment:**
- Browser: [e.g. Chrome 100]
- OS: [e.g. Windows 11]
- Version: [e.g. 2.0.0]
```

### Suggesting Enhancements 💡

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion, include:

- **Clear title and description**
- **Use case** - why would this be useful?
- **Possible implementation** - if you have ideas
- **Alternatives considered**
- **Additional context** or screenshots

### Contributing Code 💻

1. **Fork the repository**
2. **Create a feature branch** from `main`
3. **Make your changes**
4. **Test thoroughly**
5. **Commit with clear messages**
6. **Push to your fork**
7. **Open a Pull Request**

## Getting Started

### Prerequisites

- A modern web browser
- Text editor (VS Code recommended)
- Git installed
- Basic knowledge of HTML, CSS, and JavaScript

### Setup

1. Fork and clone the repository:
```bash
git clone https://github.com/YOUR-USERNAME/Form_strength.git
cd Form_strength
```

2. Create a branch for your changes:
```bash
git checkout -b feature/your-feature-name
```

3. Open `index.html` in your browser to test:
```bash
# Windows
start index.html

# macOS
open index.html

# Linux
xdg-open index.html
```

## Development Process

### Directory Structure

```
Form_strength/
├── assets/
│   └── images/        # Image assets
├── css/
│   └── style.css      # All styles
├── js/
│   └── password-strength.js  # Password validation logic
├── index.html         # Main HTML file
├── README.md
├── LICENSE
└── CHANGELOG.md
```

### Testing Your Changes

1. **Visual Testing**: Open `index.html` in multiple browsers
2. **Responsive Testing**: Test on different screen sizes
3. **Functional Testing**: 
   - Try different password combinations
   - Test all form inputs
   - Check password strength calculations

### Browser Testing Checklist

- [ ] Chrome (latest)
- [ ] Firefox (latest)
- [ ] Safari (latest)
- [ ] Edge (latest)
- [ ] Mobile browsers (Chrome/Safari)

## Style Guidelines

### HTML

- Use semantic HTML5 elements
- Include ARIA labels for accessibility
- Maintain proper indentation (2 spaces)
- Use double quotes for attributes
- Add comments for complex sections

```html
<!-- Good -->
<button type="submit" aria-label="Submit registration form">
  Register Now
</button>

<!-- Avoid -->
<button type=submit>
Register Now
</button>
```

### CSS

- Use meaningful class names (kebab-case)
- Group related properties
- Include comments for sections
- Maintain consistent spacing (2 spaces)
- Use CSS custom properties for theming
- Mobile-first approach for responsive design

```css
/* Good */
.input-box {
  margin: 25px auto;
  width: 100%;
  position: relative;
}

/* Avoid */
.input-box{margin:25px auto;width:100%;position:relative;}
```

### JavaScript

- Use meaningful variable names (camelCase)
- Add JSDoc comments for functions
- Use strict mode
- Handle errors gracefully
- Keep functions focused and small

```javascript
// Good
/**
 * Calculates password strength based on various criteria
 * @param {string} password - The password to evaluate
 * @returns {number} Strength score
 */
function calculatePasswordStrength(password) {
  // Implementation
}

// Avoid
function calc(p) {
  // Implementation
}
```

## Commit Messages

Follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

### Format
```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes (formatting, etc.)
- `refactor`: Code refactoring
- `perf`: Performance improvements
- `test`: Adding or updating tests
- `chore`: Maintenance tasks

### Examples

```bash
# Feature
feat(validation): add email format validation

# Bug fix
fix(css): correct responsive breakpoint for mobile

# Documentation
docs(readme): update installation instructions

# Style changes
style(css): improve button hover animation

# Refactoring
refactor(js): simplify password strength calculation
```

## Pull Request Process

### Before Submitting

- [ ] Code follows the style guidelines
- [ ] Self-review of your code
- [ ] Commented complex sections
- [ ] Tested on multiple browsers
- [ ] Updated documentation if needed
- [ ] No console errors or warnings

### PR Template

```markdown
## Description
Brief description of the changes.

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Breaking change
- [ ] Documentation update

## How Has This Been Tested?
Describe your testing process.

## Screenshots (if applicable)
Add screenshots to demonstrate changes.

## Checklist
- [ ] My code follows the style guidelines
- [ ] I have commented my code
- [ ] I have updated the documentation
- [ ] My changes generate no new warnings
- [ ] I have tested on multiple browsers
```

### Review Process

1. Maintainers will review your PR
2. Address any requested changes
3. Once approved, your PR will be merged
4. Your contribution will be acknowledged in the changelog

## Recognition

Contributors will be recognized in:
- The project README
- The CHANGELOG for their specific contributions
- GitHub's contributor page

## Questions?

Feel free to:
- Open an issue for discussion
- Contact the maintainer: Rajjit Laishram
- Check existing documentation

## License

By contributing, you agree that your contributions will be licensed under the MIT License.

---

Thank you for contributing to Form Strength! 🚀

Every contribution, no matter how small, makes a difference! ❤️
