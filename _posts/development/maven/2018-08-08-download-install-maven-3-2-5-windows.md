---
title: "How to Download and Install Apache Maven 3.2.5 on Windows"
permalink: /download-install-apache-maven-3-2-5-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Apache Maven 3.2.5 on Windows 10."
date: 2018-08-08
last_modified_at: 2018-08-08
header:
  teaser: "assets/images/posts/development/maven/download-install-maven-3-2-5-windows.png"
categories: [Development]
tags: [Apache Maven, Download, Install, Maven, Setup, Tutorial, Windows]
redirect_from:
  - /download-install-maven-3-2-5-windows.html
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/maven/download-install-maven-3-2-5-windows.png" alt="download install maven 3-2-5 windows" class="align-right title-image">

Do you want to download and install [Apache Maven](https://maven.apache.org/){:target="_blank"} 3.2.5 on Windows?

Then check this out:

In this tutorial, I'll show where to download Maven.

How to configure it.

(And above all) **how to check if everything is working**.

So here we go.

Check following posts if you are looking to download and install [Maven 3.2.2]({{ site.url }}/download-install-apache-maven-3-2-2-windows.html), [Maven 3.3.9]({{ site.url }}/download-install-apache-maven-3-3-9-windows.html), [Maven 3.5.0]({{ site.url }}/download-install-apache-maven-3-5-0-windows.html) or the [latest Maven version]({{ site.url }}/download-install-apache-maven-windows.html).
{: .notice--primary}

## What is Apache Maven?

[Maven](https://en.wikipedia.org/wiki/Apache_Maven){:target="_blank"} is a build automation tool. It addresses two aspects of building software:
* It describes the **different steps** in the build process.
* It describes the **dependencies** to other modules and components.

The Maven project is part of the Apache Software Foundation. Which is a decentralized open source community of developers.

## Step #1: Check Prerequisites

Maven requires [Java](http://www.oracle.com/technetwork/java/javase/downloads/index.html){:target="_blank"} to work. So let's check if you have Java configured on your system.

Click on the search button. Then type "<kbd>cmd</kbd>" (without quotes).

> If you have Windows 7 click on the Windows button.

Click on the `Command Prompt` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Type "<kbd>java -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/java-version-command.png" alt="java version command">

The above command prints the installed Java version.

<img src="{{ site.url }}/assets/images/posts/development/java-installed-version.png" alt="java installed version">

> For Maven 3 you need Java version 1.7 or higher.

If you do not have Java installed on your system. Check following post which details [how to install a JDK on Windows 10]({{ site.url }}/download-install-jdk-8-windows.html).

## Step #2: Download

Go to the [Maven 3 archives page](https://archive.apache.org/dist/maven/maven-3/){:target="_blank"}.

Click on the `3.2.5/` folder.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-5-download-archive.png" alt="maven 3-2-5 download archive">

Click on `binaries`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-5-distribution.png" alt="maven 3-2-5 distribution">

Click on the `apache-maven-3.2.5-bin.zip` link.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-5-binaries.png" alt="maven 3-2-5 binaries">

Wait for the download to complete.

> Do you want to skip the above steps? Here is the direct link to download the [Maven 3.2.5 binary](https://archive.apache.org/dist/maven/maven-3/3.2.5/binaries/apache-maven-3.2.5-bin.zip){:target="_blank"} for Windows.

## Step #3: Install

Open the location of the downloaded installer.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-5-downloaded-binary.png" alt="maven 3-2-5 downloaded binary">

Right-click the ZIP archive file. Select `Extract All…`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-5-downloaded-binary-extract-all.png" alt="maven 3-2-5 downloaded binary extract all">

Select an extract destination for the Maven files.

In this example, we extract in `C:\Users\Downlinko\tools\maven`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-extract-destination.png" alt="tools-extract-destination">

Click on `Extract`. This extracts all Maven files under `C:\Users\Downlinko\tools\maven\apache-maven-3.2.5`.

> From now on we refer to this location as `[MAVEN_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-5-install-dir.png" alt="maven 3-2-5 install dir">

## Step #4: Setup

We need to set up an environment variable that will point to our Maven installation.

Click on the search button. Then type "<kbd>env</kbd>".

> If you have Windows 7 click on the Windows button.

Click on the `Edit environment variables for your account` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-env.png" alt="windows search env">

Wait for the environment variables window to open.

Click on `New…`.

<img src="{{ site.url }}/assets/images/posts/development/windows-account-environment-variables-jdk-new.png" alt="windows account environment variables jdk new">

Enter "<kbd>M2_HOME</kbd>" as variable name. Enter the `[MAVEN_INSTALL_DIR]` as variable value.

In this tutorial the installation directory is: `C:\Users\Downlinko\tools\maven\apache-maven-3.2.5`.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-5-home-variable.png" alt="maven 3-2-5 home variable">

Next, we need to configure the PATH environment variable so we can run Maven from a command prompt.

Select the `PATH` variable. Click on `Edit…`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-5-edit-path-variable.png" alt="maven 3-2-5 edit path variable">

Click on `New` and type "<kbd>%M2_HOME%\bin</kbd>" as shown below.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-path-variable.png" alt="maven path variable">

Click `OK` once more to close the environment variables window.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-5-windows-account-environment-variables.png" alt="maven 3-2-5 windows account environment variables">

> On Windows 7 you cannot add extra values for an existing `Path` variable. You need to append "<kbd>;%M2_HOME%\bin</kbd>" at the end of the variable value instead.

## Step #5: Test

To test the setup click on the search button. Then type "<kbd>cmd</kbd>".

Click on the `Command Prompt` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Type "<kbd>mvn -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-version-command.png" alt="maven version command">

The above command prints the installed Maven version.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-5-version-output.png" alt="maven 3-2-5 version output">

**Congratulations, you have installed Maven 3.2.5 on Windows 10!**

Now go ahead and [create your first Maven project](https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html){:target="_blank"}.

Good luck and let me know if you liked this post.

Thanks!
