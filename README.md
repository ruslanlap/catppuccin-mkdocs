# 🎨 MkDocs Catppuccin Theme

<p align="center">
  <img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/palette/macchiato.png" width="400" alt="Catppuccin Palette"/>
</p>

<p align="center">
  <strong>Soothing pastel theme for MkDocs based on the Catppuccin color palette</strong>
</p>

<p align="center">
  <a href="https://pypi.org/project/mkdocs-catppuccin">
    <img alt="PyPI" src="https://img.shields.io/pypi/v/mkdocs-catppuccin">
  </a>
  <a href="https://pypi.org/project/mkdocs-catppuccin">
    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/mkdocs-catppuccin">
  </a>
  <a href="https://github.com/ruslanlap/Catppuccin-MkDocs/blob/main/LICENSE">
    <img alt="License" src="https://img.shields.io/github/license/ruslanlap/Catppuccin-MkDocs">
  </a>
</p>

## Overview

MkDocs Catppuccin extends [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) with the four Catppuccin flavors: Latte, Frappé, Macchiato, and Mocha. Every flavor includes matching UI colors and syntax highlighting to keep your documentation cohesive.

## Installation

```bash
pip install mkdocs-catppuccin
```

## Usage

Enable the theme in `mkdocs.yml`:

```yaml
theme:
  name: catppuccin
```

### Selecting color schemes

Use `theme.palette` to pick any Catppuccin flavor. Schemes map directly to the palette names:

- `default`: Latte (light)
- `frappe`: Frappé
- `macchiato`: Macchiato
- `slate`: Mocha (dark)

Examples:

```yaml
# Light + dark toggle
theme:
  name: catppuccin
  palette:
    - media: "(prefers-color-scheme: light)"
      scheme: default
      toggle:
        icon: material/weather-night
        name: Switch to dark mode
    - media: "(prefers-color-scheme: dark)"
      scheme: slate
      toggle:
        icon: material/weather-sunny
        name: Switch to light mode
```

```yaml
# Switching through intermediate flavors
theme:
  name: catppuccin
  palette:
    - scheme: frappe
      toggle:
        icon: material/weather-sunset
        name: Switch to Macchiato
    - scheme: macchiato
      toggle:
        icon: material/weather-night
        name: Switch to Latte
```

## Development

```bash
# Clone and install in editable mode
git clone https://github.com/ruslanlap/Catppuccin-MkDocs.git
cd Catppuccin-MkDocs
pip install -e .
```

Build the package locally:

```bash
python -m pip install --upgrade pip build
python -m build
```

Publishing to PyPI is automated via the `publish.yml` GitHub Actions workflow, which builds the project and uploads distributions when a release is created. Provide a `PYPI_API_TOKEN` secret in the repository settings to enable publishing.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
