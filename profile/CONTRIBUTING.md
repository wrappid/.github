# Contributing to Wrappid Repositories

Welcome to Wrappid! We appreciate your interest and contributions. This document outlines the process for contributing to wrappid repositories. Please take a moment to review it before getting started.

# Getting Started

To start contributing in this repository follow the below steps:

- We love to write code! Where to write?
  We’re going to use VSCode/VSCodium. Please download [VSCode Stable Release](https://code.visualstudio.com/download)
or [VSCodium Stable Release](https://github.com/VSCodium/vscodium/releases)  then install it & open it.
- We need an environment! How to set?
We ❤️ Javascript! We need to set up node 16.20.x & npm 8.x.x, follow the documentation [here](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm).

## How to Contribute

1. If you are Wrappid team member, clone this repository. If you are an external contributor Fork the repository to your GitHub account and clone it to your local machine

2. Create issue branch of issue.

    Create branch from development branch.
    Branch naming convention:  

    ```@terminal
     WRPD-(feature|bugfix|release|ci|enhancement|hotfix|refactor|deps|docs|experimental|security)-(issue-number)
    ```

    e.g., `WRPD-feature-1`

3. Commit your changes with appropriate commit message with [Conventional Commit extentions](https://marketplace.visualstudio.com/items?itemName=vivaxy.vscode-conventional-commits) in your VS Code.

4. For Wrappid members, Create Pull request into development branch from your issue branch. For external contributors, create issue, create issue branch and create pull request under your issue branch.

## Creating Issues

Create Issues to help us grow and improve.

- Use issue templates to create issues

- Issue title format:
         <IssueLabel>:<Issue title (keep it short)>


<!-- # Developer documentation for contributing to Wrappid Framework -->
# Framework Development Documentation

Before proceeding, it is understood that you have already went through [Initial Guide](https://github.com/wrappid#getting-started).

## Essential Commands for Wrappid Development

The two most important commands for Wrappid framework development are:

- **`wd init`**: Initializes the Wrappid development environment.
- **`wd link`**: Links Wrappid development packages to runtime environments.

> _You will learn about these command in details in below comming sections_


These commands work together, with `wd init` setting up the environment and `wd link` utilizing the configured path to link the required packages.

---

<!-- ## Initializing the Wrappid Development Environment
 -->
## Wrappid Development Toolkit - Init Command Guide


This section will guide you through setting up your Wrappid development environment using the Wrappid Development Toolkit CLI.

### Introduction to `wd init`

The `wd init` command initializes your Wrappid development environment by setting up essential configurations and downloading required packages. This is a crucial first step before you can start building applications with the Wrappid framework.

### Command Structure

```bash
wd init [options] [path]
```

#### Options:
- `-f, --force` : Execute the command forcefully without prompts.
- `-h, --help` : Display help information for the command.

### What Happens During Initialization

When you run the `wd init` command, several key processes occur:

1. **Project State Verification:**
   - The system checks if a `WRAPPID_HOME` config file exists and creates one if needed.

2. **Wrappid Dev Home Path Configuration:**
   - The command establishes a path where all Wrappid development packages will be stored.
   - If the path is already set, it uses that location.
   - If not set, it prompts you to provide a path or uses the one you specified as an argument.

3. **Package Verification & Installation:**
   - The system checks if required Wrappid packages exist in the specified path:
     - `@wrappid/core`
     - `@wrappid/native-web`
     - `@wrappid/native-mobile`
     - `@wrappid/styles`
     - `@wrappid/service-core`
   
4. **Missing Package Management:**
   - If packages are missing, you'll be prompted to either:
     - Download the missing packages.
     - Change the path.

5. **Package Validation:**
   - The system verifies that any existing packages are valid Wrappid packages by checking their remote repository URLs.

---

## Wrappid Development Toolkit - Link Command Guide

The `wrappid-dev link` command is a crucial part of the Wrappid development workflow. It establishes connections between your local development packages and the runtime environments for both web and mobile applications.

### Basic Usage

The basic syntax for the link command is:

```bash
wd link [options] [command]
```

This command links Wrappid development packages to your web and mobile runtime environments. It utilizes the packages from the path that `wd init` sets up.

### Options
- `-p, --pkg [value]`: Specify a specific Wrappid package to link (choices: `core`, `native`, `styles`, `score`).
- `-h, --help`: Display help information for the command.

### Commands

- `web [options]`: Link Wrappid development packages to the web runtime environment.
- `mobile [options]`: Link Wrappid development packages to the mobile runtime environment.

### How `link` Works

1. **Environment Setup**: Checks if you're in a valid Wrappid project and sets up the development environment.
2. **Package Building**:
   - Installs necessary dependencies.
   - Builds the package using `npm run build`.
   - Copies the built files to the appropriate runtime destination.
3. **Dependency Management**:
   - Adds required peer dependencies and dev dependencies.
   - Cleans up existing `node_modules`.
   - Installs the linked packages.

### Common Use Cases

#### Development Setup:
```bash
wd link
```

#### Specific Package Updates:
```bash
wd link --pkg core
```

#### Environment-Specific Updates:
```bash
wd link web
# or
wd link mobile
```

The `link` command is essential for maintaining a smooth development workflow when working with Wrappid packages across different environments. It relies on the environment and package locations defined during `wd init`.

For any Wrappid app or service project, during the first setup, you need to run:

**For wrappid-app**

```bash
wd link [web|mobile]
```

**For wrappid-service**

```bash
wd link [web|mobile]
```

After the initial setup, you can update specific packages individually:

```bash
wd link [web|mobile] --pkg [core|native|styles]
```

---

## Turning Off Wrappid Development Mode

To disable Wrappid development mode for a `wrappid-app` type or `wrappid-service` type project, use the following commands:

```bash
wr set --pkg stage
```

**For wrappid-app**

```bash
wr setup [web|mobile] --env [dev|stage|prod]
```

**For wrappid-service**

```bash
wr setup service --env [dev|stage|prod]
```

These commands help configure your environment to the appropriate stage or production setup.

---

By completing the initialization and linking process correctly, your development environment will be properly configured with all necessary Wrappid packages, allowing you to start contributing to Wrappid!