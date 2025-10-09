# Subagent Customization Template

Use this template to adapt any subagent template to your specific project needs.

**Time to complete**: 10-30 minutes per subagent

**When to use this**: When basic customization isn't enough and you need the subagent to deeply understand your project's unique requirements.

---

## How to Use This Template

1. **Copy this entire template** to your notes
2. **Fill out each section** with your project-specific information
3. **Copy your completed sections** into the corresponding subagent template's "CUSTOMIZE HERE" zone
4. **Test and iterate** - invoke the subagent and refine based on results

---

## Section 1: Project Identity

**Copy this into the subagent template's PROJECT CONTEXT section**

```markdown
## 📋 PROJECT CONTEXT

### Project Overview
**Name**: [Your project name]
**Type**: [Web app / Mobile app / API / CLI tool / Library / etc.]
**Purpose**: [1-2 sentence description of what the project does]
**Stage**: [Early development / Active development / Production / Legacy maintenance]

### Tech Stack
**Language(s)**: [Primary languages: JavaScript, Python, Go, etc.]
**Framework(s)**: [React, Next.js, Django, Express, etc.]
**Database(s)**: [PostgreSQL, MongoDB, Redis, etc.]
**Infrastructure**: [AWS, Docker, Kubernetes, Serverless, etc.]
**Key Libraries**: [List 3-5 most important dependencies]

### Architecture
**Pattern**: [Monolith / Microservices / Serverless / Event-driven / etc.]
**Structure**: [MVC / Clean Architecture / Domain-driven / Feature-based / etc.]
**Data Flow**: [REST API / GraphQL / Event sourcing / CQRS / etc.]
```

---

## Section 2: Codebase Navigation

**Copy this into the subagent template - helps it understand your file structure**

```markdown
### Directory Structure
**Key Directories**:
- `[path]` - [What's here: e.g., "Core business logic"]
- `[path]` - [What's here: e.g., "API endpoints"]
- `[path]` - [What's here: e.g., "Database models"]
- `[path]` - [What's here: e.g., "React components"]
- `[path]` - [What's here: e.g., "Tests"]
- `[path]` - [What's here: e.g., "Configuration files"]

**Important Files**:
- `[file_path]` - [Purpose: e.g., "Main application entry point"]
- `[file_path]` - [Purpose: e.g., "Database schema"]
- `[file_path]` - [Purpose: e.g., "Environment configuration"]

**Naming Conventions**:
- **Files**: [e.g., kebab-case, camelCase, PascalCase]
- **Components**: [e.g., PascalCase, with .component.tsx extension]
- **Tests**: [e.g., *.test.js, *.spec.ts]
- **Constants**: [e.g., UPPER_SNAKE_CASE in constants.js]
```

---

## Section 3: Code Standards & Style

**Copy this into the subagent template - ensures generated code matches your style**

```markdown
### Code Standards
**Style Guide**: [Link to or name of style guide: e.g., Airbnb, Google, internal docs]
**Linter**: [ESLint config, Prettier config, Black, etc.]
**Formatter**: [Prettier, Black, gofmt, etc.]

**Code Style Preferences**:
- **Indentation**: [Spaces or tabs, how many]
- **Quotes**: [Single or double quotes]
- **Semicolons**: [Required or optional]
- **Line Length**: [Max characters per line]
- **Import Order**: [How imports should be organized]

**Language-Specific Conventions**:
[Examples for your language]
- [e.g., "Use functional components with hooks (React)"]
- [e.g., "Prefer async/await over .then() (JavaScript)"]
- [e.g., "Use type hints for all functions (Python)"]
- [e.g., "Follow PEP 8 naming conventions (Python)"]

**Patterns We Use**:
- [e.g., "Repository pattern for data access"]
- [e.g., "Factory pattern for object creation"]
- [e.g., "Observer pattern for event handling"]

**Patterns We Avoid**:
- [e.g., "Don't use singletons"]
- [e.g., "Avoid deep inheritance hierarchies"]
- [e.g., "No God objects"]
```

