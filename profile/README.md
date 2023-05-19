<img src="https://github.com/wrappid/.github/blob/main/logo/logo-1200x400.png" />

<!--
```
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

This getting started section will help you setup a basic `Wrappid` project environment. The easiest way is to use the `Wrappid Toolkit`. Follow the below steps to get going.

1. Verify Pre-requisites
2. Install `Wrappid Toolkit`
3. Setup `Wrappid` Project(s)

### 1. Verify Pre-requisites

First you need to verify that your system fulfills the pre-requisites. Listed below are the things required to be available in your system.

- Node.js - version 16
- npm - version 8

#### Checking your version of Node.js and npm

To see if you already have Node.js and npm installed and check the installed version, run the following commands:

```
node -v
npm -v
```

#### Refer the exact version we use:

```
node -v
v16.18.1

npm -v
8.19.2
```

Please install them if they are not available in your system. Kindly follow original installation guide to do so.

### 2. Install `Wrappid Toolkit`

To setup `Wrappid Toolkit`, you need to install `Wrappid Toolkit` globally in your system.

> **_Note:_**
>
> _The `Wrappid Toolkit` is available in the GitHub npm pkg registry. You will have to setup scoped pkg registry as your npm runtime configuration._
>
> _Please fill **[this form](https://forms.gle/NCUbSXvsX1v9QhD96)** to get **<WRAPPID_TOKEN>**_
> 
> _Run the below commands to setup scoped pkg registry._
>
> <!--C:\Users\Sam>-->
>
> ```
> npm config set @wrappid:registry https://npm.pkg.github.com/wrappid
>
> npm config set //npm.pkg.github.com/:_authToken <WRAPPID_TOKEN>
> ```
>
> _The above mentioned authToken could only be used to read and download the `Wrappid Toolkit` package._

Run the below command to install `Wrappid Toolkit` globally in your system.

```
npm install -g @wrappid/toolkit
```

Once the installation is done, verify the `Wrappid Toolkit` installation. Run the below command to verify you already have `Wrappid Toolkit` installed and check the installed version

```
wrappid -v
```

This should show you the exact version of `Wrappid Toolkit` installed

```
wrappid -v
v0.0.14
```

### Setup `Wrappid` Project

#### 1. Initialize a `Wrappid` project

Run the below command to initialize a default `Wrappid` project

```
wrappid init
```

This will create a `Wrappid` project with default project name `wrappid-app`

#### 2. Initialize a `Wrappid` project with specific project name.

Run the below command to initialize a `Wrappid` project with a specified project name.

```
wrappid init <project_name>
```

This will create a `Wrappid` project with project name `<project_name>`

## Further Documentation

Run the below command to find other features supported by the `Wrappid Toolkit`.

```
wrappid --help
```

## Learn Wrappid in details

`Wrappid` Framework supports building frontend, backend (API middleware & DB handling) and business specific modules. The framework helps generate the below:

1. Frontend - `<wrappid>-app`
2. Backend - `<wrappid>-service`
3. Modules - `<wrappid>-module`

### 1. Frontend - `<wrappid>-app`

The `<wrappid>-app` is based on `React` and `React Native`.

Here, you **write code once** and use `Wrappid Toolkit` to build your web and mobile applications simultaneously.

### 2. Backend - `<wrappid>-service`

The `<wrappid>-service` is based on `node` and `express`.

Here, the `Wrappid Toolkit` helps you build API middleware along with scripts to handle DB.

### 3. Modules - `<wrappid>-module`

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

```

```
