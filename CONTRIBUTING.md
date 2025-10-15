# Contributing to Tridi Cookies

## Development Setup

1. Clone the repository
2. Install dependencies: `npm install`
3. Run development server: `npm run dev`
4. Run tests: `npm test`
5. Build package: `npm run build`

## Commit Message Convention

This project uses [Semantic Release](https://semantic-release.gitbook.io/) for automated versioning and publishing. Follow this commit message format:

### Format

```
<type>(<scope>): <description>

[optional body]

[optional footer]
```

### Types

- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes (formatting, missing semi colons, etc.)
- `refactor`: Code refactoring
- `test`: Adding or updating tests
- `chore`: Maintenance tasks

### Examples

```
feat: add dark mode support
fix: resolve cookie consent modal positioning issue
docs: update installation guide
test: add unit tests for cookie validation
chore: update dependencies
```

## Release Process

### Automated Releases (Semantic Release)

When you push to the `main` branch:

1. Semantic Release analyzes commit messages
2. Determines the next version (patch/minor/major)
3. Updates package.json version
4. Generates changelog
5. Creates GitHub release
6. Publishes to NPM

### Manual Releases (GitHub Releases)

You can still create releases manually through GitHub:

1. Create a new release with a tag (e.g., `v1.2.3`)
2. Ensure `package.json` version matches the tag
3. GitHub Actions will automatically publish to NPM

## Version Determination

- `fix` commits → Patch release (1.0.1)
- `feat` commits → Minor release (1.1.0)
- `feat!` or `BREAKING CHANGE` → Major release (2.0.0)

## Testing

Before contributing:

1. Run tests: `npm test`
2. Check code style: `npm run lint` (if available)
3. Build successfully: `npm run build`
4. Test your changes manually

## Pull Request Process

1. Fork the repository
2. Create a feature branch
3. Make your changes with proper commit messages
4. Test your changes
5. Submit a pull request to `main`

Thank you for contributing! 🍪
