# Wrapper Framework for Rapid development

<img src="https://github.com/wrappid/.github/blob/main/logo/logo-1200x400.png" width="50%" height="auto" />

## `Wrappid` Framework is a wrapper framework built to enable rapid development of applications.

`Wrappid` Framework is a wrapper framework built to enable rapid development of applications based on `React`, `React Native`, `Node`, `Express`, etc. Here, you **write code once** and use `Wrappid Toolkit` to build your web and mobile applications simultaneously.

`Wrappid` includes a repository of components, called the `CoreComponents`, for application developers to use. As application developers, you also have the flexibility to write your own components. By default the styling libraries used are `mui` for web and `react native paper` for mobile.

`Wrappid` also comes with a set of pre-coded business handling modules like app builder, user/role/permission management, authentication, authorization, error reporting, notifications (push/mail/sms/whatsapp), etc.

## Getting Started

This getting started section will help you setup a basic `Wrappid` project environment. The easiest way is to use the `Wrappid Toolkit`.

Follow the below steps to get going:

[1. Get Early Access to Wrappid](#1-get-early-access-to-wrappid)   
[2. Check Pre-requisites](#2-check-pre-requisites)   
[3. Install `Wrappid Toolkit`](#3-install-wrappid-toolkit)   
[4. One-time Initialisation](#4-one-time-initialisation)   
[5. Quick Start With Wrappid Project(s)](#5-quick-start-with-wrappid-projects)   

### 1. Get Early Access to Wrappid

Please fill [Wrappid Early Access Request form](https://forms.gle/NCUbSXvsX1v9QhD96) to get a valid `<WRAPPID_TOKEN>`. After filling the form you will receive the `<WRAPPID_TOKEN>` and Wrappiders Group link in your email. Make Sure to Join Wrappiders Group to receive important updates regarding Wrappid Framework.

The above mentioned_ `<WRAPPID_TOKEN>` _could only be used to read and download the `Wrappid` packages.   

We will use this token in later steps.

### 2. Check Pre-requisites

<!-- First you need to verify that your system fulfills the pre-requisites. Listed below are the things required to be available in your system. -->
Please verify the pre-requisites listed below:

Required for web app development:
- [Node.js - version 16.20.X](https://nodejs.org/en/blog/release/v16.20.0)
- npm - version 8.X.X

> **_Note:_** _If you have multiple node versions, to set up node 16.20.x & npm 8.x.x, follow the documentation [here](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)._  


**Check your version of Node.js and npm**

To see if you already have Node.js and npm installed and check the installed version, run the following commands:

```terminal
node -v
```
Expected output:   
v16.20.x

```terminal
npm -v
```
Expected output:   
8.x.x


> **_Note:_** _Above mentioned version is based on the time of documentation, 16.20.(x), 8.(x).(x), x may differ._


Required for mobile app development:
- Required steps for web app development
- JDK - 11 
- Android Studio
Recommended Code editor:   
- [VS Code](https://code.visualstudio.com/)/[VS Codium](https://vscodium.com/)



### 3. Install `Wrappid Toolkit`

To use `Wrappid Toolkit`, you need to setup scoped wrappid package registry and install `@wrappid/toolkit` globally in your system.

> **_Note:_**
> <!-- > _The `@wrappid/toolkit` is available in the GitHub npm package registry. You will have to setup scoped package registry as your npm runtime configuration._ -->
>
> _It is expected that you successfully went through [1. Get Early Access to Wrappid](#1-get-early-access-to-wrappid) section. If you don't, you won't be able to setup wrappid framework._

 _Run the below commands to setup scoped package registry:_

 <!--C:\Users\Wrappid>-->
Here we will use `<WRAPPID_TOKEN>` that is sent to your email.

 ```terminal
 npm config set @wrappid:registry https://npm.pkg.github.com/wrappid
```
```terminal
 npm config set //npm.pkg.github.com/:_authToken <WRAPPID_TOKEN>
 ```

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
```
Expected output:   
v0.0.107

> **_Note:_** _This is the  `Wrappid Toolkit` version at the time of this documentation._

### 4. One-time Initialisation

Run the below command to install all dependencies `Wrappid Toolkit` uses

```terminal
wrappid install
```

This one-time initialisation of `Wrappid Toolkit` follows the below steps:

- Install package dependencies
- Download & Install GitHub CLI or `gh` (if not already installed)
- Authenticate with GitHub A/c to use GitHub CLI or `gh`

#### 4.1. Install package dependencies

This is a automated process. You need not do anything.

#### 4.2. Download & Install GitHub CLI or `gh` (if not already installed)

This is a automated process but you will be prompted with GitHub CLI or `gh` installation. 

For Windows:   
Kindly click Next -> Next -> ... -> Finish to complete the GitHub CLI or `gh` installation.

For Linux:
Enter `sudo` password when prompted, and continue.

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
> _Make sure that your `gh cli` version is or above 2.40.0_
>
> _If `gh` still doesn't work, go to the [official documentation of GitHub CLI](https://github.com/cli/cli#installation) and install `gh` manually._
>
> _After successfull installation of GitHub CLI or `gh`, run `wrappid install` again._
>
> _If you are still not taken to authentication instructions, run `gh auth login` and complete your authentication manually._
>
> _[Know more about GitHub CLI](https://cli.github.com/manual)_
>
> <br/>

#### 4.3. Authenticate with GitHub A/c to use GitHub CLI or `gh`

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
```
gh version 2.28.0 (2023-04-25)
https://github.com/cli/cli/releases/tag/v2.28.0
 -->

<!--
### 4. `Wrappid` Project Setup

#### 1. Initialize a `Wrappid` project

Run the below command to initialize a `Wrappid` project with a specified project name.

```terminal
wrappid init <project_name>
```

This will create 3 `Wrappid` projects with project names  
`<project_name>-app`  
`<project_name>-module` and  
`<project_name>-service`  
-->

>**_Note_**: Now you can use the wrappid toolkit
>#### _`Wrappid Toolkit` Usage Documentation_
>
>_Run the below command to find other `[command] [subcommand] [arguments] [options]` supported by the `Wrappid Toolkit`._
>```terminal
>wrappid --help
>```

<!-- This will create 3 `Wrappid` projects, `<project_name>-app`, `<project_name>-module` and `<project_name>-service` -->
<!--
#### 2. Setup a `Wrappid` project.

##### 1. Setup `Wrappid-App` project.
After successfull initialization of a `wrappid-app`, change your directory to root of `<projectName>-<app>` wrappid project.

`Wrappid-App` has two runtime-environments, web and mobile.
Run the below command to setup a `wrappid-app` in web and mobile runtime-environments.

```bash
wrappid setup
```

Run the below command to setup a `wrappid-app` in web runtime-environment.

```bash
wrappid setup web
```

Run the below command to setup a `wrappid-app` in mobile runtime-environment.

```bash
wrappid setup mobile
```

##### 2. Setup `Wrappid-Service` project.
After successfull initialization of `wrappid-service`, change your directory to root of `<projectName>-<service>` wrappid project.

Run the below command to setup a wrappid-service:

```bash
wrappid setup service
```

#### 3. Start Your `Wrappid` project

##### 1. Start `Wrappid-App` project
After you are done with setup, you can start wrappid-app in two runtime-environments, web and mobile.  
Run the below command to start the development frontend server for web:
```bash
cd wrappid-app
wrappid start web
```

Run the below command to start the development server for mobile:
> _Note: You must have JDK 11 and Android Studio setup to start mobile_
```bash
cd wrappid-app
wrappid start mobile
```
##### 2. Start `Wrappid-Service` project

Run the below command to start the development backend service :

```bash
cd wrappid-service
wrappid start
```
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
## 5. Quick Start With Wrappid Project(s)

### 5.1 How to Create Wrappid Projects?
`Wrappid` Framework supports building frontend, backend (API middleware & DB handling) and business specific modules. Wrappid-Toolkit enables us to generates boilerplate applications.

1. [Frontend](https://github.com/wrappid/wrappid-app) - `<wrappid>-app`   
2. [Backend](https://github.com/wrappid/wrappid-service) - `<wrappid>-service`   
3. [Modules](https://github.com/wrappid/wrappid-module) - `<wrappid>-module`   

> **_Note:_** _It is understood that you have installed wrappid toolkit and initialized it successfully_

Run the below command to initialize a `Wrappid` project with a specified project name.

```terminal
wrappid init <project_name>
```

This will create 3 `Wrappid` project repositories with project names(user input) in your github account repository and 3 same 3 repositories locally with wrappid-modules at your path of command execution.
1. Frontend   
`<project_name>-app`  
2. Module   
`<project_name>-module`
3. Backend   
`<project_name>-service`  

#### Output

![init](https://github.com/wrappid/.github/assets/61864488/29bca9c0-74c8-4ea3-9264-877d206ac0f5)


### 5.2 How to Setup Wrappid Project?
To setup frontend wrappid-app in web or mobile, change directory to wrappid-app project

```terminal
cd <project_name>-app
wrappid setup [web|mobile]
```

To start backend wrappid-app, change directory to wrappid-service project

```terminal
cd <project_name>-service
wrappid setup
```

### 5.3 How to Start a Wrappid Project?

To start frontend wrappid-app in web or mobile, change directory to wrappid-app project

```terminal
cd <project_name>-app
wrappid start [web|mobile] --env=[dev|stage|prod]
```

To start backend wrappid-app, change directory to wrappid-service project

```terminal
cd <project_name>-service
wrappid start --env=[dev|stage|prod]
```

**Output**

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
<!-- 
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


``` -->
<!--
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

-->
