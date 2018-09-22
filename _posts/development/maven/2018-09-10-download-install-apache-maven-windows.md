---
title: "How to Download and Install Apache Maven on Windows"
permalink: /download-install-apache-maven-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install the latest version of Apache Maven on Windows 10."
date: 2018-09-10
last_modified_at: 2018-09-10
header:
  teaser: "assets/images/posts/development/maven/download-install-apache-maven-windows.png"
categories: [Development]
tags: [Apache Maven, Download, Install, Maven, Setup, Tutorial, Windows]
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/maven/download-install-apache-maven-windows.png" alt="download install apache maven windows" class="align-right title-image">

Do you want to download and install the latest version of [Apache Maven](https://maven.apache.org/){:target="_blank"} on Windows?

Then check this out:

In this tutorial, I'll show where to download Maven.

How to configure it.

(And above all) **how to check if everything is working**.

So here we go.

Check following posts if you are looking to download and install [Maven 3.2.2]({{ site.url }}/download-install-apache-maven-3-2-2-windows.html), [Maven 3.2.5]({{ site.url }}/download-install-apache-maven-3-2-5-windows.html), [Maven 3.3.9]({{ site.url }}/download-install-apache-maven-3-3-9-windows.html) or [Maven 3.5.0]({{ site.url }}/download-install-apache-maven-3-5-0-windows.html).
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

Go to the [Maven download page](https://maven.apache.org/download.cgi){:target="_blank"}.

<img src="{{ site.url }}/assets/images/posts/development/maven/apache-maven-download-page.png" alt="apache maven download page">

Scroll down to the `Files` section.

Click on the `Binary zip archive` link.

<img src="{{ site.url }}/assets/images/posts/development/maven/apache-maven-download-binary-zip-archive.png" alt="apache maven download binary zip archive">

Wait for the download to complete.

> Do you want to skip the above steps? Here is the direct link to download the [Maven 3.5.4 binary](http://www-us.apache.org/dist/maven/maven-3/3.5.4/binaries/apache-maven-3.5.4-bin.zip){:target="_blank"} for Windows.

## Step #3: Install

Open the location of the downloaded installer.

<img src="{{ site.url }}/assets/images/posts/development/maven/apache-mavendownloaded-binary.png" alt="apache maven downloaded binary">

Right-click the ZIP archive file. Select `Extract All…`.

<img src="{{ site.url }}/assets/images/posts/development/maven/apache-maven-downloaded-binary-extract-all.png" alt="apache maven downloaded binary extract all">

Select an extract destination for the Maven files.

In this example, we extract in `C:\Users\Downlinko\tools\maven`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-extract-destination.png" alt="maven extract destination">

Click on `Extract`. This extracts all Maven files under `C:\Users\Downlinko\tools\maven\apache-maven-3.5.4`.

> From now on we refer to this location as `[MAVEN_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/maven/apache-maven-install-dir.png" alt="apache maven install dir">

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

In this tutorial the installation directory is: `C:\Users\Downlinko\tools\maven\apache-maven-3.5.4`.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/maven/apache-maven-home-variable.png" alt="apache maven home variable">

Next, we need to configure the PATH environment variable so we can run Maven from a command prompt.

Select the `PATH` variable. Click on `Edit…`.

<img src="{{ site.url }}/assets/images/posts/development/maven/apache-maven-edit-path-variable.png" alt="apache maven edit path variable">

Click on `New` and type "<kbd>%M2_HOME%\bin</kbd>" as shown below.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-path-variable.png" alt="maven path variable">

Click `OK` once more to close the environment variables window.

<img src="{{ site.url }}/assets/images/posts/development/maven/apache-maven-windows-account-environment-variables.png" alt="apache maven windows account environment variables">

> On Windows 7 you cannot add extra values for an existing `Path` variable. You need to append "<kbd>;%M2_HOME%\bin</kbd>" at the end of the variable value instead.

## Step #5: Test

To test the setup click on the search button. Then type "<kbd>cmd</kbd>".

Click on the `Command Prompt` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Type "<kbd>mvn -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-version-command.png" alt="maven version command">

The above command prints the installed Maven version: 3.5.4.

<img src="{{ site.url }}/assets/images/posts/development/maven/apache-maven-version-output.png" alt="maven 3-5-0 version output">

**Congratulations, you have installed Apache Maven on Windows 10!**

Now it's time [to create your first Maven project](https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html){:target="_blank"}.

Go ahead and leave a comment if you liked this post.

Thanks!
