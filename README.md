# Blackboard Contrast

A dark VS Code theme based on the classic **Blackboard** palette, tuned so that
selections, highlights, and search matches are each visually distinct from one
another and from normal text.

## Color guide

| State | Color | Notes |
|---|---|---|
| Selection | Bright blue `#2B5FD9` | White foreground on selected text |
| Inactive selection | Blue, 33% alpha | Editor not focused |
| Same text as selection | Teal `#1FB89A` | Fill plus border |
| Word highlight (read) | Purple `#8A5CF6` | Symbol under cursor |
| Word highlight (write) | Magenta `#E0489A` | Assignments |
| Current search match | Orange `#FF6400` | Light border |
| Other search matches | Yellow-green `#D8FA3C` | Translucent plus border |
| Matching bracket | Cyan `#00D1FF` | Fill plus border |
| Hover highlight | Light blue | Subtle |

## Also included

- Full workbench theming: sidebar, tabs, status bar, panels, menus, inputs, buttons
- Bracket pair colorization and error, warning, info colors
- Git decorations, diff editor, and merge conflict colors
- Terminal ANSI palette
- Semantic token colors for TypeScript, JavaScript, and others

## Install

**From the Marketplace:** open Extensions, search for "Blackboard Contrast", install.
Then run **Preferences: Color Theme** and pick *Blackboard Contrast*.

**Manually:**

```
npm install -g @vscode/vsce
vsce package
code --install-extension blackboard-contrast-1.0.0.vsix
```

## Recommended settings

```json
{
  "workbench.colorTheme": "Blackboard Contrast",
  "editor.bracketPairColorization.enabled": true,
  "editor.occurrencesHighlight": "singleFile",
  "editor.selectionHighlight": true
}
```

## Customizing

Override any color in your `settings.json`:

```json
{
  "workbench.colorCustomizations": {
    "[Blackboard Contrast]": {
      "editor.findMatchBackground": "#FF8A33"
    }
  }
}
```

## Credits

Based on the Blackboard TextMate theme by Domenico Carbotta.

## License

MIT, see [LICENSE](LICENSE).
