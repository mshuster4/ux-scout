# UX Scout

A Claude skill that performs deep UX competitive research and generates visual-first research documents with lo-fi direction sketches. Built for designers, useful for PMs and developers.

Give UX Scout a design problem and it will:

1. **Research 3-6 competitors** that solve the same problem, with flow diagrams, IA maps, and wireframe sketches for each
2. **Apply Nielsen's heuristics as a design thinking lens**, scaled to the problem you give it, whether that's a full flow, a single interaction pattern, or anything in between
3. **Synthesize patterns** across competitors: what's conventional, where they diverge, and what's missing
4. **Generate lo-fi direction sketches** (3-7 configurable) ranging from convention-first to innovative
5. **Output a single self-contained easy-to-scan HTML file** with sticky nav, visual artifacts, and a recommendation

The output is visual-first. Every section leads with a diagram, chart, or wireframe. The document is scannable in 30 seconds by looking at visuals alone.

Part of the [Product Design Toolbox](../../README.md). See the [install steps](../../README.md#install) in the main README.

## How to use

### With a prompt

```
/ux-scout Research how other logistics apps handle real-time status tracking
```

### Without a prompt

If you invoke `/ux-scout` with no prompt, it will ask you a guided set of intake questions:
- What are you designing?
- Who is the user?
- What platform/device?
- Any known constraints?

### Modes

- **Deep mode** (default): 4-6 competitors, 5 directions, sub-skill synthesis
- **Quick mode**: 3 competitors, 3 directions, no sub-skills. Add "quick" to your prompt

```
/ux-scout quick: notification center patterns
```

### Configurable directions

Default is 5 directions. Request a different number (3-7):

```
/ux-scout 3 directions: scheduling calendar UX patterns
```

### Output format

- **HTML** (default): Rich visual document with diagrams, charts, and wireframes
- **Markdown**: Add "markdown" to your prompt for teams that prefer docs

```
/ux-scout markdown: onboarding flow best practices
```

### Example prompts

- "Research how other moving apps handle claims resolution"
- "What are best practices for multi-step form wizards? Show me what competitors do"
- "UX research for a scheduling calendar, what patterns work?"
- "How do logistics apps handle real-time status tracking? Research this before we design"
- "Research notification center patterns. I want to see what works before we prototype"
- "/ux-scout quick markdown: dashboard filter patterns"

## Output

UX Scout saves a self-contained HTML file to:

```
docs/ux-research/YYYY-MM-DD-<topic>/research.html
```

The document includes:

- Executive summary strip with key stats
- Competitor cards with flow diagrams, IA diagrams, and wireframe sketches
- Pattern matrix (who uses what)
- Cross-cutting insights with gap map
- Heuristic relevance bar chart
- Lo-fi direction sketches with annotated wireframes
- Direction comparison chart
- Recommendation with MVP scope

## Optional: Enhanced research

UX Scout works fully standalone with no dependencies. For richer persona, JTBD, and synthesis output, install [The Designer Skills Pack](https://github.com/Owl-Listener/designer-skills) by MC Dean.

In the Claude app, add a second marketplace the same way you added this one, using `Owl-Listener/designer-skills`. Then install the `design-research` plugin from the Discover tab.

In Claude Code:

```
/plugin marketplace add Owl-Listener/designer-skills
```

Then install the `design-research` plugin from the Discover tab. UX Scout will automatically use these sub-skills when available:

- `design-research:discover` for persona + journey mapping
- `design-research:jobs-to-be-done` for JTBD analysis
- `design-research:synthesize` for research data synthesis

If these aren't installed, UX Scout performs lightweight inline analysis instead. Same sections, slightly less depth.
