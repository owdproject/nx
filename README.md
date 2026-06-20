<p align="center">
  <img width="160" height="160" src="https://avatars.githubusercontent.com/u/65117737?s=160&v=4" />
</p>
<h1 align="center">Nx</h1>
<h3 align="center">
  Nx plugin for Open Web Desktop workspace automation.
</h3>

<br />

## Overview

This Nx plugin provides custom executors to automate the installation and configuration of OWD apps, modules, and themes in your workspace. It handles registering configurations and managing symlinks during workspace development.

## Installation

```bash
pnpm add -D @owdproject/nx
```

## Setup

Add the plugin to your workspace's `nx.json`:

```json
{
  "plugins": [
    {
      "plugin": "@owdproject/nx"
    }
  ]
}
```

Define the targets in your desktop project's `project.json`:

```json
{
  "name": "desktop",
  "targets": {
    "install-app": {
      "executor": "@owdproject/nx:install-app"
    },
    "install-module": {
      "executor": "@owdproject/nx:install-module"
    },
    "install-theme": {
      "executor": "@owdproject/nx:install-theme"
    }
  }
}
```

## Usage

Once configured, you can run the executors directly using Nx to add items to your OWD setup:

### Install an App
```bash
npx nx run desktop:install-app --name="@owdproject/app-about"
```

### Install a Module
```bash
npx nx run desktop:install-module --name="@owdproject/module-fs"
```

### Install a Theme
```bash
npx nx run desktop:install-theme --name="@owdproject/theme-nova"
```

## License

This package is released under the [MIT License](LICENSE).
