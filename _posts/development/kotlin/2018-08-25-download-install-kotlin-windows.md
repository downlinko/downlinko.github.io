---
title: "Download and Install Kotlin on Windows"
permalink: /download-install-kotlin-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Kotlin on Windows 10."
date: 2018-08-25
last_modified_at: 2018-08-25
header:
  teaser: "assets/images/posts/development/kotlin/download-install-kotlin-windows.png"
categories: [Development]
tags: [Download, Install, Kotlin, Setup, Tutorial, Windows]
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/kotlin/download-install-kotlin-windows.png" alt="download install kotlin windows" class="align-right title-image">

So you want to download and install [Kotlin](https://kotlinlang.org/){:target="_blank"} on Windows?

Then look no further!

In this guide, you’ll learn how to download the compiler…

…and how to configure it so you can use it from command line.

So let's fire away:

## Step #1: Check Prerequisites

Kotlin needs a [JDK](http://www.oracle.com/technetwork/java/javase/downloads/index.html){:target="_blank"} to work. So let's check if you have one configured on your system.

Click on the search button. Then type "<kbd>cmd</kbd>" (without quotes).

> On Windows 7 click on the Windows button.

Click on the `Command Prompt` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Type "<kbd>javac -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/jdk-version-command.png" alt="jdk version command">

The above command prints the installed JDK version.

<img src="{{ site.url }}/assets/images/posts/development/jdk-installed-version.png" alt="jdk installed version">

> For Kotlin you need JDK version 1.6 or higher.

If you do not have a Java Development Kit installed on your system. Check following post which details [how to install a JDK on Windows 10]({{ site.url }}/download-install-jdk-8-windows.html).

## Step #2: Download

Go to the [Kotlin Latest Release](https://github.com/JetBrains/kotlin/releases/latest){:target="_blank"} page on GitHub.

Click on the `kotlin-compiler-X.X.X.zip` link under the `Assets` section.

At the time of writing the latest stable Kotlin release was version `1.2.61`.

<img src="{{ site.url }}/assets/images/posts/development/kotlin/kotlin-latest-stable-release.png" alt="kotlin latest stable release">

Wait for the download to complete.

## Step #3: Install

Open the location of the downloaded installer.

<img src="{{ site.url }}/assets/images/posts/development/kotlin/kotlin-downloaded-compiler.png" alt="kotlin downloaded compiler">

Right-click the ZIP archive file. Select `Extract All…`.

<img src="{{ site.url }}/assets/images/posts/development/kotlin/kotlin-downloaded-compiler-extract-all.png" alt="kotlin downloaded compiler extract all">

Select an extract destination for the Kotlin files.

In this example, we extract in `C:\Users\Downlinko\tools\kotlin`.

<img src="{{ site.url }}/assets/images/posts/development/kotlin/kotlin-extract-destination.png" alt="kotlin extract destination">

Click on `Extract`. This extracts all kotlin files under `C:\Users\Downlinko\tools\kotlin\kotlinc`.

> From now on we refer to this location as `[KOTLIN_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/kotlin/kotlin-install-dir.png" alt="kotlin install dir">

## Step #4: Setup

We need to set up an environment variable that will point to our Kotlin installation.

Click on the search button. Then type "<kbd>env</kbd>".

> On Windows 7 click on the Windows button.

Click on the `Edit environment variables for your account` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-env.png" alt="windows search env">

Wait for the environment variables window to open.

Click on `New…`.

<img src="{{ site.url }}/assets/images/posts/development/windows-account-environment-variables-jdk-new.png" alt="windows account environment variables jdk new">

Enter "<kbd>KOTLIN_HOME</kbd>" as variable name. Enter the `[KOTLIN_INSTALL_DIR]` as variable value.

In this tutorial the installation directory is: `C:\Users\Downlinko\tools\kotlin\kotlinc`.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/kotlin/kotlin-home-variable.png" alt="kotlin home variable">

Next, we need to configure the PATH environment variable so we can run Kotlin from a command prompt.

Select the `PATH` variable. Click on `Edit…`.

<img src="{{ site.url }}/assets/images/posts/development/kotlin/kotlin-edit-path-variable.png" alt="kotlin edit path variable">

Click on `New` and type "<kbd>%KOTLIN_HOME%\bin</kbd>" as shown below.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/kotlin/kotlin-path-variable.png" alt="kotlin path variable">

Click `OK` once more to close the environment variables window.

<img src="{{ site.url }}/assets/images/posts/development/kotlin/kotlin-windows-account-environment-variables.png" alt="kotlin windows account environment variables">

> On Windows 7 you cannot add extra values for an existing `Path` variable. You need to append "<kbd>;%KOTLIN_HOME%\bin</kbd>" at the end of the variable value instead.

## Step #5: Test

To test the setup click on the search button. Then type "<kbd>cmd</kbd>".

Click on the `Command Prompt` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Type "<kbd>kotlinc -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/kotlin/kotlin-version-command.png" alt="kotlin version command">

The above command prints the installed Kotlin version.

<img src="{{ site.url }}/assets/images/posts/development/kotlin/kotlin-version-output.png" alt="kotlin version output">

**Congratulations, you have installed Kotlin on Windows 10!**

Be sure to leave a comment if you liked this post.

Thanks!
