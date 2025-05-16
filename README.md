<p align="center">
  <img width="160" height="160" src="https://avatars.githubusercontent.com/u/65117737?s=160&v=4" />
</p>
<h1 align="center">Nx Plugin</h1>
<h3 align="center">
  Nx Plugin for Open Web Desktop.
</h3>

## Overview

This plugin for the Open Web Desktop monorepo enables easy modules installation.

## Installation

To install the package, run:

```bash
pnpm install @owdproject/nx
```

## Usage

### Install a new app

```bash
nx run desktop:install-app --name=@owdproject/app-todo
```

### Install a new module

```bash
nx run desktop:install-module --name=@owdproject/module-pinia-localforage
```

### Install a new theme

```bash
nx run desktop:install-theme --name=@owdproject/theme-gnome
```

## License

This plugin is released under the [MIT License](LICENSE).

