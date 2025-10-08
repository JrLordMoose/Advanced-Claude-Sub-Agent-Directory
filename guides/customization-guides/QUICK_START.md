# 5-Minute Setup Guide - Session Documentation Agent

Get the Session Documentation Specialist Agent configured for your project in under 5 minutes.

---

## Step 1: Configure Paths (2 minutes)

Open the main template file and find the **📐 PROJECT CONFIGURATION** section at the top.

Replace these placeholders with your actual values:

```yaml
# Directory Paths
session_docs_path: "docs/sessions/"              # Where session docs are saved
session_index_file: "docs/sessions/INDEX.md"     # Session index location
project_root: "./"                               # Project root directory
```

### Common Configurations by Project Type

**Web Application (React/Next.js/Vue):**
```yaml
session_docs_path: "docs/sessions/"
session_index_file: "docs/sessions/INDEX.md"
project_root: "./"
```

**Mobile Application (iOS/Android):**
```yaml
session_docs_path: "documentation/dev-sessions/"
session_index_file: "documentation/dev-sessions/INDEX.md"
project_root: "./"
```

**Desktop Application (.NET/Electron):**
```yaml
session_docs_path: "docs/development/sessions/"
session_index_file: "docs/development/sessions/INDEX.md"
project_root: "./"
```

**API/Backend (Node.js/Python/Go):**
```yaml
session_docs_path: "docs/sessions/"
session_index_file: "docs/sessions/INDEX.md"
project_root: "./"
```

**Data Science Project:**
```yaml
session_docs_path: "notebooks/session-docs/"
session_index_file: "notebooks/session-docs/INDEX.md"
project_root: "./"
```

---

## Step 2: Set Project Type (1 minute)

Choose your project type to automatically load the correct testing checklist:

```yaml
project_type: "web"  # Options: web | mobile | desktop | api | data-science | game
```

This determines which testing checklist appears in generated session docs.

---

## Step 3: Set Tech Stack (1 minute)

Configure your primary language and framework:

```yaml
code_language: "javascript"   # Your primary programming language
framework: "react"            # Your framework (optional, leave blank if N/A)
default_branch: "main"        # Your git default branch (main/master/develop)
commit_style: "conventional"  # conventional | descriptive | ticket-based
```

**Common Configurations:**

| Stack | code_language | framework |
|-------|---------------|-----------|
| React | javascript | react |
| Next.js | javascript | nextjs |
| Vue | javascript | vue |
| Angular | typescript | angular |
| iOS (Swift) | swift | swiftui |
| Android (Kotlin) | kotlin | jetpack-compose |
| .NET Desktop | csharp | wpf |
| Django | python | django |
| FastAPI | python | fastapi |
| Node.js API | javascript | express |

---

## Step 4: Create Session Directories (30 seconds)

Run these commands in your project root:

```bash
# Create session docs directory
mkdir -p docs/sessions/

# Create empty index file
touch docs/sessions/INDEX.md

# Initialize index with header
echo "# Session Index" > docs/sessions/INDEX.md
echo "" >> docs/sessions/INDEX.md
echo "**Total Sessions:** 0" >> docs/sessions/INDEX.md
```

**Or use your configured paths:**
```bash
mkdir -p {your_session_docs_path}
touch {your_session_index_file}
```

---

## Step 5: Find/Replace Placeholders (1 minute)

Use your text editor's Find/Replace feature (usually Ctrl+H or Cmd+H):

### Replacements Needed:

| Find This | Replace With | Example |
|-----------|--------------|---------|
| `{session_docs_path}` | Your actual path | `docs/sessions/` |
| `{session_index_file}` | Your actual path | `docs/sessions/INDEX.md` |
| `{project_root}` | Your actual root | `./` |
| `{code_language}` | Your language | `javascript` |
| `{framework}` | Your framework | `react` |
| `{default_branch}` | Your branch | `main` |

