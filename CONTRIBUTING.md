# Contributing to TikTok Bonus Landing Page

Thank you for your interest in contributing to this project! We welcome contributions from everyone.

## How to Contribute

### Reporting Issues

If you find a bug or have a suggestion for improvement:

1. Check if the issue already exists in our [Issues](https://github.com/yourusername/tiktok-bonus-landing/issues)
2. If not, create a new issue with:
   - Clear title and description
   - Steps to reproduce (for bugs)
   - Expected vs actual behavior
   - Screenshots if applicable
   - Your environment details (browser, OS, etc.)

### Making Changes

1. **Fork the repository**
   ```bash
   git clone https://github.com/yourusername/tiktok-bonus-landing.git
   ```

2. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make your changes**
   - Follow the existing code style
   - Add comments for complex logic
   - Update documentation if needed

4. **Test your changes**
   ```bash
   npm run dev
   npm run build
   npm run lint
   ```

5. **Commit your changes**
   ```bash
   git add .
   git commit -m "Add: brief description of your changes"
   ```

6. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```

7. **Create a Pull Request**
   - Go to the original repository
   - Click "New Pull Request"
   - Select your branch
   - Fill out the PR template

## Code Style Guidelines

### TypeScript/React
- Use functional components with hooks
- Use TypeScript for type safety
- Follow React best practices
- Use meaningful variable and function names

### CSS/Tailwind
- Use Tailwind CSS classes
- Follow mobile-first responsive design
- Maintain consistent spacing (8px grid system)
- Use semantic color names

### File Organization
- Keep components focused and single-purpose
- Use clear, descriptive file names
- Group related functionality together

## Commit Message Format

Use clear, descriptive commit messages:

```
Type: Brief description

Longer description if needed

- Bullet points for multiple changes
- Reference issues with #123
```

**Types:**
- `Add:` New features
- `Fix:` Bug fixes
- `Update:` Changes to existing features
- `Remove:` Deleted features
- `Docs:` Documentation changes
- `Style:` Code formatting changes
- `Refactor:` Code restructuring
- `Test:` Adding or updating tests

## Pull Request Guidelines

### Before Submitting
- [ ] Code follows project style guidelines
- [ ] Changes have been tested locally
- [ ] Documentation updated if needed
- [ ] No console errors or warnings
- [ ] Responsive design maintained

### PR Description Template
```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Documentation update
- [ ] Performance improvement
- [ ] Code refactoring

## Testing
- [ ] Tested on desktop
- [ ] Tested on mobile
- [ ] Tested on different browsers
- [ ] No console errors

## Screenshots
If applicable, add screenshots

## Additional Notes
Any additional information
```

## Development Setup

1. **Prerequisites**
   - Node.js 18+
   - npm or yarn
   - Git

2. **Installation**
   ```bash
   npm install
   ```

3. **Development Server**
   ```bash
   npm run dev
   ```

4. **Build for Production**
   ```bash
   npm run build
   ```

## Code Review Process

1. All submissions require review
2. Maintainers will review PRs within 48 hours
3. Address feedback promptly
4. Once approved, maintainers will merge

## Community Guidelines

- Be respectful and inclusive
- Help others learn and grow
- Focus on constructive feedback
- Follow the project's code of conduct

## Questions?

If you have questions about contributing:
- Create an issue with the "question" label
- Reach out to maintainers
- Check existing documentation

Thank you for contributing! 🎉