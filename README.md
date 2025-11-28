# AI-Assisted Nonfiction Authoring Framework

**Distribution Repository** - Clone this repo to start writing nonfiction books with AI assistance.

---

## Quick Start (v0.16.0+)

### 1. Clone the Framework

```bash
git clone https://github.com/scooter-indie/author-nonfiction-dist.git ~/Downloads/author-nonfiction
```

### 2. Run Setup Script

**Windows:**
```batch
cd %USERPROFILE%\Downloads\author-nonfiction
configure.bat
```

**macOS/Linux:**
```bash
cd ~/Downloads/author-nonfiction
./configure.sh
```

### 3. Follow Setup Prompts

The setup will:
- Ask where to create your PROJECT_ROOT (writing environment)
- Create the unified directory structure
- Initialize git repository
- Chain to start-authoring automatically

### 4. Create Your First Book

After setup completes, say: `Execute Prompt 1`

---

## Architecture (v0.16.0+)

```
PROJECT_ROOT/
├── FW_ROOT/              # Framework (cloned, gitignored)
├── BOOKS_ROOT/           # Your books
│   ├── [Book-Name]/
│   └── Archive/
├── .config/              # Configuration
├── start-authoring.*     # Startup scripts
└── .gitignore
```

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

Start sessions with the startup script:
- **Windows:** `start-authoring.bat` from PROJECT_ROOT
- **macOS/Linux:** `./start-authoring.sh` from PROJECT_ROOT

Common commands:
```
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

Framework updates are checked automatically on `/fw-init`. To update manually:

```bash
cd PROJECT_ROOT/FW_ROOT
git pull origin main
```

Then run `/fw-init` to apply any migrations.

---

**Version:** 0.16.0 | [Changelog](CHANGELOG.md)
