---
title: "Download and Install Gradle 4.1 on Windows"
permalink: /download-install-gradle-4-1-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Gradle 4.1 on Windows 10."
date: 2018-08-23
last_modified_at: 2018-08-23
header:
  teaser: "assets/images/posts/development/gradle/download-install-gradle-4-1-windows.png"
categories: [Development]
tags: [Download, Gradle, Install, Setup, Tutorial, Windows]
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/gradle/download-install-gradle-4-1-windows.png" alt="download install gradle 4.1 windows" class="align-right title-image">

Do you need to download and install [Gradle](https://gradle.org/){:target="_blank"} 4.1 on Windows?

You’ve reached the right place.

Because in this tutorial **I'll walk you through the different setup steps**.

Off we go!

Check following post if you are looking to download and install [Gradle 3.5]({{ site.url }}/download-install-gradle-3-5-windows.html).
{: .notice--primary}

## Step #1: Check Prerequisites

Gradle requires [Java](http://www.oracle.com/technetwork/java/javase/downloads/index.html){:target="_blank"} to work. So let's check if you have Java configured on your system.

Click on the search button. Then type "<kbd>cmd</kbd>" (without quotes).

> On Windows 7 click on the Windows button.

Click on the `Command Prompt` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Type "<kbd>java -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/java-version-command.png" alt="java version command">

The above command prints the installed Java version.

<img src="{{ site.url }}/assets/images/posts/development/java-installed-version.png" alt="java installed version">

> For Gradle 4.1 you need Java version 1.7 or higher.

If you do not have Java installed on your system. Check following post which details [how to install a JDK on Windows 10]({{ site.url }}/download-install-jdk-8-windows.html).

## Step #2: Download

Go to the [Gradle releases page](https://gradle.org/releases/){:target="_blank"}.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-releases-page.png" alt="gradle releases page">

Scroll down to `v4.1` and click on the `binary-only` link.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-4-1-release.png" alt="gradle 4-1 release">

Wait for the download to complete.

> Do you want to skip above steps? Here is the direct link to download the [Gradle 4.1 binary-only installer](https://gradle.org/next-steps/?version=4.1&format=bin){:target="_blank"} for Windows.

## Step #3: Install

Open the location of the downloaded installer.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-4-1-downloaded-installer.png" alt="gradle 4-1 downloaded installer">

Right-click the ZIP archive file. Select `Extract All…`.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-4-1-downloaded-installer-extract-all.png" alt="gradle 4-1 downloaded installer extract all">

Select an extract destination for the Gradle files.

In this example, we extract in `C:\Users\Downlinko\tools\gradle`.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-extract-destination.png" alt="tools-extract-destination">

Click on `Extract`. This extracts all Gradle files under `C:\Users\Downlinko\tools\gradle\gradle-4-1`.

> From now on we refer to this location as `[GRADLE_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-4-1-install-dir.png" alt="gradle 4-1 install dir">

## Step #4: Setup

We need to set up an environment variable that will point to our Maven installation.

Click on the search button. Then type "<kbd>env</kbd>".

> On Windows 7 click on the Windows button.

Click on the `Edit environment variables for your account` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-env.png" alt="windows search env">

Wait for the environment variables window to open.

Click on `New…`.

<img src="{{ site.url }}/assets/images/posts/development/windows-account-environment-variables-jdk-new.png" alt="windows account environment variables jdk new">

Enter "<kbd>GRADLE_HOME</kbd>" as variable name. Enter the `[GRADLE_INSTALL_DIR]` as variable value.

In this tutorial the installation directory is: `C:\Users\Downlinko\tools\gradle\gradle-4.1`.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-4-1-home-variable.png" alt="gradle 4-1 home variable">

Next, we need to configure the PATH environment variable so we can run Maven from a command prompt.

Select the `PATH` variable. Click on `Edit…`.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-4-1-edit-path-variable.png" alt="gradle 4-1 edit path variable">

Click on `New` and type "<kbd>%GRADLE_HOME%\bin</kbd>" as shown below.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-path-variable.png" alt="gradle path variable">

Click `OK` once more to close the environment variables window.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-4-1-windows-account-environment-variables.png" alt="gradle 4-1 windows account environment variables">

> On Windows 7 you cannot add extra values for an existing `Path` variable. You need to append "<kbd>;%GRADLE_HOME%\bin</kbd>" at the end of the variable value instead.

## Step #5: Test

To test the setup click on the search button. Then type "<kbd>cmd</kbd>".

Click on the `Command Prompt` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Type "<kbd>gradle -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-version-command.png" alt="gradle-version-command">

The above command prints the installed Gradle version.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-4-1-version-output.png" alt="gradle 4-1 version output">

**Congratulations, you have installed Gradle 4.1 on Windows 10!**

Drop a line below if you liked this post.

Thanks!
