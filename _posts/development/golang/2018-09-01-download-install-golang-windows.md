---
title: "Download and Install Golang on Windows"
permalink: /download-install-golang-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Golang on Windows 10."
date: 2018-09-01
last_modified_at: 2018-09-01
header:
  teaser: "assets/images/posts/development/golang/download-install-golang-windows.png"
categories: [Development]
tags: [Download, Go, Golang, Install, Setup, Tutorial, Windows]
published: false
---

<img src="{{ site.url }}/assets/images/posts/development/golang/download-install-golang-windows.png" alt="download install golang windows" class="align-right title-image">

So you want to download and install the [Go programming language](https://golang.org/){:target="_blank"} on Windows?

Then look no further!

In this guide, you’ll learn how to download the compiler…

…and how to configure it so you can use it from command line.

So let's fire away:

## Step #1: Download

Head over to the [Golang downloads page](https://golang.org/dl/){:target="_blank"}. Here you will find a number of binary releases available.

[Verify your windows bit version]({{ site.url }}/windows-10-bit-version-check.html) and click on the corresponding link under the `Stable versions` section:

* For 32-bit = <kbd>goX.XX.windows-386.msi</kbd>
* For 64-bit = <kbd>goX.XX.windows-amd64.msi</kbd>

In this tutorial, we will download the `64-bit` version.

At the time of writing the latest stable Golang release was version: `1.11`.

<img src="{{ site.url }}/assets/images/posts/development/golang/golang-latest-binary-release-page.png" alt="golang latest binary release-page">

Wait for the download to complete.

## Step #2: Install

Open the location of the downloaded executable.

<img src="{{ site.url }}/assets/images/posts/development/golang/golang-downloaded-installer.png" alt="golang downloaded installer">

Double-click it to run the installer.

On Windows 10 a pop-up window will appear: `The app you're trying to install isn't a verified app from the Store`

Click on `Install anyway`.

<img src="{{ site.url }}/assets/images/posts/windows-10-install-app-not-in-store.png" alt="windows 10 install app not in store">

The Golang installer wizard will start. Click `Next`.

<img src="{{ site.url }}/assets/images/posts/development/golang/golang-installer-start.png" alt="golang installer start">

Make sure the `I accept the terms in License Agreement` checkbox is selected. Click `Next`.

<img src="{{ site.url }}/assets/images/posts/development/golang/golang-installer-license-agreement.png" alt="golang installer license agreement">

You can change the installation location by clicking on the `Change…` button.

In this example, we keep the default install location of `C:\Program Files\Java\jdk-10.0.2\`. From now on we will refer to this directory as `[JAVA_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/golang/jdk-10-installer-default-location.png" alt="jdk 10 installer default location">

We will not install the public JRE as the JDK development tools already include a private JRE.

Select the `Public JRE` dropdown and click on `This feature will not be available.` as shown below.

<img src="{{ site.url }}/assets/images/posts/development/golang/jdk-10-installer-disable-public-jre.png" alt="jdk 10 installer disable public jre">

Click `Next` to start the installation.

<img src="{{ site.url }}/assets/images/posts/development/golang/jdk-10-installer-custom-setup.png" alt="jdk 10 installer custom setup">

The JDK installation will now start.

A progress bar shows the various steps that are executed.

<img src="{{ site.url }}/assets/images/posts/development/golang/jdk-10-installer-progress.png" alt="jdk 10 installer progress">

Once the installation is complete, click `Close`.

<img src="{{ site.url }}/assets/images/posts/development/golang/jdk-10-installer-complete.png" alt="jdk 10 installer complete">

## Step #3: Setup

We need to set up an environment variable that will point to our JDK installation.

Click on the search button. Then type "<kbd>env</kbd>" (without quotes).

> On Windows 7 click on the Windows button.

Click on the `Edit environment variables for your account` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-env.png" alt="windows search env">

Wait for the environment variables window to open.

Click on `New…`.

<img src="{{ site.url }}/assets/images/posts/development/windows-account-environment-variables-new.png" alt="windows account environment variables new">

Enter "<kbd>JAVA_HOME</kbd>" as variable name. Enter the `[JAVA_INSTALL_DIR]` as variable value.

In this tutorial, the Java installation directory is `C:\Program Files\Java\jdk-10.0.2`.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/golang/jdk-10-home-variable.png" alt="jdk 10 home variable">

Next, we need to configure the PATH environment variable so we can run Java from a command prompt.

Select the `Path` variable. Click on `Edit…`.

<img src="{{ site.url }}/assets/images/posts/development/golang/jdk-edit-path-variable.png" alt="jdk edit path variable">

Click on `New` and type "<kbd>%JAVA_HOME%\bin</kbd>" as shown below.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/golang/jdk-10-edit-path-variable-add-java-home.png" alt="jdk 10 edit path variable add java home">

Click `OK` once more to close the environment variables window.

<img src="{{ site.url }}/assets/images/posts/development/golang/jdk-10-windows-account-environment-variables.png" alt="jdk 10 windows account environment variables">

> If a `Path` variable does not exist you need to create it. Use "<kbd>Path</kbd>" as variable name and "<kbd>%JAVA_HOME%\bin</kbd>" as variable value.

> On Windows 7 you cannot add extra values for an existing `Path` variable. You need to append "<kbd>;%JAVA_HOME%\bin</kbd>" at the end of the variable value instead.

## Step #4: Test

Let's test the setup.

Click on the search button. Then type "<kbd>cmd</kbd>" (without quotes).

Click on the `Command Prompt` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Type "<kbd>java -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-version-command.png" alt="jdk version command">

The above command prints the installed JDK version: `10.0.2`.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-10-version-output.png" alt="jdk 10 version output">

**Congratulations, you have installed JDK 1.10 on Windows 10!**

Now let me know if you liked this post.

Leave a comment below.

Thanks!
