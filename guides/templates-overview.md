# Claude Code Subagent Templates

Production-ready subagent templates for Claude Code projects.

## Available Templates

### 1. code-architect.md
**Purpose**: System design, architecture decisions, technical planning

**Use for**:
- Designing new features or systems
- Planning large refactors
- Making architectural decisions
- Evaluating technical approaches

**Invoke**: `"Use the code-architect subagent to design [feature]"`

---

### 2. refactor-specialist.md *(Coming Soon)*
**Purpose**: Code optimization, refactoring, technical debt reduction

**Use for**:
- Improving code quality
- Reducing complexity
- Optimizing performance
- Modernizing legacy code

---

### 3. test-engineer.md *(Coming Soon)*
**Purpose**: Test generation, coverage analysis, test strategy

**Use for**:
- Writing unit tests
- Creating integration tests
- Improving test coverage
- Designing test strategies

---

### 4. debug-detective.md *(Coming Soon)*
**Purpose**: Bug investigation, root cause analysis, debugging

**Use for**:
- Finding the source of bugs
- Understanding error traces
- Investigating weird behavior
- Analyzing production issues

---

### 5. docs-writer.md *(Coming Soon)*
**Purpose**: Documentation generation, technical writing

**Use for**:
- Writing READMEs
- Documenting APIs
- Creating guides
- Generating code comments

---

### 6. security-auditor.md *(Coming Soon)*
**Purpose**: Security review, vulnerability detection, defensive analysis

**Use for**:
- Reviewing code for security issues
- Checking for common vulnerabilities
- Auditing authentication/authorization
- Validating input sanitization

---

## How to Use These Templates

### Quick Start (No Customization)

1. **Copy template to your project**:
   ```bash
   cp templates/code-architect.md /your-project/.claude/subagents/
   ```

2. **Invoke in Claude Code**:
   ```
   "Use the code-architect subagent to design a user authentication system"
   ```

3. **Done!** The template works out-of-the-box.

### Customized Setup (Recommended)

1. **Copy template to your project**:
   ```bash
   cp templates/code-architect.md /your-project/.claude/subagents/
   ```

2. **Open the template** and find the `PROJECT CONTEXT - CUSTOMIZE HERE` section at the top

3. **Fill out your project details**:
   - Project overview (name, type, purpose)
   - Tech stack (languages, frameworks, databases)
   - Key directories and files
   - Code standards and patterns
   - Project-specific rules

4. **Save and invoke**:
   ```
   "Use the code-architect subagent to design a user authentication system"
   ```

Now it understands YOUR codebase!

---

## Template Structure

Every template follows this structure:

```
┌─────────────────────────────────────────┐
│ 📋 PROJECT CONTEXT                      │
│ ✏️ CUSTOMIZE THIS SECTION              │
│                                         │
│ - Project overview                      │
│ - Tech stack                            │
│ - Directory structure                   │
│ - Code standards                        │
│ - Project rules                         │
└─────────────────────────────────────────┘
         ↓
┌─────────────────────────────────────────┐
│ 🏗️ CORE CAPABILITIES                    │
│ ⚠️ DON'T MODIFY                         │
│                                         │
│ - What this subagent does               │
│ - Its expertise areas                   │
│ - Its responsibilities                  │
└─────────────────────────────────────────┘
         ↓
┌─────────────────────────────────────────┐
│ 🔄 WORKFLOW                              │
│ ⚠️ DON'T MODIFY                         │
│                                         │
│ - Step-by-step process                  │
│ - How it operates                       │
│ - Quality checks                        │
└─────────────────────────────────────────┘
         ↓
┌─────────────────────────────────────────┐
│ 📤 OUTPUT FORMAT                         │
│ ⚠️ DON'T MODIFY                         │
│                                         │
│ - Standardized output structure         │
│ - What you'll get back                  │
│ - Consistent formatting                 │
└─────────────────────────────────────────┘
```

**Only customize the PROJECT CONTEXT section** - the rest is battle-tested subagent logic.

---

## Customization Guide

### Level 1: Zero Config (0 minutes)
Use as-is. Templates work immediately but won't know your project specifics.

**Good for**: Quick experiments, one-off tasks

### Level 2: Basic Config (5 minutes)
Fill out the PROJECT CONTEXT section with:
- Project name and type
- Tech stack
- Key directories
- Basic rules

