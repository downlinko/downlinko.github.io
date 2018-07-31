---
title: "Download and Install JDK 1.8 on Windows"
permalink: /download-install-jdk-8-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install JDK 8u181 on Windows 10."
date: 2018-07-30
last_modified_at: 2018-07-30
header:
  teaser: "assets/images/posts/development/jdk/download-install-jdk-8-windows.png"
categories: [Development]
tags: [Download, Install, JDK, JDK 1.8, Setup, Tutorial, Windows]
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/jdk/download-install-jdk-8-windows.png" alt="download install jdk 8 windows" class="align-right title-image">

In this guide I’m going to show you exactly how to download and install JDK 1.8 on Windows.

(Step-by-step)

First, I’ll show you where you can download JDK 8.

Then you’ll see how to configure it.

And finally **how to check if everything is working**.

Let’s dive right in…

## Step #1: Download

There are [several Java packages available](https://docs.oracle.com/javaee/6/firstcup/doc/gkhoy.html){:target="_blank"}. In this tutorial, we will install the Java Standard Edition (SE) platform.

Java SE contains a **Java Development Kit** (JDK) that comes with a Java compiler. It also has a Java runtime environment (JRE) that can run compiled Java code.

Head over to the [Oracle Java download page](http://www.oracle.com/technetwork/java/javase/downloads/index.html){:target="_blank"}.

Look for the `Java SE 8u181` section.

Click on the `Download` button right below `JDK`.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-8-download-java-se.png" alt="jdk 8 download java se">

Click on the radio button next to `Accept License Agreement`.

Click on the download link for your Windows version.

In this guide we will download the 64-bit installer: `jdk-8u181-windows-x64.exe`.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-8-download-java-se-windows-binary.png" alt="jdk 8 download java se windows binary">

Wait for the download to complete.

## Step #2: Install

Open the location of the downloaded executable.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-8-downloaded-installer.png" alt="jdk 8 downloaded installer">

Double-click it to run the installer.

Click `Next`.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-8-installer-start.png" alt="jdk 8 installer start">

You can change the installation location by clicking on the `Change…` button.

In this example, we keep the default install location of `C:\Program Files\Java\jdk1.8.0_181`. From now on we will refer to this directory as `[JAVA_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-8-installer-default-location.png" alt="jdk 8 installer default location">

We will not install the public JRE as the JDK development tools already include a private JRE.

Select the `Public JRE` dropdown and click on `This feature will not be available.` as shown below.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-8-installer-disable-public-jre.png" alt="jdk 8 installer disable public jre">

Click `Next` to start the installation.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-8-installer-custom-setup.png" alt="jdk 8 installer custom setup">

Once the installation is complete, click `Close`.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-8-installer-complete.png" alt="jdk 8 installer complete">

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

In this tutorial, the Java installation directory is `C:\Program Files\Java\jdk1.8.0_181`.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-8-home-variable.png" alt="jdk 8 home variable">

Next, we need to configure the PATH environment variable so we can run Java from a command prompt.

Select the `Path` variable. Click on `Edit…`.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-8-edit-path-variable.png" alt="jdk 8 edit path variable">

Click on `New` and type "<kbd>%JAVA_HOME%\bin</kbd>" as shown below.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-edit-path-variable-add-java-home.png" alt="jdk edit path variable add java home">

Click `OK` once more to close the environment variables window.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-8-windows-account-environment-variables.png" alt="jdk 8 windows account environment variables">

> If a `Path` variable does not exist you need to create it. Use "<kbd>Path</kbd>" as variable name and "<kbd>%JAVA_HOME%\bin</kbd>" as variable value.

> On Windows 7 you cannot add extra values for an existing `Path` variable. You need to append "<kbd>;%JAVA_HOME%\bin</kbd>" at the end of the variable value instead.

## Step #4: Test

Let's test the setup.

Click on the search button. Then type "<kbd>env</kbd>" (without quotes).

Click on the `Command Prompt` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Type "<kbd>java -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-version-command.png" alt="jdk version command">

The above command prints the installed JDK version: `1.8.0_181`.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-8-version-output.png" alt="jdk 8 version output">

**Congratulations, you have installed JDK 1.8 on Windows 10!**

Now let me know if you liked this post.

Leave a comment below.

Thanks!