---
title: "Download and Install Java 8 on Windows"
permalink: /download-install-java-8-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Java 8 on Windows."
date: 2018-06-19
last_modified_at: 2018-06-19
categories: [Development]
tags: [Download, Install, Java, Setup, Tutorial, Windows]
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/java/download-install-java-8-windows.png" alt="download install java 8 windows" class="align-right title-image">

In this tutorial you’ll learn everything you need to know on **how setup Java on Windows**.

Where to download it.

How it install it.

(And most important of all) how to check if everything is working.

Let’s start!

## Step #1: Download

Go to the [Java download page](https://java.com/en/download/manual.jsp){:target="_blank"}.

<img src="{{ site.url }}/assets/images/posts/development/java/java-download-page.jpg" alt="java download page">

Click on the `Windows Online` link.

<img src="{{ site.url }}/assets/images/posts/development/java/java-8-online-installer-link.jpg" alt="java 8 online installer link">

Wait for the download to complete.

> Do you want to skip above steps? Here is the direct link for the [Java online installer](http://javadl.oracle.com/webapps/download/AutoDL?BundleId=233169_512cd62ec5174c3487ac17c61aaa89e8){:target="_blank"} for Windows.

## Step #3: Install

Open the location of the downloaded installer.

<img src="{{ site.url }}/assets/images/posts/development/java/java-8-online-installer.jpg" alt="java 8 online installer">

Double-click on the installer. The Java setup welcome window opens.

Double-click on `Install >`.

<img src="{{ site.url }}/assets/images/posts/development/java/java-8-installer-welcome.jpg" alt="java 8 installer welcome">

A Java setup window appears (this might take a few seconds).

The green bar shows the installation progress.

Wait for the installation to complete.

<img src="{{ site.url }}/assets/images/posts/development/java/java-8-installer-installing.jpg" alt="java 8 installer installing">

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

Drop a line below if you liked this post.

Thanks!
