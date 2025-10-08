# SEO & Content Marketing Specialist Agent

**Comprehensive SEO and content marketing agent for Claude Code - Optimize content for search engines and conversions**

## Overview

The SEO & Content Marketing Specialist Agent helps you create SEO-optimized content, perform competitive analysis, conduct keyword research, and implement technical SEO best practices. Perfect for content creators, marketers, and developers building content-rich applications.

## Key Features

✅ **Full-Stack SEO Capabilities** - On-page, technical, and content SEO
✅ **Keyword Research & Analysis** - Target keyword identification and optimization
✅ **Competitive Analysis** - Analyze competitors' SEO strategies
✅ **Content Optimization** - Meta tags, headings, internal linking, readability
✅ **Technical SEO Audits** - Site speed, mobile-friendliness, structured data
✅ **Universal & Configurable** - Works with any CMS, framework, or static site generator
✅ **Schema.org Markup** - Automated JSON-LD structured data generation

## Files in This Directory

- **Universal SEO & Content Marketing Specialist Agent Template.md** - The main agent template

## Quick Start

### Step 1: Install the Agent

```bash
# Copy to your project's .claude/agents/ directory
cp "Universal SEO & Content Marketing Specialist Agent Template.md" /path/to/your/project/.claude/agents/seo-specialist.md
```

### Step 2: Configure (2 minutes)

Open the file and update the `PROJECT CONFIGURATION` section:

```yaml
# SEO Configuration
domain: "example.com"                            # Your domain
default_locale: "en-US"                          # Primary language/locale
target_audience: "B2B SaaS buyers"               # Your target audience

# Content Paths
content_path: "content/"                         # Where your content files live
public_path: "public/"                           # Public/static assets directory
seo_reports_path: "docs/seo/"                    # Where SEO reports are saved

# CMS/Framework
cms_type: "markdown"                             # markdown | wordpress | contentful | custom
framework: "nextjs"                              # nextjs | gatsby | hugo | wordpress | custom
```

### Step 3: Find/Replace Placeholders (1 minute)

Use your editor's Find/Replace (Ctrl+H or Cmd+H):

| Find | Replace |
|------|---------|
| `{domain}` | `example.com` |
| `{content_path}` | `content/` |
| `{public_path}` | `public/` |
| `{seo_reports_path}` | `docs/seo/` |

### Step 4: Test

Invoke the agent in Claude Code:

```
Perform SEO audit of the homepage
```

## What the Agent Does

### Content SEO
- **Keyword Research** - Identify target keywords with search volume and competition data
- **Content Optimization** - Optimize titles, meta descriptions, headings, and body content
- **Readability Analysis** - Flesch reading score, sentence length, paragraph structure
- **Internal Linking** - Strategic internal link suggestions
- **Content Gap Analysis** - Identify missing content opportunities

### Technical SEO
- **Site Speed Audit** - Performance analysis and optimization recommendations
- **Mobile-Friendliness** - Responsive design and mobile usability checks
- **Structured Data** - Schema.org markup generation (Article, Product, FAQ, etc.)
- **Robots.txt & Sitemap** - Configuration and validation
- **Core Web Vitals** - LCP, FID, CLS analysis

### Competitive Analysis
- **Competitor SEO Audit** - Analyze competitors' keyword strategies
- **Backlink Analysis** - Identify competitor backlink sources
- **Content Gap Analysis** - Find topics competitors rank for that you don't
- **SERP Analysis** - Understand search intent and ranking factors

## Common Use Cases

### 1. Optimize Blog Post

```
Optimize this blog post for SEO: content/blog/getting-started.md
Target keyword: "getting started with [product]"
```

**Agent will:**
- Analyze keyword density and placement
- Optimize meta tags and headings
- Add internal links to related content
- Generate Schema.org Article markup
- Provide readability improvements
- Suggest image alt text

### 2. Technical SEO Audit

```
Perform comprehensive technical SEO audit
```

**Agent will:**
- Check site speed and Core Web Vitals
- Validate robots.txt and sitemap
- Audit structured data implementation
- Check mobile-friendliness
- Identify broken links
- Review security (HTTPS, security headers)

### 3. Keyword Research

```
Perform keyword research for topic: "project management tools"
```

**Agent will:**
- Identify primary and related keywords
- Estimate search volume and competition
- Analyze search intent
- Suggest long-tail keyword opportunities
- Provide content structure recommendations

### 4. Competitive Analysis

```
Analyze competitor SEO strategy: competitor-domain.com
```

**Agent will:**
- Identify competitor's top-ranking keywords
- Analyze their content strategy
- Review their backlink profile
- Identify content gaps and opportunities
- Provide actionable recommendations

## Supported Platforms

