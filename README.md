# Product Design Toolbox

Product design skills for Claude, from early research to prototyping. Each tool installs separately, so you can pick only the ones you need.

## What's inside

| Tool | What it does |
|---|---|
| [UX Scout](plugins/ux-scout/README.md) | Researches how competitors solve a design problem, then turns the findings into a visual research document with lo-fi direction sketches. |

More tools for wireframing, hi-fi design and prototyping are coming.

## How it fits together

- **Skill:** a set of instructions that teaches Claude one task, like UX research.
- **Plugin:** the installable package that delivers a skill to Claude.
- **Marketplace:** this repo. It's a catalog of plugins you add once, then install tools from.

## Install

### Claude app (no terminal required)

Works in the Claude desktop app on Mac and Windows.

1. Open the Claude app
2. Click **Customize** in the left sidebar, then open the **Plugins** tab
3. Click the **Add** dropdown at the top right and choose **Add marketplace**
4. Select **Add from a repository**, paste `mshuster4/product-design-toolbox`, and sync
5. Switch to the **Discover** tab and find the tool you want, such as **ux-scout**
6. Click the **+** on the plugin card to install it
7. Switch back to **Yours** to confirm it is listed and enabled
8. Start a new conversation and type `/ux-scout` followed by your design problem

When new tools are added, they appear in the **Discover** tab automatically. You don't need to add the marketplace again.

### Claude Code: plugin marketplace

```
/plugin marketplace add mshuster4/product-design-toolbox
/plugin install ux-scout@product-design-toolbox
```

### Claude Code: Skills CLI

```
npx skills add mshuster4/product-design-toolbox --skill ux-scout
```

This copies the skill into your `.claude/skills/` directory automatically.

### Manual (terminal)

From a copy of this repo:

```
cp -r plugins/ux-scout/skills/ux-scout ~/.claude/skills/ux-scout
```

## License

MIT. See [LICENSE](LICENSE).

## Credits

See [CREDITS.md](CREDITS.md) for attribution to the projects and authors that informed these tools.
