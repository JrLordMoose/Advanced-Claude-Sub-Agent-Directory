# UX/UI Design Expert Agent

**Comprehensive UX/UI design agent for Claude Code - Create user-centered designs with conversion optimization**

## Overview

The UX/UI Design Expert Agent helps you audit, design, and optimize user interfaces with a focus on mobile-first design, accessibility, and conversion optimization. Perfect for designers, developers, and product teams building user-facing applications.

## Key Features

✅ **Mobile-First Design Framework** - Progressive enhancement from mobile to desktop
✅ **Comprehensive Accessibility** - WCAG 2.1 AA/AAA compliance guidance
✅ **Conversion Optimization** - CTA design, landing page optimization, A/B testing
✅ **Design System Integration** - Component libraries, design tokens, style guides
✅ **Interactive Prototyping** - Figma/Sketch mockups with specifications
✅ **User Research Integration** - Persona-driven design decisions
✅ **Performance-Aware Design** - Optimize for Core Web Vitals

## Files in This Directory

- **Universal UX-UI Designer Agent Template for GitHub.md** - The main agent template (2700+ lines)

## Quick Start

### Step 1: Install the Agent

```bash
# Copy to your project's .claude/agents/ directory
cp "Universal UX-UI Designer Agent Template for GitHub.md" /path/to/your/project/.claude/agents/ux-ui-designer.md
```

### Step 2: Configure (2 minutes)

Open the file and update the `PROJECT CONFIGURATION` section:

```yaml
# Project Context
product_name: "[YOUR_PRODUCT_NAME]"
product_type: "[YOUR_PRODUCT_TYPE]"              # e.g., SaaS, E-commerce, Mobile App
target_audience: "[TARGET_AUDIENCE]"             # e.g., "B2B professionals", "E-commerce shoppers"

# Design Paths
designs_path: "designs/"                         # Where design mockups are saved
components_path: "src/components/"               # Where UI components live
styles_path: "src/styles/"                       # Where stylesheets live

# Design System
design_system: "material"                        # material | bootstrap | tailwind | custom
primary_color: "#007bff"
secondary_color: "#6c757d"

# Accessibility
wcag_level: "AA"                                 # A | AA | AAA
```

### Step 3: Find/Replace Placeholders (1 minute)

Use your editor's Find/Replace (Ctrl+H or Cmd+H):

| Find | Replace |
|------|---------|
| `[YOUR_PRODUCT_NAME]` | `YourApp` |
| `[YOUR_PRODUCT_TYPE]` | `SaaS Dashboard` |
| `[TARGET_AUDIENCE]` | `B2B professionals` |
| `{designs_path}` | `designs/` |
| `{components_path}` | `src/components/` |

### Step 4: Test

Invoke the agent in Claude Code:

```
Audit the homepage for UX/UI best practices
```

## What the Agent Does

### UI/UX Audits
- **Design Consistency** - Check alignment, spacing, typography, colors
- **Accessibility** - WCAG compliance, keyboard navigation, screen readers
- **Mobile Responsiveness** - Breakpoints, touch targets, mobile patterns
- **Conversion Optimization** - CTA placement, visual hierarchy, friction points
- **Performance Impact** - Image optimization, layout shifts, font loading

### Design Creation
- **Component Design** - Buttons, forms, cards, navigation, modals
- **Layout Design** - Grid systems, spacing, alignment, responsive breakpoints
- **Color Systems** - Primary/secondary colors, semantic colors, accessibility contrast
- **Typography** - Font pairing, hierarchy, readability, responsive scaling
- **Iconography** - Icon selection, sizing, accessibility labels

### Design Systems
- **Component Libraries** - Reusable UI components with variants
- **Design Tokens** - Colors, spacing, typography, shadows, borders
- **Style Guides** - Documentation, usage guidelines, do's and don'ts
- **Accessibility Guidelines** - ARIA patterns, keyboard shortcuts, focus management

### Prototyping
- **Wireframes** - Low-fidelity layouts for rapid iteration
- **Mockups** - High-fidelity designs with real content
- **Interactive Prototypes** - Clickable prototypes with Figma/Sketch specs
- **Design Handoffs** - Developer-ready specs with measurements, colors, fonts

## Common Use Cases

### 1. UI Audit & Improvements

```
Audit the signup page for UX issues and suggest improvements
```

