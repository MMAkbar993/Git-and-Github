# Welcome to Git and GitHub at ChaiCode Cohort! 🚀

## Introduction

Welcome aboard! This guide will walk you through everything you need to know about using Git and GitHub at ChaiCode Cohort. Version control is at the heart of our collaborative development process, helping us work together efficiently while maintaining code quality and history.

## Why Git and GitHub?

Git is a distributed version control system that helps us track changes in our codebase, collaborate with team members, and maintain different versions of our projects. GitHub, our chosen platform for hosting Git repositories, provides additional features like pull requests, issue tracking, and project management tools that are essential for our team collaboration.

## Installation and Setup

### Installing Git

### Windows

1. Download Git from [git-scm.com](https://git-scm.com/)
2. Run the installer with default settings
3. Verify installation by opening Command Prompt and typing:
    
    ```bash
    git --version
    
    ```
    

### macOS

1. Install via Homebrew:
Or download from [git-scm.com](https://git-scm.com/)
    
    ```bash
    brew install git
    
    ```
    

### Linux (Ubuntu/Debian)

```bash
sudo apt-get update
sudo apt-get install git

```

### Initial Configuration

Configure your Git identity:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

```

### GitHub Account Setup

1. Visit [github.com](https://github.com/)
2. Click "Sign Up"
3. Follow the registration process
4. Share your GitHub username with the ChaiCode team lead for repository access

## Working with ChaiCode Repositories

### Cloning a Repository

```bash
git clone <https://github.com/ChaiCode/example-repo.git>
cd example-repo

```

## Essential Git Commands

### Checking Status

View the state of your working directory:

```bash
git status

```

### Making Changes

1. Stage changes:
    
    ```bash
    git add filename
    # or stage all changes:
    git add .
    
    ```
    
2. Commit changes:
    
    ```bash
    git commit -m "feat: Add new feature"
    
    ```
    
3. Push changes:
    
    ```bash
    git push origin branch-name
    
    ```
    
4. Get latest changes:
    
    ```bash
    git pull
    
    ```
    
5. View commit history:
    
    ```bash
    git log
    
    ```
    

## Commit Message Standards

At ChaiCode, we follow a structured commit message format:

### Format

```
type: Subject line (50 chars max)

[optional body]

```

### Types

- `feat:` New features
- `fix:` Bug fixes
- `docs:` Documentation changes
- `style:` Code style changes (formatting, semicolons, etc)
- `refactor:` Code refactoring
- `test:` Adding or modifying tests
- `chore:` Maintenance tasks

### Examples

```bash
feat: Add chai customization options
fix: Resolve tea temperature calculation
docs: Update installation guide

```

## Branching Strategy

We follow a trunk-based development workflow:

### Main Branches

- `main`: Production-ready code
- `develop`: Integration branch for features

### Feature Development

1. Create a feature branch:
    
    ```bash
    git checkout -b feature/tea-menu
    
    ```
    
2. Make your changes and commit regularly
3. Push your branch:
    
    ```bash
    git push origin feature/tea-menu
    
    ```
    

### Merging Changes

1. Update your branch with latest changes:
    
    ```bash
    git checkout develop
    git pull
    git checkout feature/tea-menu
    git merge develop
    
    ```
    
2. Resolve any conflicts if they occur

## Pull Requests (PR)

### Creating a PR

1. Push your feature branch to GitHub
2. Go to the repository on GitHub
3. Click "New Pull Request"
4. Select your feature branch as the source
5. Add a descriptive title and description
6. Request reviews from team members

### PR Description Template

```markdown
## Description
[Describe the changes you've made]

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Documentation update
- [ ] Code refactoring

## Testing
- [ ] Unit tests added/updated
- [ ] Tested manually

## Screenshots
[If applicable]

```

## Best Practices

### Daily Workflow

1. Start your day by pulling latest changes:
    
    ```bash
    git pull
    
    ```
    
2. Create or switch to your feature branch:
    
    ```bash
    git checkout feature/your-feature
    
    ```
    
3. Make small, focused commits regularly
4. Push your changes at least daily:
    
    ```bash
    git push origin feature/your-feature
    
    ```
    

### Code Review Guidelines

- Review PRs within 24 hours
- Provide constructive feedback
- Use GitHub's review features for inline comments
- Approve only when all comments are resolved

### Avoiding Common Issues

1. Always pull before starting new work
2. Don't commit directly to `main` or `develop`
3. Keep commits focused and atomic
4. Write meaningful commit messages
5. Regular pushes prevent large merge conflicts

## Need Help?

- Check the #git-help Slack channel
- Ask in team meetings
- Contact your team lead
- Review this documentation

Remember: There are no "stupid" questions when it comes to Git. We're here to help!