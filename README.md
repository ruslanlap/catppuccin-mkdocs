# 🎨 MkDocs Catppuccin Theme

<p align="center">
  <img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/palette/macchiato.png" width="400" alt="Catppuccin Palette"/>
</p>

<p align="center">
  <strong>
    Soothing pastel theme for MkDocs based on the Catppuccin color palette
  </strong>
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

---

## 📖 Overview

This is a [MkDocs](https://www.mkdocs.org/) theme that extends [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) with the beautiful [Catppuccin](https://catppuccin.com) color palette. It provides a comfortable and aesthetically pleasing documentation experience with carefully crafted soothing pastel colors.

## ✨ Features

- 🎨 **Four Catppuccin Flavors**: Latte (light), Frappé, Macchiato, and Mocha (dark)
- 🌈 **Complete Color Integration**: All UI elements styled with Catppuccin colors
- 🎯 **Syntax Highlighting**: Code blocks with Catppuccin-themed syntax colors
- 📱 **Fully Responsive**: Works perfectly on all devices
- 🔌 **Easy Installation**: Just `pip install mkdocs-catppuccin`
- ⚡ **Extends Material**: All Material for MkDocs features available

## 🚀 Installation

Install the theme using pip:

```bash
pip install mkdocs-catppuccin
```

Or install from source:

```bash
git clone https://github.com/ruslanlap/Catppuccin-MkDocs.git
cd Catppuccin-MkDocs
pip install -e .
```

## 📝 Usage

### Basic Configuration

Add the theme to your `mkdocs.yml`:

```yaml
theme:
  name: catppuccin
```

### With Color Scheme Toggle

Enable switching between light and dark modes:

```yaml
theme:
  name: catppuccin
  palette:
    # Light mode - Catppuccin Latte
    - media: "(prefers-color-scheme: light)"
      scheme: default
      toggle:
        icon: material/weather-night
        name: Switch to dark mode

    # Dark mode - Catppuccin Mocha
    - media: "(prefers-color-scheme: dark)"
      scheme: slate
      toggle:
        icon: material/weather-sunny
        name: Switch to light mode
```

### Advanced Configuration

Customize further with Material for MkDocs features:

```yaml
theme:
  name: catppuccin
  features:
    - navigation.tabs
    - navigation.sections
    - navigation.top
    - search.suggest
    - search.highlight
    - content.code.copy
  palette:
    - scheme: default
      toggle:
        icon: material/weather-night
        name: Switch to dark mode
    - scheme: slate
      toggle:
        icon: material/weather-sunny
        name: Switch to light mode
```

## 🎨 Color Schemes

### Light Mode - Latte 🌻
Perfect for daytime reading with warm, gentle tones:
- **Background**: `#eff1f5` (Base)
- **Text**: `#4c4f69` (Text)
- **Primary**: `#8839ef` (Mauve)
- **Accent**: `#1e66f5` (Blue)

### Dark Mode - Mocha 🌙
Cozy and comfortable for nighttime with rich, soft colors:
- **Background**: `#1e1e2e` (Base)
- **Text**: `#cdd6f4` (Text)
- **Primary**: `#cba6f7` (Mauve)
- **Accent**: `#89b4fa` (Blue)

### Syntax Highlighting

Both themes include complete syntax highlighting:
- **Keywords**: Red
- **Strings**: Green
- **Functions**: Mauve
- **Numbers**: Peach
- **Comments**: Overlay0
- **Operators**: Sky
- **Variables**: Rosewater

## 📦 What's Included

```
mkdocs-catppuccin/
├── mkdocs_catppuccin/
│   ├── __init__.py
│   ├── mkdocs_theme.yml         # Theme configuration
│   └── assets/
│       └── stylesheets/
│           └── catppuccin.css   # Catppuccin colors
├── pyproject.toml               # Package configuration
├── LICENSE                      # MIT License
└── README.md                    # This file
```

## 🔧 Development

### Setting Up Development Environment

```bash
# Clone the repository
git clone https://github.com/ruslanlap/Catppuccin-MkDocs.git
cd Catppuccin-MkDocs

# Install in editable mode
pip install -e .

# Create a test MkDocs project
mkdocs new test-site
cd test-site

# Configure to use the theme
echo "theme:
  name: catppuccin" > mkdocs.yml

# Serve the documentation
mkdocs serve
```

### Building the Package

```bash
# Install build tools
pip install build twine

# Build the package
python -m build

# The package will be in dist/
```

### Publishing to PyPI

```bash
# Upload to TestPyPI first
python -m twine upload --repository testpypi dist/*

# If everything looks good, upload to PyPI
python -m twine upload dist/*
```

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Credits

- **Catppuccin Theme**: [catppuccin.com](https://catppuccin.com) - The beautiful color palette
- **Material for MkDocs**: [squidfunk/mkdocs-material](https://github.com/squidfunk/mkdocs-material) - The base theme
- **MkDocs**: [mkdocs.org](https://www.mkdocs.org/) - The documentation framework

## 🔗 Links

- **Homepage**: [github.com/ruslanlap/Catppuccin-MkDocs](https://github.com/ruslanlap/Catppuccin-MkDocs)
- **PyPI**: [pypi.org/project/mkdocs-catppuccin](https://pypi.org/project/mkdocs-catppuccin)
- **Catppuccin**: [catppuccin.com](https://catppuccin.com)
- **Material for MkDocs**: [squidfunk.github.io/mkdocs-material](https://squidfunk.github.io/mkdocs-material)

---

<p align="center">
  <a href="https://squidfunk.github.io/mkdocs-material/">
    <img src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/logo.svg" width="320" alt="Material for MkDocs">
  </a>
</p>

<p align="center">
  <strong>
    Original Material for MkDocs - A powerful documentation framework on top of
    <a href="https://www.mkdocs.org/">MkDocs</a>
  </strong>
</p>

<p align="center">
  <a href="https://github.com/squidfunk/mkdocs-material/actions"><img
    src="https://github.com/squidfunk/mkdocs-material/workflows/build/badge.svg"
    alt="Build"
  /></a>
  <a href="https://pypistats.org/packages/mkdocs-material"><img
    src="https://img.shields.io/pypi/dm/mkdocs-material.svg"
    alt="Downloads"
  /></a>
  <a href="https://pypi.org/project/mkdocs-material"><img
    src="https://img.shields.io/pypi/v/mkdocs-material.svg"
    alt="Python Package Index"
  /></a>
  <a href="https://hub.docker.com/r/squidfunk/mkdocs-material/"><img
    src="https://img.shields.io/docker/pulls/squidfunk/mkdocs-material"
    alt="Docker Pulls"
  /></a>
</p>

<p align="center">
  Write your documentation in Markdown and create a professional static site for
  your Open Source or commercial project in minutes – searchable, customizable,
  more than 60 languages, for all devices.
</p>

<p align="center">
  <a href="https://squidfunk.github.io/mkdocs-material/getting-started/">
    <img src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/screenshot.png" width="700" />
  </a>
</p>

<p align="center">
  <em>
    Check out the demo –
    <a
      href="https://squidfunk.github.io/mkdocs-material/"
    >squidfunk.github.io/mkdocs-material</a>.
  </em>
</p>

<h2></h2>
<p id="premium-sponsors">&nbsp;</p>
<p align="center"><strong>Silver sponsors</strong></p>
<p align="center">
  <a href="https://fastapi.tiangolo.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-fastapi.png" height="120"
  /></a>
  <a href="https://www.trendpop.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-trendpop.png" height="120"
  /></a>
  <a href="https://documentation.sailpoint.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-sailpoint.png" height="120"
  /></a>
  <a href="https://futureplc.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-future.svg" width="332" height="120"
  /></a>
  <a href="https://opensource.siemens.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-siemens.png" height="120"
  /></a>
</p>
<p>&nbsp;</p>
<p align="center"><strong>Bronze sponsors</strong></p>
<p align="center">
  <a href="https://cirrus-ci.org/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-cirrus-ci.png" height="58"
  /></a>
  <a href="https://docs.baslerweb.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-basler.png" height="58"
  /></a>
  <a href="https://kx.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-kx.png" height="58"
  /></a>
  <a href="https://orion-docs.prefect.io/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-prefect.png" height="58"
  /></a>
  <a href="https://www.zenoss.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-zenoss.png" height="58"
  /></a>
  <a href="https://docs.posit.co" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-posit.png" height="58"
  /></a>
  <a href="https://n8n.io" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-n8n.png" height="58"
  /></a>
  <a href="https://www.dogado.de" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-dogado.png" height="58"
  /></a>
  <a href="https://wwt.com" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-wwt.png" height="58"
  /></a>
  <a href="https://elastic.co" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-elastic.png" height="58"
  /></a>
  <a href="https://ipfabric.io/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-ip-fabric.png" height="58"
  /></a>
  <a href="https://www.apex.ai/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-apex-ai.png" height="58"
  /></a>
  <a href="https://jitterbit.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-jitterbit.png" height="58"
  /></a>
  <a href="https://sparkfun.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-sparkfun.png" height="58"
  /></a>
  <a href="https://eccenca.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-eccenca.png" height="58"
  /></a>
  <a href="https://neptune.ai/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-neptune-ai.png" height="58"
  /></a>
  <a href="https://rackn.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-rackn.png" height="58"
  /></a>
  <a href="https://civicactions.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-civic-actions.png" height="58"
  /></a>
  <a href="https://getscreen.me/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-getscreenme.png" height="58"
  /></a>
  <a href="https://botcity.dev/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-botcity.png" height="58"
  /></a>
  <a href="https://kolena.io/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-kolena.png" height="58"
  /></a>
  <a href="https://www.evergiving.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-evergiving.png" height="58"
  /></a>
  <a href="https://astral.sh/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-astral.png" height="58"
  /></a>
  <a href="https://oikolab.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-oikolab.png" height="58"
  /></a>
  <a href="https://www.buhlergroup.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-buhler.png" height="58"
  /></a>
  <a href="https://3dr.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-3dr.png" height="58"
  /></a>
  <a href="https://spotware.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-spotware.png" height="58"
  /></a>
  <a href="https://milfordasset.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-milford.png" height="58"
  /></a>
  <a href="https://www.lechler.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-lechler.png" height="58"
  /></a>
  <a href="https://invers.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-invers.png" height="58"
  /></a>
  <a href="https://vantor.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-vantor.png" height="58"
  /></a>
  <a href="https://www.equipmentshare.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-equipmentshare.png" height="58"
  /></a>
  <a href="https://hummingbot.org/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-hummingbot.png" height="58"
  /></a>
  <a href="https://octoperf.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-octoperf.png" height="58"
  /></a>
  <a href="https://intercomestibles.ch/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-intercomestibles.png" height="58"
  /></a>
  <a href="https://www.centara.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-centara.png" height="58"
  /></a>
  <a href="https://pydantic.dev/logfire/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-logfire.png" height="58"
  /></a>
  <a href="https://www.vector.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-vector.png" height="58"
  /></a>
  <a href="https://second.tech/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-second.png" height="58"
  /></a>
  <a href="https://mvtec.com/" target=_blank><img
    src="https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/.github/assets/sponsors/sponsor-mvtec.png" height="58"
  /></a>
</p>
<p>&nbsp;</p>

## Everything you would expect

### It's just Markdown

Focus on the content of your documentation and create a professional static site
in minutes. No need to know HTML, CSS or JavaScript – let Material for MkDocs do
the heavy lifting for you.

### Works on all devices

Serve your documentation with confidence – Material for MkDocs automatically
adapts to perfectly fit the available screen estate, no matter the type or size
of the viewing device. Desktop. Tablet. Mobile. All great.

### Made to measure

Make it yours – change the colors, fonts, language, icons, logo, and more with
a few lines of configuration. Material for MkDocs can be easily extended and
provides many options to alter appearance and behavior.

### Fast and lightweight

Don't let your users wait – get incredible value with a small footprint by using
one of the fastest themes available with excellent performance, yielding optimal
search engine rankings and happy users that return.

### Maintain ownership

Own your documentation's complete sources and outputs, guaranteeing both
integrity and security – no need to entrust the backbone of your product
knowledge to third-party platforms. Retain full control.

### Open Source

You're in good company – choose a mature and actively maintained solution built
with state-of-the-art Open Source technologies, trusted by more than 50,000
individuals and organizations. Licensed under MIT.

## Quick start

Material for MkDocs can be installed with `pip`:

``` sh
pip install mkdocs-material
```

Add the following lines to `mkdocs.yml`:

``` yaml
theme:
  name: material
```

For detailed installation instructions, configuration options, and a demo, visit
[squidfunk.github.io/mkdocs-material][Material for MkDocs]

  [Material for MkDocs]: https://squidfunk.github.io/mkdocs-material/

## Trusted by ...

### ... industry leaders

[ArXiv](https://info.arxiv.org),
[Atlassian](https://atlassian.github.io/data-center-helm-charts/),
[AWS](https://aws.github.io/copilot-cli/),
[Bloomberg](https://bloomberg.github.io/selekt/),
[CERN](http://abpcomputing.web.cern.ch/),
[Datadog](https://datadoghq.dev/integrations-core/),
[Google](https://google.github.io/accompanist/),
[Harvard](https://informatics.fas.harvard.edu/),
[Hewlett Packard](https://hewlettpackard.github.io/squest/),
[HSBC](https://hsbc.github.io/pyratings/),
[ING](https://ing-bank.github.io/baker/),
[Intel](https://open-amt-cloud-toolkit.github.io/docs/),
[JetBrains](https://jetbrains.github.io/projector-client/mkdocs/),
[LinkedIn](https://linkedin.github.io/school-of-sre/),
[Microsoft](https://microsoft.github.io/code-with-engineering-playbook/),
[Mozilla](https://mozillafoundation.github.io/engineering-handbook/),
[Netflix](https://netflix.github.io/titus/),
[OpenAI](https://openai.github.io/openai-agents-python/),
[Red Hat](https://ansible.readthedocs.io/projects/lint/),
[Roboflow](https://inference.roboflow.com/),
[Salesforce](https://policy-sentry.readthedocs.io/),
[SIEMENS](https://opensource.siemens.com/),
[Slack](https://slackhq.github.io/circuit/),
[Square](https://square.github.io/okhttp/),
[Uber](https://uber-go.github.io/fx/),
[Zalando](https://opensource.zalando.com/skipper/)

### ... and successful Open Source projects

[Amp](https://amp.rs/docs/),
[Apache Iceberg](https://iceberg.apache.org/),
[Arduino](https://arduino.github.io/arduino-cli/),
[Asahi Linux](https://asahilinux.org/docs/),
[Auto-GPT](https://docs.agpt.co/),
[AutoKeras](https://autokeras.com/),
[BFE](https://www.bfe-networks.net/),
[CentOS](https://docs.infra.centos.org/),
[Crystal](https://crystal-lang.org/reference/),
[eBPF](https://ebpf-go.dev/),
[ejabberd](https://docs.ejabberd.im/),
[Electron](https://www.electron.build/),
[FastAPI](https://fastapi.tiangolo.com/),
[FlatBuffers](https://flatbuffers.dev/),
[{fmt}](https://fmt.dev/),
[Freqtrade](https://www.freqtrade.io/en/stable/),
[GoReleaser](https://goreleaser.com/),
[GraphRAG](https://microsoft.github.io/graphrag/),
[Headscale](https://headscale.net/),
[HedgeDoc](https://docs.hedgedoc.org/),
[Hummingbot](https://hummingbot.org/),
[Knative](https://knative.dev/docs/),
[Kubernetes](https://kops.sigs.k8s.io/),
[kSQL](https://docs.ksqldb.io/),
[LeakCanary](https://square.github.io/leakcanary/),
[LlamaIndex](https://docs.llamaindex.ai/),
[NetBox](https://netboxlabs.com/docs/netbox/en/stable/),
[Nokogiri](https://nokogiri.org/),
[OpenAI](https://openai.github.io/openai-agents-python/),
[OpenFaaS](https://docs.openfaas.com/),
[OpenSSL](https://docs.openssl.org/),
[Orchard Core](https://docs.orchardcore.net/en/latest/),
[Percona](https://docs.percona.com/percona-monitoring-and-management/),
[Pi-Hole](https://docs.pi-hole.net/),
[Polars](https://docs.pola.rs/),
[Pydantic](https://pydantic-docs.helpmanual.io/),
[PyPI](https://docs.pypi.org/),
[Quivr](https://core.quivr.com/),
[Renovate](https://docs.renovatebot.com/),
[RetroPie](https://retropie.org.uk/docs/),
[Ruff](https://docs.astral.sh/ruff/),
[Supervision](https://supervision.roboflow.com/latest/),
[Textual](https://textual.textualize.io/),
[Traefik](https://docs.traefik.io/),
[Trivy](https://aquasecurity.github.io/trivy/),
[Typer](https://typer.tiangolo.com/),
[tinygrad](https://docs.tinygrad.org/),
[Ultralytics](https://docs.ultralytics.com/),
[UV](https://docs.astral.sh/uv/),
[Vapor](https://docs.vapor.codes/),
[WebKit](https://docs.webkit.org/),
[WTF](https://wtfutil.com/),
[ZeroNet](https://zeronet.io/docs/)

## License

**MIT License**

Copyright (c) 2016-2025 Martin Donath

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to
deal in the Software without restriction, including without limitation the
rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
sell copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
IN THE SOFTWARE.