---

## Section 4: Project-Specific Rules

**Copy this into the subagent template - critical project-specific constraints**

```markdown
### Project Rules & Constraints

**Must Follow**:
1. [Critical rule: e.g., "All API endpoints must have rate limiting"]
2. [Critical rule: e.g., "No direct database queries in controllers"]
3. [Critical rule: e.g., "All user input must be sanitized"]
4. [Add 3-7 non-negotiable rules]

**Should Follow**:
1. [Preference: e.g., "Prefer composition over inheritance"]
2. [Preference: e.g., "Keep functions under 50 lines"]
3. [Preference: e.g., "Write self-documenting code"]
4. [Add 3-5 strong preferences]

**Technology Constraints**:
- [e.g., "Must support Node 18+"]
- [e.g., "Must work in IE11 (legacy requirement)"]
- [e.g., "Cannot use GPL-licensed libraries"]
- [e.g., "Must be GDPR compliant"]

**Performance Requirements**:
- [e.g., "API responses must be under 200ms"]
- [e.g., "Bundle size must stay under 500KB"]
- [e.g., "Support 10K concurrent users"]
```

---

## Section 5: Testing Strategy

**Copy this into the subagent template if it involves testing**

```markdown
### Testing Standards

**Test Framework**: [Jest, Pytest, Go test, etc.]
**Coverage Target**: [Minimum code coverage percentage]
**Test Location**: [Co-located with code or separate test directory]

**Required Tests**:
- [e.g., "Unit tests for all business logic"]
- [e.g., "Integration tests for API endpoints"]
- [e.g., "E2E tests for critical user flows"]

**Test Structure**:
- **Naming**: [e.g., "describe/it format", "test_* functions"]
- **Organization**: [e.g., "Arrange-Act-Assert", "Given-When-Then"]
- **Mocking**: [e.g., "Use jest.mock for external dependencies"]

**What to Test**:
✅ [e.g., "All public APIs"]
✅ [e.g., "Error handling paths"]
✅ [e.g., "Edge cases"]

**What NOT to Test**:
❌ [e.g., "Third-party library internals"]
❌ [e.g., "Simple getters/setters"]
❌ [e.g., "Framework code"]
```

---

## Section 6: Documentation Standards

**Copy this into the subagent template if it involves documentation**

```markdown
### Documentation Requirements

**Code Comments**:
- [When to comment: e.g., "Complex algorithms only"]
- [Format: e.g., "JSDoc for all public functions"]
- [What to explain: e.g., "Why, not what"]

**Documentation Format**:
- [e.g., "Markdown in /docs directory"]
- [e.g., "JSDoc comments for API reference"]
- [e.g., "Inline examples in docstrings"]

**Required Documentation**:
- [e.g., "README for each major module"]
- [e.g., "API documentation for all endpoints"]
- [e.g., "Architecture decision records (ADRs)"]

**Documentation Style**:
- [e.g., "Clear, concise, beginner-friendly"]
- [e.g., "Include code examples"]
- [e.g., "Link to related docs"]
```

---

## Section 7: Integration Points

**Copy this into the subagent template - helps it understand system boundaries**

```markdown
### External Dependencies & APIs

**Third-Party Services**:
- [Service name: e.g., "Stripe for payments"] - [How we use it]
- [Service name: e.g., "SendGrid for email"] - [How we use it]
- [Service name: e.g., "AWS S3 for storage"] - [How we use it]

**Internal APIs/Services**:
- [Service name] at [URL/path] - [What it does]
- [Service name] at [URL/path] - [What it does]

**Authentication/Authorization**:
- **Method**: [e.g., JWT, OAuth2, API keys]
- **Location**: [Where tokens/credentials are stored]
- **Scope**: [What needs auth, what doesn't]

**Environment Variables**:
- **Required**: [List critical env vars]
- **Optional**: [List optional env vars]
- **Location**: [.env file, secrets manager, etc.]
```

---

## Section 8: Error Handling & Logging

