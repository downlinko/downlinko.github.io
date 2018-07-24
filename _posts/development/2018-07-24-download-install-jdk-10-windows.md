---
title: "Download and Install JDK 10 on Windows"
permalink: /download-install-jdk-10-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install JDK 10 on Windows."
date: 2018-07-24
last_modified_at: 2018-07-24
categories: [Development]
tags: [Download, Install, JDK, Setup, Tutorial, Windows]
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/jdk/download-install-jdk-10-windows.png" alt="download install jdk 10 windows" class="align-right title-image">

I’m going to show you exactly how to download and install JDK 10 on Windows.

(Step-by-step)

First, I’ll show you where you can download JDK 10.

Then you’ll see how to configure it.

(And above all) **how to check if everything is working**.

Let’s dive right in…

## Step #1: Download

There are a number of [different Java packages available](https://docs.oracle.com/javaee/6/firstcup/doc/gkhoy.html){:target="_blank"}. In this tutorial we will be installing the Java Standard Edition (SE) platform.

It contains a **Java Development Kit** (JDK) package that comes with a Java compiler. It also has a Java runtime environment (JRE) that can run compiled Java code.

Head over to the [Oracle Java download page](http://www.oracle.com/technetwork/java/javase/downloads/index.html){:target="_blank"}.

Look for the `Java SE 10.0.2` section.

Click on the `Download` button right below `JDK`.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-10-download-java-se.png" alt="jdk 10 download java se">

Click on radio button next to `Accept License Agreement`.

Click on the Windows download link: `jdk-10.0.2_windows-x64_bin.exe`.

<img src="{{ site.url }}/assets/images/posts/development/jdk/jdk-10-download-java-se-windows-binary" alt="jdk 10 download java se windows binary">

Click on the `apache-maven-3.3.9-bin.zip` link.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-binaries.png" alt="maven 3-3-9 binaries">

Wait for the download to complete.

> Do you want to skip above steps? Here is the direct link to download the [Maven 3.3.9 installer](https://archive.apache.org/dist/maven/maven-3/3.3.9/binaries/apache-maven-3.3.9-bin.zip){:target="_blank"} for Windows.

## Step #3: Install

Open the location of the downloaded installer.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-downloaded-binary.png" alt="maven 3-3-9 downloaded binary">

Right-click the ZIP archive file. Select `Extract All...`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-downloaded-binary-extract-all.png" alt="maven 3-3-9 downloaded binary extract all">

Select an extract destination for the Maven files.

In this example, we extract in `C:\Users\Downlinko\tools`.

<img src="{{ site.url }}/assets/images/posts/development/tools-extract-destination.jpg" alt="tools-extract-destination">

Click on `Extract`. This extracts all Maven files under `C:\Users\Downlinko\tools\apache-maven-3.3.9`.

> From now on we refer to this location as `[MAVEN_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-install-dir.png" alt="maven 3-3-9 install dir">

## Step #4: Setup

We need to set up an environment variable that will point to our Maven installation.

Click on the Windows button. Then type "<kbd>env</kbd>" in the search box and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-env.png" alt="windows search env">

Click on the `Edit environment variables for your account` shortcut. Wait for the environment variables window to open.

<img src="{{ site.url }}/assets/images/posts/development/windows-account-environment-variables-jdk.png" alt="windows account environment variables jdk">

Click on `New...`.

<img src="{{ site.url }}/assets/images/posts/development/windows-account-environment-variables-jdk-new.png" alt="windows account environment variables jdk new">

Enter "<kbd>M2_HOME</kbd>" as variable name. Enter the `[MAVEN_INSTALL_DIR]` as variable value.

In this tutorial the installation directory is: `C:\Users\Downlinko\tools\apache-maven-3.3.9`.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-home-variable.png" alt="maven 3-3-9 home variable">

Next we need to configure the PATH environment variable so we can run Maven from a command prompt.

Select the `PATH` variable. Click on `Edit...`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-edit-path-variable.png" alt="maven 3-3-9 edit path variable">

Append "<kbd>;%M2_HOME%\bin</kbd>" at the end of the variable value.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-path-variable.png" alt="maven 3-3-9 path variable">

Click `OK` once more to close the environment variables window.

> If a PATH variable does not exist you need to create it. Use "<kbd>PATH</kbd>" as variable name and "<kbd>%M2_HOME%\bin</kbd>" as variable value.

## Step #5: Test

To test the setup click on the Windows button. Type "<kbd>cmd</kbd>" in the search box and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Click on the `cmd` shortcut. Wait for the command prompt to open.

Type "<kbd>mvn -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-version-command.png" alt="maven-version-command">

The above command prints the installed Maven version.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-version-output.png" alt="maven 3-3-9 version output">

**Congratulations, you have installed Maven 3.3.9 on Windows!**

Good luck and let me know if you liked this post.

Thanks!
