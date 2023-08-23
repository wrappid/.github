<img src="https://github.com/wrappid/.github/blob/main/logo/logo-1200x400.png" />

<!--
```text
                                    _     _
    __      ___ __ __ _ _ __  _ __ (_) __| |
    \ \ /\ / / '__/ _` | '_ \| '_ \| |/ _` |
     \ V  V /| | | (_| | |_) | |_) | | (_| |
      \_/\_/ |_|  \__,_| .__/| .__/|_|\__,_|
                       |_|   |_|

```

# `Wrappid`
-->

# Wrapper Framework for Rapid development

## `Wrappid` Framework is a wrapper framework built to enable rapid development of applications.

`Wrappid` Framework is a wrapper framework built to enable rapid development of applications based on `React`, `React Native`, `Node`, `Express`, etc. Here, you **write code once** and use `Wrappid Toolkit` to build your web and mobile applications simultaneously.

`Wrappid` includes a repository of components, called the `CoreComponents`, for application developers to use. As application developers, you also have the flexibility to write your own components. By default the styling libraries used are `mui` for web and `react native paper` for mobile.

`Wrappid` also comes with a set of pre-coded business handling modules like app builder, user/role/permission management, authentication, authorization, error reporting, notifications (push/mail/sms/whatsapp), etc.

## Getting Started

This getting started section will help you setup a basic `Wrappid` project environment. The easiest way is to use the `Wrappid Toolkit`.

Follow the below steps to get going.

1. Verify Pre-requisites
2. Install `Wrappid Toolkit`
3. One-time Initialisation
4. Setup `Wrappid` Project(s)

### 1. Verify Pre-requisites

First you need to verify that your system fulfills the pre-requisites. Listed below are the things required to be available in your system.

- Node.js - version 16
- npm - version 8

#### Checking your version of Node.js and npm

To see if you already have Node.js and npm installed and check the installed version, run the following commands:

```terminal
node -v
npm -v
```

#### Refer the exact version we use:

```terminal
node -v
v16.18.1

npm -v
8.19.2
```

Please install them if they are not available in your system. Kindly follow original installation guide to do so.

### 2. Install `Wrappid Toolkit`

To use `Wrappid Toolkit`, you need to install `Wrappid Toolkit` globally in your system.

