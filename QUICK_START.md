# Quick Start Guide - Claude Code Subagent Templates

Get advanced subagents running in your project in under 5 minutes.

## What Are These Templates?

Pre-built, specialized Claude Code subagents that handle complex workflows autonomously. Think of them as expert team members you can invoke on-demand.

## 3-Step Setup

### 1. Copy Templates to Your Project (30 seconds)

```bash
# Copy the templates directory to your project root
cp -r templates/ /path/to/your/project/.claude/subagents/
```

Or manually create: `.claude/subagents/` in your project root and copy template files there.

### 2. Test a Template Immediately (1 minute)

Templates work out-of-the-box. Try one:

```bash
# In Claude Code, invoke a subagent:
"Use the code-architect subagent to design a user authentication system"
```

The template will analyze your codebase and provide architecture recommendations.

### 3. Customize for Your Project (3 minutes)

Each template has a `CUSTOMIZE HERE` section at the top. Update it with your project details:

```markdown
## 📋 PROJECT CONTEXT - CUSTOMIZE HERE

**Tech Stack**: [Your stack: React, Node.js, PostgreSQL, etc.]
**Architecture**: [Your architecture: Microservices, Monolith, etc.]
**Code Style**: [Your conventions: ESLint config, formatting rules, etc.]
**Key Directories**: [Your structure: src/, lib/, components/, etc.]
```

## Available Templates

| Template | Use Case | Invoke With |
|----------|----------|-------------|
| **code-architect** | System design, architecture decisions | "Use code-architect to design..." |
| **refactor-specialist** | Code refactoring, optimization | "Use refactor-specialist to improve..." |
| **test-engineer** | Test generation, coverage analysis | "Use test-engineer to test..." |
| **debug-detective** | Bug investigation, root cause analysis | "Use debug-detective to find..." |
| **docs-writer** | Documentation generation | "Use docs-writer to document..." |
| **security-auditor** | Security review, vulnerability scanning | "Use security-auditor to audit..." |

## How to Invoke Subagents

In Claude Code, use natural language:

```
"Use the [template-name] subagent to [your task]"
```

**Examples:**
- "Use the code-architect subagent to design a caching layer"
- "Use the refactor-specialist to optimize the UserService class"
- "Use the test-engineer to add tests for the authentication module"

## Customization Levels

### Level 1: Zero Config (Works Immediately)
Use templates as-is. They'll analyze your project on the fly.

### Level 2: Basic Config (5 minutes)
Fill out the `CUSTOMIZE HERE` section with your project basics.

### Level 3: Advanced Config (15-30 minutes)
Use `SUBAGENT_CUSTOMIZATION_TEMPLATE.md` to deeply customize behavior, add project-specific rules, and integrate with your workflows.

## Need More Control?

See `SUBAGENT_CUSTOMIZATION_TEMPLATE.md` for the complete customization guide.

## Template Structure

Each template follows this pattern:

```
┌─────────────────────────────────────┐
│ PROJECT CONTEXT (your customization)│
├─────────────────────────────────────┤
│ CORE CAPABILITIES (template logic)  │
├─────────────────────────────────────┤
│ WORKFLOW (how it operates)          │
├─────────────────────────────────────┤
│ OUTPUT FORMAT (what you get back)   │
└─────────────────────────────────────┘
```

Only customize the PROJECT CONTEXT section to start. Leave the rest as-is.

## Tips

- **Start with zero config**: Templates work immediately
- **Customize incrementally**: Add project details over time as needed
- **Invoke frequently**: Subagents are designed for repeated use
- **Chain subagents**: Use code-architect, then refactor-specialist, then test-engineer in sequence
- **Read outputs carefully**: Subagents return detailed reports with file paths and line numbers

## Troubleshooting

**Subagent not working?**
- Ensure the template is in `.claude/subagents/` directory
- Check that the file has proper markdown formatting
- Verify you're using the correct subagent name when invoking

**Want to modify behavior?**
- See `SUBAGENT_CUSTOMIZATION_TEMPLATE.md` for detailed guidance
- Each template has inline comments showing what's safe to change

## Next Steps

1. Copy templates to your project
2. Try one immediately (zero config)
3. Customize as you use them
4. Create your own using the templates as examples

---

**Ready to customize?** → See `SUBAGENT_CUSTOMIZATION_TEMPLATE.md`

**Want to build your own?** → See `templates/EXAMPLE_TEMPLATE.md`
