---
title: "Download and Install Visual Studio Code on Windows"
permalink: /download-install-visual-studio-code-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Visual Studio Code on Windows."
date: 2018-08-18
last_modified_at: 2018-08-18
header:
  teaser: "assets/images/posts/development/editors/download-install-visual-studio-code-windows.png"
categories: [Development]
tags: [Code Editor, Download, Install, Setup, Tutorial, Visual Studio, Windows]
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/editors/download-install-visual-studio-code-windows.png" alt="download install visual studio code windows" class="align-right title-image">

Today you’re going to learn how to download and install [Visual Studio Code](https://code.visualstudio.com/){:target="_blank"} on Windows.

(FAST)

I’m going to show you where to get the installer. And how to run the setup.

Let’s jump right in…

## Step #1: Download

Head over to the [Visual Studio Code downloads page](https://code.visualstudio.com/#alt-downloads){:target="_blank"}.

There are three Windows installer versions available:
1. User installer: Installs in your User folder and does not need Administrator privileges.
2. System installer: Installs for all users on the system and needs Administrator privileges.
3. .zip installer: a portable version.

> [Note that the User setup is recommended since version 1.26](https://code.visualstudio.com/updates/v1_26#_user-setup-for-windows){:target="_blank"}.

[Check your windows bit version]({{ site.url }}/windows-10-bit-version-check.html) and click on the corresponding link.

In this guide we will download the 64 bit User installer.

<img src="{{ site.url }}/assets/images/posts/development/editors/visual-studio-code-download-user-installer.png" alt="visual studio code download user installer">

Wait for the download to complete.

## Step #2: Install

Open the location of the downloaded executable.

<img src="{{ site.url }}/assets/images/posts/development/editors/visual-studio-code-downloaded-installer.png" alt="visual-studio-code-downloaded-installer">

Double-click it to run the installer.

Click `Next`.

<img src="{{ site.url }}/assets/images/posts/development/editors/visual-studio-code-installer-start.png" alt="visual studio code installer start">

Click on the radio button next to `I accept the agreement`.

Click `Next`.

<img src="{{ site.url }}/assets/images/posts/development/editors/visual-studio-code-installer-license-agreement.png" alt="visual studio code installer license agreement">

You can change the installation location by clicking on the `Browse…` button.

In this example, we keep the default install location.

Click `Next`.

<img src="{{ site.url }}/assets/images/posts/development/editors/visual-studio-code-installer-destination-location.png" alt="visual studio code installer destination location">

Keep the default Start Menu Folder.

Click `Next`.

<img src="{{ site.url }}/assets/images/posts/development/editors/visual-studio-code-installer-start-menu-folder.png" alt="visual studio code installer start menu folder">

Select the `Create a desktop icon` checkbox.

Click `Next`.

<img src="{{ site.url }}/assets/images/posts/development/editors/visual-studio-code-installer-additional-tasks.png" alt="visual studio code installer additional tasks">

An overview of the selected installation settings are shown.

Click `Install` to start the installation.

<img src="{{ site.url }}/assets/images/posts/development/editors/visual-studio-code-installer-ready-to-install.png" alt="visual studio code installer ready to install">

The Visual Studio Code installation will now start.

A progress bar shows the various steps that are executed.

<img src="{{ site.url }}/assets/images/posts/development/editors/visual-studio-code-installer-progress.png" alt="visual studio code installer progress">

Once the installation is complete, click `Finish`.

<img src="{{ site.url }}/assets/images/posts/development/editors/visual-studio-code-installer-finish.png" alt="visual studio code installer finish">

## Step #3: Run

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

Click on the search button. Then type "<kbd>cmd</kbd>" (without quotes).

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
