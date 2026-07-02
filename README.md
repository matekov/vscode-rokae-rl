# ROKAE RL for Visual Studio Code

Syntax highlighting and dark theme for **ROKAE xCore Robot Language (RL)** `.mod` files.

This extension provides a lightweight development environment for ROKAE RL inside Visual Studio Code. It automatically recognizes `.mod` files, applies syntax highlighting, and includes a dark theme inspired by the ROKAE xCore programming environment.

---

## Features

- Automatic recognition of `.mod` source files
- Custom ROKAE RL language definition
- Custom **ROKAE Dark** theme
- Syntax highlighting for:
  - Keywords
  - Data types
  - Robot motion commands
  - Built-in functions
  - Constants
  - Variables
  - Strings
  - Numbers
  - Comments
- Automatic bracket matching
- Automatic quote pairing
- Line and block comment support

---

## Installation

### Install from VSIX

1. Download the latest `.vsix` package from the GitHub Releases page.
2. Open **Visual Studio Code**.
3. Open the **Extensions** view (`Ctrl + Shift + X`).
4. Click the **...** menu in the upper-right corner.
5. Select **Install from VSIX...**
6. Choose the downloaded `.vsix` file.
7. Reload Visual Studio Code if prompted.

---

## Selecting the Theme

After installing the extension:

1. Press `Ctrl + K`, then `Ctrl + T`
   (or open **Preferences → Color Theme**).
2. Select:

```
ROKAE Dark
```

---

## Opening ROKAE Projects

Open any folder containing `.mod` files.

The extension will automatically recognize them as **ROKAE RL**.

If a file is opened as another language:

1. Click the language indicator in the bottom-right corner.
2. Select

```
ROKAE RL
```

3. Choose **Configure File Association** if you want VS Code to remember it.

---

## Building the Extension

Install dependencies:

```bash
npm install
```

Package the extension:

```bash
npx vsce package
```

The generated `.vsix` package will be created in the project directory (or in `dist/` if using the `--out` option).

---

## Project Structure

```
.
├── syntaxes/
│   └── rokae.tmLanguage.json
├── themes/
│   └── rokae-dark-color-theme.json
├── language-configuration.json
├── package.json
├── README.md
├── CHANGELOG.md
└── LICENSE
```

---

## Planned Features

- Code snippets
- Symbol navigation
- Function list
- Code folding improvements
- Hover documentation
- Go to Definition
- Diagnostics
- IntelliSense support
- Auto-completion

---

## License

MIT License.