| Platform | Content Management | SEO Features |
|----------|-------------------|--------------|
| **Next.js** | Markdown, MDX, CMS | next-seo, sitemap, robots.txt |
| **Gatsby** | Markdown, CMS | gatsby-plugin-seo, gatsby-plugin-sitemap |
| **WordPress** | WordPress CMS | Yoast SEO, RankMath integration |
| **Hugo** | Markdown | Built-in SEO templates |
| **Contentful** | Headless CMS | API-based content optimization |
| **Custom** | Any system | Framework-agnostic recommendations |

## Schema.org Markup Support

The agent generates JSON-LD structured data for:

- **Article** - Blog posts, news articles
- **Product** - E-commerce products
- **FAQ** - Frequently asked questions
- **How-To** - Step-by-step guides
- **Event** - Events, webinars
- **Organization** - Company information
- **Person** - Author/person profiles
- **Recipe** - Cooking recipes
- **Review** - Product/service reviews

## Output Format

### SEO Audit Report

```markdown
# SEO Audit Report: [Page Title]

## Executive Summary
[High-level findings and priority recommendations]

## On-Page SEO (Score: X/100)
- Title Tag: ✅/⚠️/❌
- Meta Description: ✅/⚠️/❌
- Headings Structure: ✅/⚠️/❌
- Keyword Optimization: ✅/⚠️/❌
- Internal Linking: ✅/⚠️/❌

## Technical SEO (Score: X/100)
- Site Speed: ✅/⚠️/❌
- Mobile-Friendliness: ✅/⚠️/❌
- Structured Data: ✅/⚠️/❌
- Security: ✅/⚠️/❌

## Content Quality (Score: X/100)
- Readability: ✅/⚠️/❌
- Content Length: ✅/⚠️/❌
- Keyword Usage: ✅/⚠️/❌

## Recommendations
[Prioritized list of actionable improvements]

## Implementation Guide
[Step-by-step instructions with code examples]
```

## Benefits

### For Content Creators
- **SEO-Optimized Content** - Every piece of content follows SEO best practices
- **Keyword Guidance** - Data-driven keyword targeting
- **Competitive Insights** - Learn from competitors' strategies
- **Readability Improvements** - Make content more engaging

### For Developers
- **Technical SEO** - Implement structured data, sitemaps, robots.txt
- **Performance Optimization** - Improve Core Web Vitals
- **Automated Audits** - Regular SEO health checks
- **Framework-Specific Guidance** - Tailored to your tech stack

### For Marketers
- **Content Strategy** - Data-driven content planning
- **Competitive Analysis** - Understand market landscape
- **ROI Tracking** - Measure SEO impact
- **Multi-Channel Integration** - SEO aligned with overall marketing

## Best Practices

### SEO Content Checklist
- ✅ Target keyword in title (first 60 characters)
- ✅ Target keyword in meta description (first 160 characters)
- ✅ Target keyword in H1 (once)
- ✅ Related keywords in H2s and H3s
- ✅ Target keyword in first paragraph
- ✅ Internal links to related content (3-5 links)
- ✅ External links to authoritative sources (1-3 links)
- ✅ Image alt text with keywords
- ✅ Schema.org markup where applicable
- ✅ Mobile-friendly and fast loading

### Content Structure
- **Title Tag** - 50-60 characters, includes target keyword
- **Meta Description** - 150-160 characters, compelling CTA
- **H1** - One per page, includes target keyword
- **H2s/H3s** - Logical structure, includes related keywords
- **Content Length** - 800+ words for blog posts, 300+ for pages
- **Readability** - 8th-9th grade reading level (Flesch 60-70)

## Configuration Options

### SEO Scoring Weights

Customize how the agent scores SEO factors:

```yaml
seo_scoring:
  on_page_weight: 40        # Title, meta, headings, keywords
  technical_weight: 30      # Speed, mobile, structured data
  content_weight: 20        # Readability, length, quality
  off_page_weight: 10       # Backlinks, social signals
```

### Keyword Density Targets

```yaml
keyword_targets:
  primary_density: "1-2%"   # Target keyword density
  related_density: "0.5-1%" # Related keywords density
  title_required: true      # Must include in title
  h1_required: true         # Must include in H1
```

## Advanced Features

### Custom Schema Templates
Add project-specific Schema.org templates for unique content types.

### SEO Monitoring Integration
Connect with Google Search Console, Ahrefs, SEMrush APIs.

### Automated Reporting
Schedule regular SEO audits and email reports.

### Multi-Language SEO
Configure hreflang tags and locale-specific optimization.

## Version

**v1.0** - Universal SEO & Content Marketing Agent
**Platform Support:** All major CMS and frameworks
**Setup Time:** 3 minutes

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

**Ready to optimize your content?** Follow the Quick Start guide above to get started in 3 minutes.
