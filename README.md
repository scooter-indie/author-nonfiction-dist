# AI-Assisted Nonfiction Authoring Framework

**Distribution Repository** - Clone this repo to start writing your nonfiction book with AI assistance.

---

## Quick Start (Claude Code CLI)

**Recommended method** - Full automation with git integration.

```bash
# 1. Clone the framework
git clone https://github.com/scooter-indie/author-nonfiction-dist.git my-book
cd my-book

# 2. Start Claude Code
claude

# 3. Configure the framework (say this in Claude Code)
execute configure.md

# 4. Initialize your book (say this in Claude Code)
execute Prompt 1
```

After setup, start each session with:
```
/fw-init
```

---

## Alternative: Claude Desktop

If you prefer Claude Desktop over the CLI:

### Step 1: Clone and Open

```bash
git clone https://github.com/scooter-indie/author-nonfiction-dist.git my-book
```

### Step 2: Configure System Instructions

1. Open Claude Desktop
2. Go to **Settings** → **Custom Instructions**
3. Open `system-instructions.md` from your cloned directory
4. Copy everything between the `---SYSTEM INSTRUCTIONS---` markers (lines 40-356)
5. Paste into Claude Desktop's Custom Instructions field
6. Save and **start a new chat**

### Step 3: Run Configuration

In your new Claude Desktop chat, say:
```
execute configure.md
```

Follow the prompts. When git commands are needed, Claude will provide commands to run in Claude Code CLI.

### Step 4: Initialize Your Book

```
execute Prompt 1
```

---

## Documentation & Support

| Resource | Link |
|----------|------|
| Full Documentation | [Main Repository](https://github.com/scooter-indie/author-nonfiction) |
| Issues & Bugs | [Report Issues](https://github.com/scooter-indie/author-nonfiction/issues) |
| Release Notes | [Releases](https://github.com/scooter-indie/author-nonfiction/releases) |
| Installation Guide | [INSTALLATION.md](INSTALLATION.md) |

---

## Updating the Framework

```bash
git pull origin main
```

Then run `execute configure.md` to apply any migrations.

---

**Version:** 0.15.1 | [Changelog](CHANGELOG.md)