**Copy this into the subagent template - ensures proper error handling**

```markdown
### Error Handling Standards

**Error Strategy**:
- [e.g., "Throw exceptions for unrecoverable errors"]
- [e.g., "Return error objects for expected failures"]
- [e.g., "Use Result type for fallible operations"]

**Error Logging**:
- **Logger**: [Winston, Pino, Python logging, etc.]
- **Log Levels**: [When to use DEBUG, INFO, WARN, ERROR]
- **Format**: [JSON, structured, plain text]

**User-Facing Errors**:
- [e.g., "Never expose stack traces to users"]
- [e.g., "Provide actionable error messages"]
- [e.g., "Include error codes for support"]

**Monitoring**:
- [e.g., "Sentry for error tracking"]
- [e.g., "CloudWatch for metrics"]
- [e.g., "DataDog for APM"]
```

---

## Section 9: Workflow Integration

**Copy this into the subagent template - how it fits into your process**

```markdown
### Development Workflow

**Version Control**:
- **Branching**: [Git flow, trunk-based, feature branches, etc.]
- **Branch Naming**: [e.g., feature/*, bugfix/*, hotfix/*]
- **Commits**: [Conventional commits, descriptive messages, etc.]

**CI/CD Pipeline**:
- **Build**: [How code is built]
- **Test**: [What tests run automatically]
- **Deploy**: [Deployment process]

**Code Review Process**:
- [e.g., "At least 2 approvals required"]
- [e.g., "All comments must be resolved"]
- [e.g., "Tests must pass before merge"]

**What This Subagent Should Output**:
- [e.g., "Ready-to-commit code (no WIP)"]
- [e.g., "Include tests with implementation"]
- [e.g., "Update docs in same PR"]
- [e.g., "Follow commit message conventions"]
```

---

## Section 10: Domain-Specific Context

**Copy this into the subagent template - critical business domain knowledge**

```markdown
### Domain Knowledge

**Business Domain**: [e.g., E-commerce, FinTech, Healthcare, SaaS]

**Key Concepts** (terms the subagent should understand):
- **[Term 1]**: [Definition relevant to your project]
- **[Term 2]**: [Definition relevant to your project]
- **[Term 3]**: [Definition relevant to your project]
[Add 5-10 domain-specific terms]

**Business Rules**:
1. [Critical business logic: e.g., "Orders can't be modified after shipping"]
2. [Critical business logic: e.g., "Discounts stack multiplicatively"]
3. [Critical business logic: e.g., "Users must be 18+ to register"]
[Add 3-7 core business rules]

**Edge Cases to Consider**:
- [e.g., "Handle timezone differences for international orders"]
- [e.g., "Account for leap years in subscription billing"]
- [e.g., "Deal with partial refunds"]
```

---

## Section 11: Subagent-Specific Instructions

**Copy this into the subagent template - customize behavior for specific use cases**

```markdown
### Subagent-Specific Configuration

**When invoked, prioritize**:
1. [e.g., "Code readability over performance"]
2. [e.g., "Backward compatibility"]
3. [e.g., "Security over convenience"]

**Output Preferences**:
- **Format**: [How you want results: markdown, code files, diagrams]
- **Detail Level**: [Brief / Detailed / Exhaustive]
- **Examples**: [Include / Don't include code examples]

**Interaction Style**:
- [e.g., "Ask clarifying questions before starting"]
- [e.g., "Propose multiple solutions"]
- [e.g., "Explain trade-offs"]

**Forbidden Actions**:
- [e.g., "Never modify production database files"]
- [e.g., "Don't touch config files without asking"]
- [e.g., "Avoid refactoring working legacy code"]
```

---

## Quick Customization Checklist

Use this to ensure you've covered the essentials:

