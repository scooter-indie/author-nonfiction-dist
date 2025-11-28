# AI-Assisted Nonfiction Authoring Framework

**Distribution Repository** - Clone this repo to start writing nonfiction books with AI assistance.

---

## Quick Start

### Option A: Single Book (Simplest)

```bash
# 1. Clone the framework to your book project
git clone https://github.com/scooter-indie/author-nonfiction-dist.git my-book
cd my-book

# 2. Start Claude Code
claude

# 3. Configure and initialize (say these in Claude Code)
execute configure.md
execute Prompt 1
```

After setup, start each session with `/fw-init`.

### Option B: Multi-Book Setup (Recommended for Multiple Books)

This setup separates the framework from your books, allowing you to:
- Manage multiple book projects from one framework installation
- Update the framework without touching your books
- Switch between books easily

```bash
# 1. Clone framework to a permanent location
git clone https://github.com/scooter-indie/author-nonfiction-dist.git ~/nonfiction-framework
cd ~/nonfiction-framework

# 2. Start Claude Code and configure
claude
execute configure.md
```

Configuration will ask where to store your books (BOOKS_ROOT). After setup:
- **Windows:** Double-click `start-authoring.bat` to launch
- **macOS/Linux:** Run `./start-authoring.sh` to launch

The start script opens Claude Code in your books directory and reminds you to run `/fw-init`.

---

## Key Features

- 📝 **16 Conversational Prompts** for writing, editing, and publishing
- 🎨 **19 Writing Styles** across 5 categories (or create your own)
- 📚 **Multi-Book Support** - Work on multiple books from one framework
- 🔍 **Consistency Checking** and quality control
- 📦 **Export to DOCX, PDF, EPUB** for publication
- ✨ **Anti-Hallucination Guidelines** for factual accuracy

---

## Session Workflow

```bash
# Start each session
/fw-init

# Common commands
execute Prompt 3    # Apply changes from _chg files
execute Prompt 4    # Interactive editing
execute Prompt 10   # View progress dashboard
execute Prompt 8    # Consistency check
```

---

## Documentation & Support

| Resource | Link |
|----------|------|
| Installation Guide | [INSTALLATION.md](INSTALLATION.md) |
| Quick Reference | `Process/Prompts/QUICK_REFERENCE.md` |
| Full Documentation | [Main Repository](https://github.com/scooter-indie/author-nonfiction) |
| Issues & Bugs | [Report Issues](https://github.com/scooter-indie/author-nonfiction/issues) |
| Release Notes | [Releases](https://github.com/scooter-indie/author-nonfiction/releases) |

---

## Updating

```bash
cd ~/nonfiction-framework  # or wherever you cloned
git pull origin main
```

Then run `execute configure.md` to apply any migrations.

---

**Version:** 0.15.3 | [Changelog](CHANGELOG.md)
