# General Purpose Agents

**Versatile agents for common development workflows**

## Overview

This directory contains general-purpose agents that can be used across different project types and development scenarios. These agents focus on specific development tasks rather than specialized domains.

## Files in This Directory

- **code-architect.md** - Software architecture and system design agent

## Code Architect Agent

### Overview

The Code Architect Agent helps you design and plan software architecture, make technical decisions, and structure your codebase for scalability and maintainability.

### Key Features

✅ **System Design** - Architecture patterns, component design, data flow
✅ **Technical Decision Making** - Evaluate technology choices with trade-offs
✅ **Code Structure Planning** - Directory structure, module organization
✅ **Scalability Planning** - Design for growth and performance
✅ **Best Practices** - Industry-standard patterns and conventions
✅ **Documentation** - Architecture diagrams, decision records

### Quick Start

```bash
# Copy to your project's .claude/agents/ directory
cp code-architect.md /path/to/your/project/.claude/agents/
```

### Common Use Cases

#### 1. Design System Architecture

```
Design a microservices architecture for an e-commerce platform
```

**Agent will:**
- Propose service boundaries (user service, product service, order service, etc.)
- Design inter-service communication (REST, gRPC, message queues)
- Plan data storage strategy (databases per service, caching)
- Consider scalability and fault tolerance
- Provide architecture diagram
- Document technical decisions

#### 2. Evaluate Technology Choices

```
Should we use PostgreSQL or MongoDB for this project?
```

**Agent will:**
- Analyze project requirements
- Compare both options with pros/cons
- Consider data structure, query patterns, scalability
- Evaluate team expertise and ecosystem
- Provide recommendation with rationale
- Suggest migration path if switching

#### 3. Plan Code Structure

```
Organize this React application for scalability
```

**Agent will:**
- Propose directory structure (features, components, utils, hooks)
- Suggest module boundaries and separation of concerns
- Plan state management approach
- Design routing structure
- Consider code splitting and lazy loading
- Provide examples and guidelines

#### 4. Refactoring Strategy

```
Plan refactoring of monolithic app to modular architecture
```

**Agent will:**
- Analyze current architecture
- Identify module boundaries
- Propose phased refactoring approach
- Design module interfaces
- Plan data migration
- Minimize disruption to existing functionality

### Design Patterns Supported

**Architectural Patterns:**
- Microservices
- Monolithic
- Serverless
- Event-Driven
- Layered (N-Tier)
- Hexagonal (Ports & Adapters)
- CQRS (Command Query Responsibility Segregation)

**Design Patterns:**
- Creational: Singleton, Factory, Builder, Prototype
- Structural: Adapter, Decorator, Facade, Proxy
- Behavioral: Observer, Strategy, Command, State

**Frontend Patterns:**
- Component Composition
- Container/Presentation
- Higher-Order Components
- Render Props
- Hooks Patterns
- State Management (Redux, MobX, Context API)

**Backend Patterns:**
- Repository Pattern
- Service Layer
- Dependency Injection
- Middleware Pattern
- Circuit Breaker
- Saga Pattern

### Output Format

#### Architecture Design Document

```markdown
# Architecture Design: [Feature/System Name]

## Overview
[High-level description of the system]

## Requirements
[Functional and non-functional requirements]

## Architecture Diagram
[Mermaid diagram or description]

## Components
### Component 1
- Responsibility: [what it does]
- Dependencies: [what it depends on]
- Technology: [language, framework, database]
- API: [endpoints, methods, data structures]

### Component 2
[Similar structure]

## Data Model
[Database schema, entity relationships]

## Technology Stack
- Frontend: [framework, libraries]
- Backend: [language, framework]
- Database: [type, justification]
- Infrastructure: [hosting, CI/CD, monitoring]

## Technical Decisions
### Decision 1: [Topic]
- Context: [why this decision is needed]
- Options Considered: [alternatives]
- Decision: [chosen approach]
- Rationale: [why this was chosen]
- Consequences: [trade-offs, implications]

## Scalability Considerations
[How the system scales, bottlenecks, mitigation strategies]

## Security Considerations
[Authentication, authorization, data protection, vulnerabilities]

## Testing Strategy
[Unit tests, integration tests, E2E tests]

## Deployment Strategy
[CI/CD pipeline, environments, rollback plans]

## Monitoring & Observability
[Logging, metrics, alerting, tracing]

## Future Enhancements
[Planned improvements, technical debt]
```

### Benefits

#### For Solo Developers
- **Think through design** before coding
- **Avoid costly refactors** with upfront planning
- **Learn best practices** through guided decision-making
- **Document decisions** for future reference

#### For Teams
- **Shared understanding** of system architecture
- **Consistent patterns** across the codebase
- **Knowledge transfer** through architecture docs
- **Aligned technical decisions** with recorded rationale

#### For Technical Leaders
- **Communicate architecture** to stakeholders
- **Evaluate technical debt** and refactoring needs
- **Plan roadmap** with architectural implications
- **Mentor developers** with architecture guidance

### Configuration

The Code Architect agent can be customized for:

- **Project Type** - Web, mobile, desktop, API, data pipeline, embedded
- **Scale** - Startup MVP, small team, enterprise
- **Tech Stack** - Language, framework, database preferences
- **Team Size** - Solo, small team, large team
- **Industry** - SaaS, e-commerce, fintech, healthcare, etc.

### Usage Tips

**Best Practices:**
- Invoke early in the feature development cycle
- Provide context about requirements and constraints
- Ask about trade-offs between different approaches
- Request diagrams for complex architectures
- Document decisions in your codebase

**Example Invocations:**
```
Design authentication system with OAuth and JWT
Plan database schema for multi-tenant SaaS app
Evaluate GraphQL vs REST API for mobile app
Design CI/CD pipeline for microservices deployment
Plan migration from monolith to microservices
```

### Integration with Other Agents

The Code Architect agent works well with:

- **Session Documentation** - Document architecture decisions in session docs
- **SEO Specialist** - Plan technical SEO architecture
- **UX/UI Designer** - Align frontend architecture with design system

Workflow example:
```
1. Use Code Architect to design feature architecture
2. Implement the feature following the architecture plan
3. Use Session Documentation to record the implementation
4. Reference architecture in future sessions
```

## Coming Soon

Additional general-purpose agents planned:

- **Debug Detective** - Systematic debugging and troubleshooting
- **Test Engineer** - Test strategy, test generation, coverage analysis
- **Performance Optimizer** - Performance profiling and optimization
- **Security Auditor** - Security best practices and vulnerability scanning
- **Refactoring Specialist** - Code refactoring patterns and strategies
- **Documentation Writer** - README, API docs, code comments

## Version

**v1.0** - Code Architect Agent
**Pattern Support:** 20+ architecture and design patterns
**Project Types:** All

## Additional Resources

- **[Main Repository README](../../README.md)** - Overview of all available agents
- **[Customization Guide](../../guides/SUBAGENT_CUSTOMIZATION_TEMPLATE.md)** - How to customize any agent
- **[Quick Start](../../QUICK_START.md)** - General agent setup guide

## Support

**Questions or issues?**
- Review the agent template for detailed usage instructions
- Open an issue in the repository

---

**Ready to architect?** Copy the code-architect.md file to your project and start planning your next feature.
