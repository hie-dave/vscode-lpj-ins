# LPJ-GUESS Instruction (.ins) File Support for Visual Studio Code

This folder contains a minimal VS Code language extension for LPJ-GUESS
instruction files (`*.ins`).

## What It Highlights

- `!` line comments (including inline comments)
- Directives: `import`, `include`, `param`, `group`, `pft`, `st`, `mt`, `file`,
  `column`
- Assignment keys at start of lines (e.g. `ifdailygrass`, `npatch`)
- Strings in single or double quotes
- Numeric literals (integers, floats, scientific notation)
- Parentheses/brackets

## Install Locally (from this repo)

```bash
npm install --save-dev @vscode/vsce
npx @vscode/vsce package

# This will create a .vsix file, which you can install in VS Code:
code --install-extension lpj-ins-0.0.1.vsix # Adjust filename as needed
```

## Notes

- This is a syntax grammar only (no validation/linting).
- If needed, additional keyword classes can be added in
  `syntaxes/lpj-ins.tmLanguage.json`.