**Agent will:**
- Analyze visual hierarchy and information architecture
- Check form usability (field labels, validation, error messages)
- Review accessibility (color contrast, keyboard navigation)
- Identify friction points in the signup flow
- Suggest mobile-first improvements
- Provide before/after mockups

### 2. Design a New Component

```
Design a mobile-first navigation menu with hamburger icon
```

**Agent will:**
- Create mobile (320px), tablet (768px), and desktop (1440px) designs
- Specify touch target sizes (minimum 44x44px)
- Design open/close animations
- Add accessibility considerations (ARIA labels, keyboard nav)
- Provide implementation code (HTML + CSS)
- Include interactive states (hover, focus, active)

### 3. Conversion Optimization

```
Optimize the landing page hero section for conversions
```

**Agent will:**
- Analyze current hero design
- Improve headline clarity and value proposition
- Optimize CTA button (size, color, copy, placement)
- Enhance visual hierarchy
- Add social proof elements
- Suggest A/B test variations
- Provide mockups with annotations

### 4. Accessibility Audit

```
Perform WCAG 2.1 AA accessibility audit on the dashboard
```

**Agent will:**
- Check color contrast ratios (minimum 4.5:1)
- Validate keyboard navigation
- Review screen reader compatibility
- Check focus indicators
- Validate form labels and error messages
- Test with common assistive technologies
- Provide remediation code examples

## Design Principles

### Mobile-First Framework

The agent follows a mobile-first approach:

1. **Mobile (320px - 767px)** - Base design
   - Single column layouts
   - Hamburger navigation
   - Touch-friendly targets (44x44px minimum)
   - Simplified content hierarchy

2. **Tablet (768px - 1023px)** - Progressive enhancement
   - Multi-column layouts where appropriate
   - Expanded navigation
   - Larger touch targets
   - More content visible

3. **Desktop (1024px+)** - Full experience
   - Full navigation
   - Multi-column layouts
   - Hover states
   - Advanced interactions

### Accessibility Standards

All designs meet or exceed:

- **WCAG 2.1 Level AA** (default)
- **Color Contrast** - 4.5:1 for normal text, 3:1 for large text
- **Keyboard Navigation** - All interactive elements accessible via keyboard
- **Screen Readers** - Proper ARIA labels and semantic HTML
- **Focus Indicators** - Visible focus states for all interactive elements
- **Touch Targets** - Minimum 44x44px for mobile

### Conversion Optimization

Every design considers:

- **Visual Hierarchy** - Guide users to primary actions
- **CTA Design** - High contrast, action-oriented copy, prominent placement
- **Friction Reduction** - Minimize form fields, provide inline validation
- **Trust Signals** - Social proof, security badges, testimonials
- **Urgency/Scarcity** - Limited-time offers, stock indicators (when authentic)

## Output Format

### Design Audit Report

```markdown
# UX/UI Audit: [Page Name]

## Executive Summary
[High-level findings and priority recommendations]

## Design Consistency (Score: X/10)
- Spacing: ✅/⚠️/❌ [Issues found]
- Typography: ✅/⚠️/❌ [Issues found]
- Colors: ✅/⚠️/❌ [Issues found]
- Components: ✅/⚠️/❌ [Issues found]

## Accessibility (Score: X/10)
- Color Contrast: ✅/⚠️/❌ [Issues found]
- Keyboard Nav: ✅/⚠️/❌ [Issues found]
- Screen Readers: ✅/⚠️/❌ [Issues found]
- Focus Indicators: ✅/⚠️/❌ [Issues found]

## Mobile Responsiveness (Score: X/10)
- Breakpoints: ✅/⚠️/❌ [Issues found]
- Touch Targets: ✅/⚠️/❌ [Issues found]
- Mobile Patterns: ✅/⚠️/❌ [Issues found]

## Conversion Optimization (Score: X/10)
- Visual Hierarchy: ✅/⚠️/❌ [Issues found]
- CTA Design: ✅/⚠️/❌ [Issues found]
- Friction Points: ✅/⚠️/❌ [Issues found]

## Priority Recommendations
1. [High Priority Issue + Solution]
2. [Medium Priority Issue + Solution]
3. [Low Priority Issue + Solution]

## Mockups
[Before/After designs or improvement mockups]

## Implementation Guide
[Step-by-step implementation with code examples]
```