**Good for**: Most use cases, regular project work

### Level 3: Deep Config (15-30 minutes)
Use `SUBAGENT_CUSTOMIZATION_TEMPLATE.md` to fill out:
- Detailed code standards
- Testing requirements
- Documentation preferences
- Domain-specific knowledge
- Error handling patterns
- Workflow integration

**Good for**: Complex projects, team use, long-term maintenance

---

## Detailed Customization

For detailed customization instructions, see:
- **`SUBAGENT_CUSTOMIZATION_TEMPLATE.md`** - Complete customization guide with 11 sections
- **`QUICK_START.md`** - 5-minute setup guide

---

## Creating Your Own Templates

Want to build a custom subagent? Use this structure:

1. **Copy `code-architect.md`** as a starting point
2. **Modify the CORE CAPABILITIES** section to match your subagent's purpose
3. **Adjust the WORKFLOW** for your specific process
4. **Customize the OUTPUT FORMAT** for what you want back
5. **Keep the PROJECT CONTEXT structure** - it's reusable across all subagents

**Key principles**:
- ✅ Keep PROJECT CONTEXT standardized (users can reuse across templates)
- ✅ Make capabilities clear and focused
- ✅ Define a structured workflow
- ✅ Specify concrete output format
- ✅ Include usage examples

---

## Tips for Effective Use

1. **Start simple**: Use templates without customization first
2. **Customize incrementally**: Add project details as you use them
3. **Reuse context**: Copy your PROJECT CONTEXT to other templates
4. **Chain subagents**: Use architect → refactor → test in sequence
5. **Version control**: Commit customized templates to your repo
6. **Team alignment**: Share customizations with your team
7. **Update regularly**: Keep PROJECT CONTEXT current as project evolves

---

## Template Maintenance

**When to update templates**:
- Project structure changes (new directories, different organization)
- Tech stack updates (framework upgrades, new libraries)
- Pattern changes (new coding standards, different architectures)
- Team growth (new conventions, style guide updates)

**How to update**:
1. Open the template in `.claude/subagents/`
2. Update only the PROJECT CONTEXT section
3. Test with a simple invocation
4. Commit changes to version control

---

## Invocation Patterns

### Single Subagent
```
"Use the code-architect subagent to design a caching layer"
```

### Sequential Subagents
```
"First use code-architect to design authentication,
then use test-engineer to create a test plan"
```

### Parallel Subagents (if you have multiple tasks)
```
"Use debug-detective to investigate the login bug
while also using docs-writer to update the API documentation"
```

---

## Troubleshooting

### Subagent not responding as expected?
1. Check that the template file is in `.claude/subagents/` directory
2. Verify markdown formatting is correct
3. Ensure you're using the correct subagent name when invoking

### Output quality issues?
1. Fill out more of the PROJECT CONTEXT section
2. Add project-specific rules and constraints
3. Include examples of your code style in PROJECT CONTEXT

### Subagent ignoring project rules?
1. Make rules more specific in PROJECT CONTEXT
2. Add examples showing what to do/avoid
3. Mark critical rules as "Must Follow" vs "Should Follow"

---

## Contributing Templates

Have a great subagent template? Here's how to share it:

1. **Follow the standard structure** (PROJECT CONTEXT → CAPABILITIES → WORKFLOW → OUTPUT)
2. **Include clear documentation** (purpose, use cases, examples)
3. **Test thoroughly** on multiple projects
4. **Add usage examples** showing real invocations
5. **Submit a pull request** with your template

**Good template ideas**:
- API designer
- Database schema planner
- Performance optimizer
- Migration planner
- Code reviewer
- Dependency updater
- CI/CD configurator

---

## Examples Directory

See `examples/` directory (coming soon) for:
- Fully customized templates for different project types
- Real-world usage examples
- Before/after comparisons
- Team customization strategies

---

## Support

**Issues or questions?**
- Open an issue in this repository
- Check `QUICK_START.md` for basic setup
- See `SUBAGENT_CUSTOMIZATION_TEMPLATE.md` for detailed configuration

---

## License

[Your license here]

---

**Ready to start?** → See `QUICK_START.md`

**Need customization help?** → See `SUBAGENT_CUSTOMIZATION_TEMPLATE.md`

**Want to contribute?** → Submit a PR with your template
