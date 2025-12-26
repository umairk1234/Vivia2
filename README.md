# Vivia - Agents, Tools & Knowledge Platform

A workspace for building AI agents, tools, knowledge management, and data visualization dashboards for Vivia.

## Project Structure

```
Vivia/
├── agents/          # AI agents and automation scripts
├── tools/           # Custom tools and utilities
├── knowledge/       # Knowledge base, documentation, and swipe files
├── dashboards/      # Data visualization dashboards
└── config/          # Configuration files
```

## Getting Started

1. Open this folder in Cursor: **File → Open Folder → Select the Vivia folder**
2. Start building your agents, tools, and knowledge base

## Components

- **Agents**: AI-powered automation and decision-making agents
- **Tools**: Custom utilities and helper functions
- **Knowledge**: Swipe files, documentation, and reference materials
- **Dashboards**: Data visualization and analytics

## Version Control & Backup

This workspace is set up with Git for version control. To back up your work online and access it from anywhere:

### Option 1: GitHub (Recommended)

1. **Create a GitHub repository:**
   - Go to [github.com](https://github.com) and sign in
   - Click the "+" icon → "New repository"
   - Name it (e.g., "vivia-ecommerce")
   - Choose Private (recommended for business code)
   - **Don't** initialize with README (we already have one)
   - Click "Create repository"

2. **Connect your local repository:**
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/vivia-ecommerce.git
   git branch -M main
   git push -u origin main
   ```

3. **Future updates:**
   ```bash
   git add .
   git commit -m "Your commit message"
   git push
   ```

### Option 2: GitLab

1. Create a repository at [gitlab.com](https://gitlab.com)
2. Follow similar steps as GitHub, using your GitLab repository URL

### Option 3: Bitbucket

1. Create a repository at [bitbucket.org](https://bitbucket.org)
2. Follow similar steps as GitHub, using your Bitbucket repository URL

### Quick Commands Reference

- **Check status:** `git status`
- **Add changes:** `git add .`
- **Commit changes:** `git commit -m "Description of changes"`
- **Push to remote:** `git push`
- **Pull latest changes:** `git pull`

**Note:** Your `.env` files and sensitive data are automatically excluded via `.gitignore` for security.

