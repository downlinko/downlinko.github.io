---
title: "Download and Install Maven 3.3.9 on Windows"
permalink: /download-install-maven-3-3-9-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Apache Maven 3.3.9 on Windows."
date: 2018-07-21
last_modified_at: 2018-07-21
categories: [Development]
tags: [Download, Install, Maven, Setup, Tutorial, Windows]
published: false
---

<img src="{{ site.url }}/assets/images/posts/development/maven/download-install-maven-3-3-9-windows.png" alt="download install maven 3-3-9 windows" class="align-right title-image">

Do you want to download and install Maven 3.3.9 on Windows?

Then Check this out:

In this tutorial I'll show where to download Maven.

**How to configure it**.

(And above all) how to check if everything is working.

Let's get down to it!

## Step #1: Check Prerequisites

Maven requires [Java](http://www.oracle.com/technetwork/java/javase/downloads/index.html){:target="_blank"} to work. So let's check if you have Java on your system.

Click on the Windows button. Then type "<kbd>cmd</kbd>" in the search box and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Click on the `cmd` shortcut. Wait for the command prompt to open.

Type "<kbd>java -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/java-version-command.png" alt="java version command">

The above command prints the installed Java version.

<img src="{{ site.url }}/assets/images/posts/development/java-installed-version.png" alt="java installed version">

> For Maven 3 you need Java version 1.7 or higher.

## Step #2: Download

Go to the [Gradle releases page](https://gradle.org/releases/){:target="_blank"}.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-releases-page.jpg" alt="gradle releases page">

Scroll down to `v3.5.1` and click on the `binary-only` link.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-3-5-1-release.jpg" alt="gradle 3.5.1 release">

Wait for the download to complete.

> Do you want to skip above steps? Here is the direct link to download the [Gradle 3.5.1 binary-only installer](https://gradle.org/next-steps/?version=3.5.1&format=bin){:target="_blank"} for Windows.

## Step #3: Install

Open the location of the downloaded installer.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-3-5-1-downloaded-installer.jpg" alt="gradle 3.5.1 downloaded installer">

Right-click the ZIP archive file. Select `Extract All...`.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-3-5-1-installer-extract-all.jpg" alt="gradle 3.5.1 installer extract all">

Select an extract destination for the Gradle files.

In this example, we extract in `C:\Users\Downlinko\tools`.

<img src="{{ site.url }}/assets/images/posts/development/tools-extract-destination.jpg" alt="tools-extract-destination">

Click on `Extract`. This extracts all Gradle files under `C:\Users\Downlinko\tools\gradle-3.5.1`.

> From now on we refer to this location as `[GRADLE_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-3-5-1-home.jpg" alt="gradle 3.5.1 home">

## Step #4: Setup

Click on the Windows button. Then type "<kbd>env</kbd>" in the search box and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-env.jpg" alt="windows search env">

Click on the `Edit environment variables for your account` shortcut. Wait for the environment variables window to open.

<img src="{{ site.url }}/assets/images/posts/development/windows-environment-variables.jpg" alt="windows environment variables">

Click on `New...`.

<img src="{{ site.url }}/assets/images/posts/development/windows-environment-variables-new.jpg" alt="windows environment variables new">

Enter "<kbd>GRADLE_HOME</kbd>" as variable name. Enter the `[GRADLE_INSTALL_DIR]` as variable value. Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-3-5-1-home-variable.jpg" alt="gradle 3.5.1 home variable">

Select the `PATH` variable. Click on `Edit...`.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-3-5-1-edit-path-variable.jpg" alt="gradle 3.5.1 edit path variable">

Append "<kbd>;%GRADLE_HOME%\bin</kbd>" at the end of the variable value. Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-3-5-1-path-variable.jpg" alt="gradle 3.5.1 path variable">

Click `OK` once more to close the environment variables window.

## Step #5: Test

To test the setup click on the Windows button. Type "<kbd>cmd</kbd>" in the search box and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.jpg" alt="windows search cmd">

Click on the `cmd` shortcut. Wait for the command prompt to open.

Type "<kbd>gradle -v</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-version-command.jpg" alt="gradle-version-command">

The above command prints the installed Gradle version.

<img src="{{ site.url }}/assets/images/posts/development/gradle/gradle-3-5-1-version-output.jpg" alt="gradle 3.5.1 version output">

**Congratulations, you have installed Gradle 3.5.1 on Windows!**

Good luck and let me know if you liked this post.

Thanks!