- [ ] **Section 1**: Project identity filled out
- [ ] **Section 2**: Key directories and files listed
- [ ] **Section 3**: Code style preferences documented
- [ ] **Section 4**: Critical project rules defined
- [ ] **Section 5**: Testing requirements specified (if applicable)
- [ ] **Section 6**: Documentation standards set (if applicable)
- [ ] **Section 7**: External dependencies listed
- [ ] **Section 8**: Error handling strategy defined
- [ ] **Section 9**: Workflow integration clarified
- [ ] **Section 10**: Domain-specific terms explained
- [ ] **Section 11**: Subagent behavior preferences set

---

## Example: Completed Customization

**For a Next.js e-commerce project:**

```markdown
## 📋 PROJECT CONTEXT

### Project Overview
**Name**: ShopFast
**Type**: E-commerce web application
**Purpose**: B2C online marketplace for electronics with real-time inventory
**Stage**: Active development (pre-launch)

### Tech Stack
**Language(s)**: TypeScript
**Framework(s)**: Next.js 14 (App Router), React 18
**Database(s)**: PostgreSQL (main), Redis (cache)
**Infrastructure**: Vercel (hosting), AWS S3 (images), Stripe (payments)
**Key Libraries**: Prisma, TailwindCSS, React Query, Zustand

### Architecture
**Pattern**: Monolith with serverless functions
**Structure**: Feature-based (domains: products, cart, orders, users)
**Data Flow**: REST API with tRPC for type-safe internal APIs

### Directory Structure
**Key Directories**:
- `src/app` - Next.js App Router pages and layouts
- `src/features` - Feature modules (products, cart, checkout)
- `src/lib` - Shared utilities and database client
- `src/components` - Reusable React components
- `src/server` - tRPC routers and business logic
- `prisma` - Database schema and migrations

**Naming Conventions**:
- **Files**: kebab-case for pages, PascalCase for components
- **Components**: PascalCase with .tsx extension
- **Tests**: *.test.tsx co-located with components

### Code Standards
**Style Guide**: Internal (documented in CONTRIBUTING.md)
**Linter**: ESLint with Next.js config + custom rules
**Formatter**: Prettier (2 spaces, single quotes)

**Code Style Preferences**:
- Use functional components with hooks
- Prefer server components over client components
- Extract complex logic into custom hooks
- Keep components under 200 lines

**Patterns We Use**:
- Repository pattern for database access
- Custom hooks for shared logic
- Compound components for complex UI

### Project Rules & Constraints
**Must Follow**:
1. All data mutations must go through tRPC procedures
2. Server components by default, use 'use client' only when needed
3. All prices stored as integers (cents) to avoid floating-point errors
4. Images must use Next.js Image component for optimization

**Performance Requirements**:
- Lighthouse score 90+ on all pages
- LCP under 2.5s
- Bundle size under 300KB (excluding images)

### Domain Knowledge
**Business Domain**: E-commerce (consumer electronics)

**Key Concepts**:
- **SKU**: Stock Keeping Unit - unique product identifier
- **Cart abandonment**: User adds items but doesn't complete purchase
- **Inventory sync**: Real-time stock updates across sessions

**Business Rules**:
1. Orders can't be modified after payment confirmation
2. Stock is reserved for 15 minutes during checkout
3. Discounts apply before tax calculation
```

---

## Tips for Effective Customization

1. **Start minimal**: Fill out Sections 1-4 first, add others as needed
2. **Be specific**: "Use React hooks" is better than "Write modern code"
3. **Include examples**: Show don't tell - paste actual code snippets
4. **Update iteratively**: Refine based on subagent output quality
5. **Keep it current**: Update as your project evolves
6. **Don't over-constrain**: Leave room for subagent creativity
7. **Test after customizing**: Invoke the subagent to verify it understands context

---

## What to Do After Customizing

1. **Copy relevant sections** into your chosen subagent template's PROJECT CONTEXT area
2. **Save your customization** (you can reuse it for other subagents)
3. **Test the subagent** with a real task
4. **Iterate**: Refine customization based on output quality
5. **Share with team**: Commit customized templates to version control

---

**Ready to build your own subagent?** → See `templates/EXAMPLE_TEMPLATE.md` for template structure
