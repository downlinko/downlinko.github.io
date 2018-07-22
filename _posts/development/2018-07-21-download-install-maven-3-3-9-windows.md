---
title: "Download and Install Maven 3.3.9 on Windows"
permalink: /download-install-maven-3-3-9-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Apache Maven 3.3.9 on Windows."
date: 2018-07-21
last_modified_at: 2018-07-21
categories: [Development]
tags: [Download, Install, Maven, Setup, Tutorial, Windows]
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/maven/download-install-maven-3-3-9-windows.png" alt="download install maven 3-3-9 windows" class="align-right title-image">

Do you want to download and install [Apache Maven](https://maven.apache.org/){:target="_blank"} 3.3.9 on Windows?

Then Check this out:

In this tutorial I'll show where to download Maven.

How to configure it.

(And above all) **how to check if everything is working**.

So here we go.

## Step #1: Check Prerequisites

Maven requires [Java](http://www.oracle.com/technetwork/java/javase/downloads/index.html){:target="_blank"} to work. So let's check if you have Java on your system.

Click on the Windows button. Then type "<kbd>cmd</kbd>" in the search box and press `ENTER`.

Click on the `cmd` shortcut. Wait for the command prompt to open.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Type "<kbd>java -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/java-version-command.png" alt="java version command">

The above command prints the installed Java version.

<img src="{{ site.url }}/assets/images/posts/development/java-installed-version.png" alt="java installed version">

> For Maven 3 you need Java version 1.7 or higher.

## Step #2: Download

Go to the [Maven 3 archives page](https://archive.apache.org/dist/maven/maven-3/){:target="_blank"}. Click on the `3.3.9/` folder.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-download-archive.png" alt="maven 3 download archive">

Click on `binaries`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-distribution.png" alt="maven 3-3-9 distribution">

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

We need to setup an environment variable that will point to our Maven installation.

Click on the Windows button. Then type "<kbd>env</kbd>" in the search box and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-env.png" alt="windows search env">

Click on the `Edit environment variables for your account` shortcut. Wait for the environment variables window to open.

<img src="{{ site.url }}/assets/images/posts/development/windows-user-environment-variables.png" alt="windows user environment variables">

Click on `New...`.

<img src="{{ site.url }}/assets/images/posts/development/windows-user-environment-variables-new.png" alt="windows user environment variables new">

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

Click on the `cmd` shortcut. Wait for the command prompt to open.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Type "<kbd>mvn -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-version-command.png" alt="maven-version-command">

The above command prints the installed Maven version.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-version-output.png" alt="maven 3-3-9 version output">

**Congratulations, you have installed Maven 3.3.9 on Windows!**

Good luck and let me know if you liked this post.

Thanks!
