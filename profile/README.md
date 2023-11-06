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
4. Get started with `Wrappid` Project(s)
5. Run `Wrappid` project.

### 1. Verify Pre-requisites

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
v16.20.0

npm -v
8.19.4
```

> **_Note:_** _Above mentioned version is based on the time of documentation, 16.20.(x), 8.(x).(x), x may differ._


Required for mobile app development:
- Required steps for web app development
- JDK - 11 
- Android Studio
Recommended Code editor:   
- [VS Code](https://code.visualstudio.com/)/[VS Codium](https://vscodium.com/)



### 2. Install `Wrappid Toolkit`

To use `Wrappid Toolkit`, you need to setup scoped wrappid package registry and install `@wrappid/toolkit` globally in your system.

> <br/>
>
> **_Note:_**
>
<!-- > _The `@wrappid/toolkit` is available in the GitHub npm package registry. You will have to setup scoped package registry as your npm runtime configuration._ -->
>
> _Please fill [Wrappid Early Access Request form](https://forms.gle/NCUbSXvsX1v9QhD96) to get a valid_ `<WRAPPID_TOKEN>`. After filling the form you will receive the `<WRAPPID_TOKEN>` in your email.
>
> _The above mentioned_ `<WRAPPID_TOKEN>` _could only be used to read and download the `Wrappid` packages._
>
> <br/>

 _Run the below commands to setup scoped package registry:_

 <!--C:\Users\Sam>-->

 ```terminal
 npm config set @wrappid:registry https://npm.pkg.github.com/wrappid

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
v0.0.100
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
> _If `gh` still doesn't work, go to the [official documentation of GitHub CLI](https://github.com/cli/cli#installation) and install `gh` manually._
>
> _After successfull installation of GitHub CLI or `gh`, run `wrappid install` again._
>
> _If you are still not taken to authentication instructions, run `gh auth login` and complete your authentication manually._
>
> _[Know more about GitHub CLI](https://cli.github.com/manual)_
>
> <br/>

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
## 4. Get started with `Wrappid` Project(s)

`Wrappid` Framework supports building frontend, backend (API middleware & DB handling) and business specific modules. Wrappid-Toolkit enables us to generates boilerplate applications.

1. Frontend - `<wrappid>-app`
2. Backend - `<wrappid>-service`
3. Modules - `<wrappid>-module`

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



> **_Note:_** _From now, we will refer <project_name> as <wrappid>_  

### 4.1. Frontend - `<wrappid>-app`

The `<wrappid>-app` is based on `React` and `React Native`.

Here, you **write code once** and use `Wrappid Toolkit` to run and build your web and mobile applications simultaneously.

Now we will learn:
1. Frontend runtime environments
2. Initialize a frontend wrappid-app
3. Set up a frontend wrappid-app

#### 4.1.1. Frontend runtime environments
Frontend `Wrappid-App` has two runtime-environments:
- Web
- Mobile

We will talk about these environments in upcomming sections.

#### 4.1.2. Initialize a frontend wrappid-app

Run the below command to create Frontend Wrappid Project

```terminal
wrappid init app <wrappid>
```

**Output:**  
![wrappid-app](https://github.com/wrappid/.github/assets/61864488/c7b6f0ae-bc7c-4008-87d0-96994839002a)


#### 4.1.3. Set up a frontend wrappid-app

Run the below command to setup a Frontend Wrappid Project in web and mobile runtime-environments.

```bash
cd <wrappid>-<app>
wrappid setup
```

Run the below command to setup a `wrappid-app` in web runtime-environment.

```bash
cd <wrappid>-<app>
wrappid setup web
```

Run the below command to setup a `wrappid-app` in mobile runtime-environment.

```bash
cd <wrappid>-<app>
wrappid setup mobile
```

### 4.2. Backend - `<wrappid>-service`

The `<wrappid>-service` is based on `node` and `express`.

Here, the `Wrappid Toolkit` helps you build API middleware along with scripts to handle DB.

Now we will learn to:
1. Initialize a backend wrappid-service
2. Set up a backend wrappid-service

in a similar manner as wrappid-app.

#### 4.2.1. Initialize a backend wrappid-service
Run the below command to create Backend Wrappid Project

```terminal
wrappid init service <wrappid>
```

**Output:**  
![wrappid-service](https://github.com/wrappid/.github/assets/61864488/b5c91ac7-f30f-48e7-b3f3-f0e736f27e95)


#### 4.2.2. Set up a backend wrappid-service
Run the below command to setup the development Backend Project :

```bash
cd <wrappid>-service
wrappid setup
```

> **_Note:_** _Backend wrappid-service doesn't have any runtime environments_


### 4.3. Module - `<wrappid>-module`

Now we will learn to:
1. Initialize a backend wrappid-service
2. Include or exclude a wrappid-module from `wrappid-[app|service]`

#### 4.3.1. Initialize a backend wrappid-service
Run the below command to create Module Wrappid Project

```terminal
wrappid init module <wrappid>
```

**Output:**  
![wrappid-module](https://github.com/wrappid/.github/assets/61864488/fc0f4866-43d5-4e3a-92a6-7b3e0aa768ab)


Now you have a `<wrappid>-<module>` Module Wrappid Project at the directory the command was executed from.

#### 4.3.2. Include or exclude a wrappid-module from `wrappid-[app|service]`

> **_Note:_** _You cannot setup or start a wrappid-module project like wrappid-app and wrappid-service._   

To use Wrappid module projects

- You need to `include` the module into your `wrappid-[app|service]`, from inside of the root of `wrappid-[app|service]`.
- Your module must be located in the parent directory of  `wrappid-[app|service]` project.
- Your `wrappid-[app|service]` should be setup.

Run the below command from the root of the `wrappid-[app|service]` project you wish to include your module.
```terminal
cd wrappid-[app|service]
wrappid include <module-name>
```

Make sure to not write `-module` following your <module-name>

Similarly, to exclude a module from your `wrappid-[app|service]`, run the below command.
```terminal
wrappid exclude <module>-name
```

Make sure to not write `-module` following your <module-name>

Wrappid modules are hot swappable, you can `include` and `exclude` a module while `wrappid-[app|service]` is running

### 5. Run `Wrappid` project.
Now time to see some action:
1. Start a Wrappid Frontend project
2. Start a Backend project
3. Wrappid Environments

### 5.1. Start a Wrappid Frontend project
You can start a frontend app in two modes:
- Static (Without Backend Service)
- Dynamic (With Backend Service)

- Static (Without Backend Service)
Run the below command to start the development frontend server for web:
```bash
cd wrappid-app
wrappid start web
```
By default wrappid-app web runtime env runs at `localhost:3000`

Run the below command to start the development server for mobile:

```bash
cd wrappid-app
wrappid start mobile
```

- Dynamic (With Backend Service)

To start Dynamic Fontend Wrappid project, you'll first need your Wrappid Backend up and running. [steps for backend](https://github.com/wrappid/#2-starting-backend-project).   
 - Enter you Backend URL in `wrappid.conf.json` file located at the root of `wrappid-app` project.
 - Follow the same steps for starting a [static frontend wrappid-app]()

### 5.2. Start a Backend project

To Start a Backend Wrappid Service project, follow below steps:

- Change directory to  `wrappid-service` project.
- Setup `wrappid-service` project. (Skip this step if you already setup)
- `Include` your `wrappid-modules` if any.
- Enter you database credential in `wrappid.conf.json` file located at the root of `wrappid-service` project.
- Finally run the below command to start your development Wrappid Backend Project
  ```terminal
  wrappid start
  ```
- By default, your backend will run at port : ``

### 5.3 Wrappid Environments
Wrappid projects can be runned in 3 environments:
- Dev: Suitable for Development
- Stage: Suitable for Testing
- Prod: Suitable for Testing

By default, Wrappid project setups and starts in `dev` environment.
These environments are to be configured in wrappid.conf.json located at the root of `wrappid-[app|service]` project

To run a Wrappid-[app|service] project in a different environment, run the below command:
```terminal
cd wrappid-app
wrappid start [web|mobile] --env=[dev|stage|prod]

```
```terminal
cd wrappid-service
wrappid start --env=[dev|stage|prod]
```

### Tips:
- The `cd` command changes the directory you're working with. In order to work with your newly created Wrappid-App, you'll need to navigate the terminal there.

- Do not edit runtime files

# Learn Wrappid In Details   
[Click here.]()
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