> <br/>
>
> **_Note:_**
>
> _The `Wrappid Toolkit` is available in the GitHub npm pkg registry. You will have to setup scoped pkg registry as your npm runtime configuration._
>
> _Run the below commands to setup scoped pkg registry:_
>
> <!--C:\Users\Sam>-->
>
> ```terminal
> npm config set @wrappid:registry https://npm.pkg.github.com/wrappid
>
> npm config set //npm.pkg.github.com/:_authToken <WRAPPID_TOKEN>
> ```
>
> _Please fill [Wrappid Early Access Request form](https://forms.gle/NCUbSXvsX1v9QhD96) to get a valid_ `<WRAPPID_TOKEN>`. After filling the form you will receive the `<WRAPPID_TOKEN>` in your email.
>
> _The above mentioned_ `<WRAPPID_TOKEN>` _could only be used to read and download the `Wrappid Toolkit` package._
>
> <br/>

<br/>Run the below command to install `Wrappid Toolkit` globally in your system.

```terminal
npm install -g @wrappid/toolkit
```

Once the installation is done, verify the `Wrappid Toolkit` installation. Run the below command to verify you already have `Wrappid Toolkit` installed and check the installed version

```terminal
wrappid -V
```

This should show you the exact version of `Wrappid Toolkit` installed

```terminal
wrappid -V
v0.0.14
```

### 3. One-time Initialisation

Run the below command to install all dependencies `Wrappid Toolkit` uses

```terminal
wrappid install
```

This one-time initialisation of `Wrappid Toolkit` follows the below steps:

- Install package dependencies
- Download & Install GitHub CLI or `gh` (if not already installed)
- Authenticate with GitHub A/c to use GitHub CLI or `gh`

#### 3.1. Install package dependencies

This is a automated process. You need not do anything.

#### 3.2. Download & Install GitHub CLI or `gh` (if not already installed)

This is a automated process but you will be prompted with GitHub CLI or `gh` installation. Kindly click Next -> Next -> ... -> Finish to complete the GitHub CLI or `gh` installation.

#### 3.3. Authenticate with GitHub A/c to use GitHub CLI or `gh`

When prompted, follow on-screen instructions to authenticate yourself with your GitHub A/c. It starts like:

<!-- <span style="color:orange"><code>GitHub CLI authenticating...</code></span> -->

```terminal
GitHub CLI authenticating...
? What account do you want to log into?  [Use arrows to move, type to filter]
> GitHub.com
  GitHub Enterprise Server
```

Select Github.com (generally already selected), Press Enter.

You'll be asked to authenticate yourself.  
Press `Y` and hit Enter if you are not authenticated or if you wish to re-authenticate, Otherwise press `N` and hit Enter.

<!-- Once the installation is done, verify the `gh` installation. Run the below command to verify you already have `gh` installed and check the installed version.
This should show you the exact version of `gh` installed. -->

<!--wrappid_user@system:~$-->

<!-- ```terminal
gh --version
gh version 2.28.0 (2023-04-25)
https://github.com/cli/cli/releases/tag/v2.28.0
``` -->

> <br/>
>
> **_Note:_**
>
> _If you get an error during the course of execution of the command (`wrappid install`), or find that `gh` isn't working, which generally looks like the below:_
>
> ```terminal
> 'gh' is not recognized as an internal or external command,
> operable program or batch file.
> ```
>
> _Close all terminals/cmd and open a fresh terminal/cmd and run `gh` or `gh --version` to confirm GitHub CLI installation._
>
> _If `gh` still doesn't work, go to the [official documentation of GitHub CLI](https://github.com/cli/cli#installation) and install `gh` manually._
>
> _After successfull installation of GitHub CLI or `gh`, run `wrappid install` again._
>
> _If you are still not taken to authentication instructions, run `gh auth login` and complete your authentication manually._
>
> [Know more about GitHub CLI](https://cli.github.com/manual)
>
> <br/>

### 4. Setup `Wrappid` Project

#### 1. Initialize a `Wrappid` project

Run the below command to initialize a `Wrappid` project with a specified project name.

```terminal
wrappid init <project_name>
```

This will create 3 `Wrappid` projects with project names  
`<project_name>-app`  
`<project_name>-module` and  
`<project_name>-service`  
<!-- This will create 3 `Wrappid` projects with default project names `wrappid-app`, `wrappid-module` and `wrappid-service` -->

## `Wrappid Toolkit` Usage Documentation

Run the below command to find other `[command] [subcommand] [arguments] [options]` supported by the `Wrappid Toolkit`.

```terminal
wrappid --help
```
<!--
## Start Development Server


```
wrappid start
This should launch your default browser with a URL `http://localhost:3000`
```
-->
## Learn Wrappid in details

`Wrappid` Framework supports building frontend, backend (API middleware & DB handling) and business specific modules. The framework helps generate the below:

1. Frontend - `<wrappid>-app`
2. Backend - `<wrappid>-service`
3. Modules - `<wrappid>-module`

### 1. Frontend - `<wrappid>-app`

The `<wrappid>-app` is based on `React` and `React Native`.

Here, you **write code once** and use `Wrappid Toolkit` to build your web and mobile applications simultaneously.

Run the below command to create Frontend Wrappid Project

```terminal
wrappid init app <project_name>
```

### 2. Backend - `<wrappid> service`

The `<wrappid>-service` is based on `node` and `express`.

Here, the `Wrappid Toolkit` helps you build API middleware along with scripts to handle DB.

Run the below command to create Backend Wrappid Project

```terminal
wrappid init service <project_name>
```

### 3. Modules - `<wrappid>-module`

Run the below command to create Frontend Wrappid Project

```terminal
wrappid init module <project_name>
```
<!--
## Hi there 👋

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

# `Wrappid` CLI Tool

This is a npm package for our own `Wrappid` command line interface to create a `Wrappid` project.

## Requirements

- Node - 16
- React - 18.2.0
- React Native - 0.71.6


### Step 2

Choosing a template for your wrappid project.
Template(s) available for now as follows:

- Web: Using React 18.2.0
- Mobile: Using React Native 0.71.6

```

> Choose template
>
> 1. Web: Using React 18.2.0
> 2. Mobile: Using React Native 0.71.6

```

Based on your template selection your project will be prepared.

### Step 3

Start auto installation process.

### Step 4

Now you have a sample module for business module refference.

-->

### All commands for ref:
wrappid cli
Alias: `wcli`, `wr`.
```
wrappid [command] [subcommand] [arguments] [options]

This is a npm package to enable Wrappid Toolkit so that application developers
can use the wrappid command line interface to handle Wrappid projects.

Options:
  -V, --version          output the version number
  -h, --help             display help for command

Commands:
  install                This command will install all the pre-requisite such as:
                         a. Install GitHub CLI
                         b. Authenticate with GitHub A/c using GitHub CLI
  list [options]         Show list of wrappid projects in current working directory.
  list deps              Show list of project dependencies
  init <project-name>    Initialize app service module project using wrappid template.
  setup                  Setup [APP(web|mobile)|SERVICE] project.
  start                  Start [APP(web|mobile)|SERVICE] project.
  copy [options]         Copy src and res to web and mobile runtime.
  include <module-name>  Include module inside wrappid project
  exclude <module-name>  Exclude module from wrappid project
  add                    Include new modules into project directory (Not needed)
  build (web|android)    Create build for web or android
  reinstall (web|mobile) Reinstall wrappid packages for web or mobile
  update                 Update wrappid toolkit
  update modules         Update project modules
  update modules <name>  Update specified module, if module is included in project

wrappid install

wrappid init app test - old
wrappid init service test - old
wrappid init test - old

wrappid init <projectname>
wrappid init app <projectname>
wrappid init module <projectname>
wrappid init service <projectname>

wrappid setup web --env=(dev|stage|prod)
wrappid setup mobile --env=(dev|stage|prod)
wrappid setup service --env=(dev|stage|prod)

wrappid start web --env=(dev|stage|prod)
wrappid start mobile --env=(dev|stage|prod)
wrappid start service --env=(dev|stage|prod)

wrappid copy web
wrappid copy mobile

wrappid add <modulename> - old

wrappid build web
wrappid build android

```
wrappid-dev cli
Alias: `wdev`, `wd`.

```
Usage: wrappid-dev [command] [subcommand] [arguments] [options]

This is a npm package to enable Wrappid Developer Toolkit so that application developers
can use the wrappid command line interface to handle Wrappid projects.

Options:
  -V, --version     output the version number
  -h, --help        display help for command

Commands:
  init [path-to-wrappid-dev-home]                Initialize and setup wrappid development environment.
  reset                                          Removes wrappid dev environment configuration
  link [web|mobile]                            Link wdpkg (wrappid development packages) in web and mobile runtime.
  reload [web|mobile] --pkg [core|native|styles] Reload wdpkg (wrappid development packages) in web and mobile runtime
  
```
