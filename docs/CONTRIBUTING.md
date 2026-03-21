# Contributing to AgroConnect

Thank you for your interest in contributing to AgroConnect! This document provides guidelines and information for contributing to the project.

---

## 🎯 Our Mission

We believe in combining efforts to create a healthier, more sustainable future through organic agriculture. Your contributions help us achieve this goal.

---

## 📋 Table of Contents

1. [Getting Started](#getting-started)
2. [Ways to Contribute](#ways-to-contribute)
3. [Development Setup](#development-setup)
4. [Coding Standards](#coding-standards)
5. [Commit Guidelines](#commit-guidelines)
6. [Pull Request Process](#pull-request-process)
7. [Code of Conduct](#code-of-conduct)
8. [Reporting Issues](#reporting-issues)

---

## 🚀 Getting Started

### Prerequisites
- Git knowledge (basics)
- HTML, CSS, and JavaScript understanding
- Willingness to learn and improve

### First Steps
1. Fork the repository on GitHub
2. Clone your fork locally
3. Create a feature branch
4. Make your changes
5. Submit a pull request

---

## 💡 Ways to Contribute

### 1. **Code Contributions**
- ✅ Bug fixes
- ✅ New features
- ✅ Performance improvements
- ✅ Code optimization
- ✅ Browser compatibility fixes

### 2. **Documentation**
- 📝 README updates
- 📝 Feature documentation
- 📝 Installation guides
- 📝 API documentation
- 📝 Tutorial creation

### 3. **Design & UX**
- 🎨 UI/UX improvements
- 🎨 Icon design
- 🎨 Color scheme optimization
- 🎨 Responsive design fixes
- 🎨 Accessibility enhancements

### 4. **Testing**
- 🧪 Bug reporting
- 🧪 Cross-browser testing
- 🧪 Mobile device testing
- 🧪 Performance testing
- 🧪 Accessibility testing

### 5. **Content**
- ✍️ Blog post writing
- ✍️ Case studies
- ✍️ Tutorial videos
- ✍️ Social media content
- ✍️ Translation

### 6. **Community**
- 💬 Help other contributors
- 💬 Review pull requests
- 💬 Answer questions
- 💬 Promote the project
- 💬 Event organization

---

## 🛠️ Development Setup

### 1. Fork & Clone
```bash
# Fork on GitHub (use web interface)

# Clone your fork
git clone https://github.com/yourusername/AgroConnect.git
cd AgroConnect

# Add upstream remote
git remote add upstream https://github.com/original-owner/AgroConnect.git
```

### 2. Create Feature Branch
```bash
# Update main branch
git fetch upstream
git checkout main
git merge upstream/main

# Create feature branch
git checkout -b feature/your-feature-name
# or
git checkout -b fix/bug-description
```

### 3. Setup Development Environment
```bash
# Install dependencies (if applicable)
npm install

# Start development server
npm start
# or
python -m http.server 8000
```

### 4. Make Your Changes
- Create/modify files
- Test thoroughly
- Verify responsive design
- Check browser compatibility

---

## 📋 Coding Standards

### HTML Standards
```html
<!-- Use semantic HTML -->
<header>
  <nav>
    <ul>
      <li><a href="#">Home</a></li>
    </ul>
  </nav>
</header>

<main>
  <article>
    <h1>Article Title</h1>
    <p>Content goes here</p>
  </article>
</main>

<footer>
  <p>&copy; 2026 AgroConnect</p>
</footer>

<!-- Guidelines -->
<!-- ✓ Use lowercase tag names -->
<!-- ✓ Use double quotes for attributes -->
<!-- ✓ Include alt text for images -->
<!-- ✓ Use proper heading hierarchy -->
<!-- ✓ Include proper meta tags -->
```

### CSS Standards
```css
/* Use organized structure */
/* Layout Styles */
.container {
  display: flex;
  width: 100%;
}

/* Typography Styles */
h1 {
  font-size: 2.5rem;
  font-weight: 700;
}

/* Component Styles */
.button {
  padding: 10px 20px;
  background-color: #2ecc71;
}

/* Guidelines */
/* ✓ Use CSS variables for colors */
/* ✓ Sort properties alphabetically */
/* ✓ Use meaningful class names */
/* ✓ Keep specificity low */
/* ✓ Mobile-first approach */
```

### JavaScript Standards
```javascript
// Use clear, descriptive names
function handleMenuToggle() {
  const menu = document.getElementById('menu');
  menu.classList.toggle('active');
}

// Guidelines
// ✓ Use const/let, avoid var
// ✓ Use arrow functions
// ✓ Add comments for complex logic
// ✓ Handle errors appropriately
// ✓ Use async/await for promises
```

### Naming Conventions
```
Files:     kebab-case (my-component.js)
Classes:   kebab-case (.my-class)
IDs:       camelCase (#myId)
Variables: camelCase (myVariable)
Constants: UPPER_SNAKE_CASE (MY_CONSTANT)
```

### Comments & Documentation
```javascript
/**
 * Brief description of the function
 * @param {type} paramName - Description
 * @returns {type} Description
 */
function myFunction(paramName) {
  // Implementation
}
```

---

## 📝 Commit Guidelines

### Commit Message Format
```
<type>(<scope>): <subject>

<body>

<footer>
```

### Type
- `feat:` A new feature
- `fix:` A bug fix
- `docs:` Documentation only
- `style:` Changes that don't affect code meaning
- `refactor:` Code change without feature or bug fix
- `perf:` Code change that improves performance
- `test:` Adding or updating tests
- `chore:` Changes to build process or dependencies

### Subject Line
- Use imperative mood ("add" not "added")
- Don't capitalize first letter
- No period at the end
- Keep it under 50 characters

### Examples
```
feat(navbar): add dropdown menu for services
fix(responsive): correct mobile menu alignment
docs(readme): update installation instructions
style(css): format code according to standards
```

### Git Commit Commands
```bash
# Stage changes
git add filename.html

# Commit with message
git commit -m "feat(pages): add about page content"

# View commit history
git log --oneline

# Amend last commit (if not pushed)
git commit --amend
```

---

## 🔄 Pull Request Process

### 1. Before Starting
- [ ] Check existing issues/PRs to avoid duplicates
- [ ] Create an issue for discussion (if major change)
- [ ] Fork the repository
- [ ] Clone your fork locally

### 2. Development
- [ ] Create feature branch from main
- [ ] Make changes following coding standards
- [ ] Test thoroughly on multiple devices
- [ ] Update documentation if needed
- [ ] Add comments for complex logic

### 3. Prepare to Submit
```bash
# Update your branch with latest changes
git fetch upstream
git rebase upstream/main

# Push to your fork
git push origin feature/your-feature-name

# Create pull request on GitHub
```

### 4. Pull Request Template
```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Documentation update
- [ ] Performance improvement

## Related Issue
Fixes #(issue number)

## Testing Done
Describe testing performed

## Screenshots (if applicable)
Add screenshots of visual changes

## Checklist
- [ ] Code follows style guidelines
- [ ] Comments added for complexity
- [ ] Documentation updated
- [ ] Tested on mobile/tablet/desktop
- [ ] No console errors
- [ ] Responsive design verified
```

### 5. Review & Merge
- [ ] Wait for code review
- [ ] Address review comments
- [ ] Request re-review if needed
- [ ] Project maintainer merges when approved

---

## ⚖️ Code of Conduct

### Expected Behavior
- 🤝 Be respectful and inclusive
- 🎯 Focus on the code, not the person
- 📚 Help others learn and grow
- 🙌 Celebrate diverse perspectives
- 🚀 Work toward common goals

### Unacceptable Behavior
- ❌ Harassment or discrimination
- ❌ Personal attacks
- ❌ Spam or advertising
- ❌ Sharing private information
- ❌ Other unethical conduct

### Reporting Issues
Contact project maintainers at your-email@example.com with details of the incident.

---

## 🐛 Reporting Issues

### Bug Report Template
```markdown
## Describe the Bug
Clear description of what's wrong

## Steps to Reproduce
1. Go to '...'
2. Click on '...'
3. See error

## Expected Behavior
What should happen instead

## Actual Behavior
What actually happens

## Environment
- Device: (phone/tablet/desktop)
- Browser: (Chrome/Firefox/Safari)
- OS: (Windows/Mac/Linux)

## Screenshots
Add screenshots if helpful

## Additional Context
Any other relevant information
```

### Feature Request Template
```markdown
## Description
Clear description of the feature

## Problem It Solves
What issue does this address

## Proposed Solution
Suggested implementation

## Examples
Real-world use cases

## Additional Context
Design mockups or references
```

### Submitting Issues
1. Go to [GitHub Issues](https://github.com/yourusername/AgroConnect/issues)
2. Click "New Issue"
3. Choose template (Bug Report or Feature Request)
4. Fill in all sections
5. Submit

---

## 🎓 Learning Resources

### Documentation
- [MDN Web Docs](https://developer.mozilla.org/)
- [CSS-Tricks](https://css-tricks.com/)
- [Eloquent JavaScript](https://eloquentjavascript.net/)

### Tools
- [VS Code](https://code.visualstudio.com/)
- [Git Documentation](https://git-scm.com/doc)
- [Can I Use](https://caniuse.com/)

### Community
- GitHub Discussions (in repo)
- Stack Overflow (tag projects)
- Dev Communities

---

## 🏆 Recognition

Contributors will be recognized in:
- 📋 README.md Contributors section
- 🏅 GitHub contributor graph
- 📢 Release notes
- 💌 Special mentions

---

## ❓ FAQ

### Q: I'm new to open source, where do I start?
A: Look for issues labeled `good-first-issue` or `help-wanted`. Start with documentation or small bug fixes.

### Q: How long does review take?
A: Typically 3-5 days, but may vary based on complexity.

### Q: Can I work on multiple features?
A: Yes! Create separate branches and PRs for each feature.

### Q: What if my PR is rejected?
A: Review feedback, ask questions, and try again. Rejection is about the code, not you.

### Q: How do I update my fork?
A: 
```bash
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
```

---

## 📞 Contact

- **Questions:** Open a GitHub Discussion
- **Issues:** Report on GitHub Issues
- **Email:** your-email@example.com
- **Twitter:** @AgroConnect

---

## 📄 License

By contributing, you agree that your contributions will be licensed under the MIT License.

---

**Thank you for contributing to AgroConnect! Together, we're building a healthier future.** 🌱

**Last Updated:** March 2026  
**Status:** Contributing Guide v1.0