### Quick Find/Replace in VS Code:
1. Press `Ctrl+H` (Cmd+H on Mac)
2. Enable "Use Regular Expression" (.*) icon
3. Find: `\{(\w+)\}`
4. Replace one by one with your values

### Quick Find/Replace via Command Line:
```bash
# macOS/Linux
sed -i 's|{session_docs_path}|docs/sessions/|g' "Session Documentation Specialist Sub-Agent Universal Template.md"
sed -i 's|{session_index_file}|docs/sessions/INDEX.md|g' "Session Documentation Specialist Sub-Agent Universal Template.md"
sed -i 's|{project_root}|./|g' "Session Documentation Specialist Sub-Agent Universal Template.md"

# Windows (PowerShell)
(Get-Content "Session Documentation Specialist Sub-Agent Universal Template.md") -replace '\{session_docs_path\}', 'docs/sessions/' | Set-Content "Session Documentation Specialist Sub-Agent Universal Template.md"
```

---

## Step 6: Test the Agent (30 seconds)

Invoke the agent in Claude Code:

```
Create test session documentation for setup verification
```

**Expected Output:**
- Markdown file created at `{session_docs_path}/Session_01_Test_Setup.md`
- Quick Resume section with 3-5 bullets
- File change manifest
- Git activity section
- Next steps section

If successful, you're ready to use it for real sessions!

---

## Alternative: Use Pre-Configured Template (Zero Config)

Instead of universal template, copy a pre-configured one:

### Web Application
```bash
cp templates/session-documentation/session-doc-web.md .claude/agents/session-doc-agent.md
```
- Paths: `docs/sessions/`
- Testing: Browser testing enabled
- Examples: React/Next.js

### Mobile Application
```bash
cp templates/session-documentation/session-doc-mobile.md .claude/agents/session-doc-agent.md
```
- Paths: `documentation/dev-sessions/`
- Testing: iOS/Android testing enabled
- Examples: Swift/Kotlin

### Desktop Application
```bash
cp templates/session-documentation/session-doc-desktop.md .claude/agents/session-doc-agent.md
```
- Paths: `docs/development/sessions/`
- Testing: Windows/macOS/Linux testing enabled
- Examples: C#/.NET/Electron

### API/Backend
```bash
cp templates/session-documentation/session-doc-api.md .claude/agents/session-doc-agent.md
```
- Paths: `docs/sessions/`
- Testing: API testing enabled
- Examples: Node.js/Python/Go

### Data Science
```bash
cp templates/session-documentation/session-doc-data-science.md .claude/agents/session-doc-agent.md
```
- Paths: `notebooks/session-docs/`
- Testing: Data pipeline testing enabled
- Examples: Python/Jupyter

---

## Troubleshooting

### Issue: "Can't find session docs directory"
**Solution:** Make sure you created the directory (Step 4) and updated paths correctly (Step 1)

### Issue: "Placeholders still showing in output"
**Solution:** Run Find/Replace again (Step 5) - you may have missed some

### Issue: "Wrong testing checklist showing"
**Solution:** Check `project_type` in config (Step 2) - should match your project

### Issue: "Agent not saving to correct location"
**Solution:** Verify `session_docs_path` is absolute or relative to project root

---

## Next Steps

1. **Use it:** Invoke at end of every work session
2. **Refine it:** Adjust config based on your workflow
3. **Share it:** Commit customized template to your repo for team use
4. **Automate it:** Set up hooks to auto-invoke after commits

---

## Usage Example

**At end of coding session:**
```
Create session documentation for today's work
```

**Agent will:**
1. Analyze conversation for accomplishments
2. Extract file changes and line numbers
3. Run git commands to detect commits
4. Document technical decisions
5. Create Quick Resume section
6. Update Session Index
7. Save to `{session_docs_path}/Session_XX_Title.md`

**Time:** 2-5 minutes

**Benefit:** 80% faster context resumption in future sessions

---

**Setup complete!** Start documenting your sessions.
