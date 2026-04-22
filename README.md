# LPJ-GUESS `.ins` Syntax Highlighting (VS Code)

This folder contains a minimal VS Code language extension for LPJ-GUESS
instruction files (`*.ins`).

## What It Highlights

- `!` line comments (including inline comments)
- Directives: `import`, `include`, `param`, `group`, `pft`, `st`, `mt`
- Assignment keys at start of lines (e.g. `ifdailygrass`, `file_met_forcing`)
- Strings in single or double quotes
- Numeric literals (integers, floats, scientific notation)
- Parentheses/brackets

## Install Locally (from this repo)

1. Open VS Code in this repository.
2. Open Extensions (`Ctrl+Shift+X` / `Cmd+Shift+X`).
3. Click the `...` menu in the Extensions view.
4. Choose `Install from VSIX...` if you have packaged the extension, or run in
   extension dev mode with:

```bash
code --extensionDevelopmentPath "/path/to/vscode-lpj-ins"
```

## Notes

- This is a syntax grammar only (no validation/linting).
- If needed, additional keyword classes can be added in
  `syntaxes/lpj-ins.tmLanguage.json`.
