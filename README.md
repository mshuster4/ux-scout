# Product Design Toolbox

Product design skills for Claude, from early research to prototyping. Install it once and you get every skill in the toolbox.

## What's inside

| Skill | What it does |
|---|---|
| [UX Scout](skills/ux-scout/README.md) | Researches how competitors solve a design problem, then turns the findings into a visual research document with lo-fi direction sketches. |

More tools coming soon.

## How it fits together

- **Skill:** a set of instructions that teaches Claude one task, like UX research.
- **Plugin:** the Product Design Toolbox itself. It bundles all the skills into one install.
- **Marketplace:** the source Claude installs the plugin from. For this toolbox, that's this repo.

## Install

### Claude app (no terminal required)

Works in the Claude desktop app on Mac and Windows.

1. Open the Claude app
2. Click **Customize** in the left sidebar, then open the **Plugins** tab
3. Click the **Add** dropdown at the top right and choose **Add marketplace**
4. Select **Add from a repository**, paste `mshuster4/product-design-toolbox`, and sync
5. Switch to the **Discover** tab and find **Product Design Toolbox**
6. Click the **+** on the plugin card to install it
7. Switch back to **Yours** to confirm it is listed and enabled
8. Start a new conversation and type `/ux-scout` followed by your design problem

When new skills are added, they arrive with plugin updates. You don't need to install anything again.

### Claude Code: plugin marketplace

```
/plugin marketplace add mshuster4/product-design-toolbox
/plugin install product-design-toolbox@product-design-toolbox
```

### Claude Code: Skills CLI

```
npx skills add mshuster4/product-design-toolbox --skill ux-scout
```

This copies the skill into your `.claude/skills/` directory automatically.

### Manual (terminal)

From a copy of this repo:

```
cp -r skills/ux-scout ~/.claude/skills/ux-scout
```

## License

MIT. See [LICENSE](LICENSE).

## Credits

See [CREDITS.md](CREDITS.md) for attribution to the projects and authors that informed these skills.