### Design Deliverable

```markdown
# Component Design: [Component Name]

## Overview
[Purpose, use cases, context]

## Design Specifications

### Mobile (320px - 767px)
- Dimensions: [width x height]
- Spacing: [padding, margins]
- Typography: [font, size, weight, line-height]
- Colors: [background, text, borders]
- States: [default, hover, active, disabled, error]

### Tablet (768px - 1023px)
[Similar specifications for tablet]

### Desktop (1024px+)
[Similar specifications for desktop]

## Accessibility
- ARIA Labels: [specific labels]
- Keyboard Navigation: [tab order, shortcuts]
- Screen Reader Text: [hidden text for context]
- Color Contrast: [ratios]

## Interactive States
- Default: [description]
- Hover: [description]
- Focus: [description]
- Active: [description]
- Disabled: [description]
- Error: [description]

## Code Implementation
[HTML + CSS + JavaScript if needed]

## Usage Guidelines
- ✅ Do: [recommended usage]
- ❌ Don't: [anti-patterns]
```

## Design System Support

The agent supports common design systems:

| System | Components | Utilities | Customization |
|--------|-----------|-----------|---------------|
| **Material Design** | 50+ components | Grid, spacing, elevation | Theme customization |
| **Bootstrap** | 40+ components | Grid, spacing, utilities | Sass variables |
| **Tailwind CSS** | Utility-first | All utilities | Config file |
| **Ant Design** | 60+ components | Grid, spacing, themes | Theme editor |
| **Chakra UI** | 50+ components | Style props, themes | Theme customization |
| **Custom** | Your components | Your utilities | Full control |

## Advanced Features

### Design Tokens

Generate design tokens for consistency:

```json
{
  "colors": {
    "primary": "#007bff",
    "secondary": "#6c757d",
    "success": "#28a745",
    "danger": "#dc3545"
  },
  "spacing": {
    "xs": "4px",
    "sm": "8px",
    "md": "16px",
    "lg": "24px",
    "xl": "32px"
  },
  "typography": {
    "fontFamily": "Inter, sans-serif",
    "fontSize": {
      "xs": "12px",
      "sm": "14px",
      "base": "16px",
      "lg": "18px",
      "xl": "20px"
    }
  }
}
```

### A/B Testing Guidance

The agent can suggest A/B test variations:

- **Headline variations** - Different value propositions
- **CTA variations** - Button copy, color, size, placement
- **Layout variations** - Different information hierarchies
- **Image variations** - Hero images, product photos
- **Form variations** - Field count, layout, validation

### Responsive Image Optimization

Guidance on:
- **Srcset/sizes** - Responsive images
- **WebP/AVIF** - Modern image formats
- **Lazy loading** - Performance optimization
- **Art direction** - Different crops for different screens

## Benefits

### For Designers
- **Consistency** - Maintain design system standards
- **Accessibility** - WCAG compliance built-in
- **Efficiency** - Rapid prototyping with best practices
- **Collaboration** - Developer-ready specifications

### For Developers
- **Implementation Guidance** - Code examples for every design
- **Accessibility Code** - ARIA patterns, semantic HTML
- **Responsive Code** - Media queries, mobile-first CSS
- **Performance** - Optimized implementations

### For Product Teams
- **Conversion Focus** - Designs optimized for business goals
- **User-Centered** - Research-backed design decisions
- **A/B Testing** - Data-driven design iterations
- **Scalability** - Design systems for growth

## Version

**v1.0** - Universal UX/UI Design Expert Agent
**Design Systems Supported:** Material, Bootstrap, Tailwind, Ant Design, Chakra UI, Custom
**Accessibility:** WCAG 2.1 AA/AAA
**Template Size:** 2700+ lines

## Additional Resources

- **[Main Repository README](../../README.md)** - Overview of all available agents
- **[Customization Guide](../../guides/SUBAGENT_CUSTOMIZATION_TEMPLATE.md)** - How to customize any agent
- **[Quick Start](../../QUICK_START.md)** - General agent setup guide

## Support

**Questions or issues?**
- Review the agent template for detailed usage instructions
- Check inline comments for configuration options
- Open an issue in the repository

---

**Ready to design?** Follow the Quick Start guide above to get started in 3 minutes.
