---
title: "Download and Install Python 2.7 on Windows"
permalink: /download-install-python-2-7-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Python 2.7.15 on Windows 10."
date: 2018-08-05
last_modified_at: 2018-08-05
header:
  teaser: "assets/images/posts/development/maven/download-install-python-2-7-windows.png"
categories: [Development]
tags: [Download, Install, Python, Setup, Tutorial, Windows]
published: false
---

<img src="{{ site.url }}/assets/images/posts/development/python/download-install-python-2-7-windows.png" alt="download install python 2-7 windows" class="align-right title-image">

This is a complete guide to download and install [Python](https://www.python.org){:target="_blank"} 2.7 on Windows.

So if you want to know how to setup Python, you’ll love the step-by-step approach in this tutorial.

We’ve got a number of steps to cover, so let’s get started.

## Step #1: Download

Head over to the [Python downloads page](https://www.python.org/downloads/){:target="_blank"}.

<img src="{{ site.url }}/assets/images/posts/development/python/python-download-page.png" alt="python-download-page">

Scroll down to the `Looking for a specific release?` section.

Look for the latest Python 2.7 entry in the list. At the time of writing this was Python `2.7.15`.

Click on `Download`.

<img src="{{ site.url }}/assets/images/posts/development/python/python-2-7-15-specific-release-section.png" alt="python 2-7-15 specific release section">

Check your windows bit version and click on the corresponding link.

In this guide we will install the 64-bit version. So we click on the link that contains `x86-64`: `Windows x86-64 MSI installer`.

<img src="{{ site.url }}/assets/images/posts/development/python/python-2-7-15-windows-installer.png" alt="python 2-7-15 windows installer">

Wait for the download to complete.

> Do you want to skip above steps? Here is the direct link to download the [32 bit](https://www.python.org/ftp/python/2.7.15/python-2.7.15.msi){:target="_blank"} or [64 bit](https://www.python.org/ftp/python/2.7.15/python-2.7.15.amd64.msi){:target="_blank"} Python 2.7.15 installer for Windows.

## Step #2: Install

Open the location of the downloaded installer.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-2-downloaded-binary.png" alt="maven 3-2-2 downloaded binary">

Right-click the ZIP archive file. Select `Extract All…`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-2-downloaded-binary-extract-all.png" alt="maven 3-2-2 downloaded binary extract all">

Select an extract destination for the Maven files.

In this example, we extract in `C:\Users\Downlinko\tools`.

<img src="{{ site.url }}/assets/images/posts/development/tools-extract-destination.png" alt="tools-extract-destination">

Click on `Extract`. This extracts all Maven files under `C:\Users\Downlinko\tools\apache-maven-3.2.2`.

> From now on we refer to this location as `[MAVEN_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-2-install-dir.png" alt="maven 3-2-2 install dir">

## Step #4: Setup

We need to set up an environment variable that will point to our Maven installation.

Click on the search button. Then type "<kbd>env</kbd>".

> On Windows 7 click on the Windows button.

Click on the `Edit environment variables for your account` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-env.png" alt="windows search env">

Wait for the environment variables window to open.

Click on `New…`.

<img src="{{ site.url }}/assets/images/posts/development/windows-account-environment-variables-jdk-new.png" alt="windows account environment variables jdk new">

Enter "<kbd>M2_HOME</kbd>" as variable name. Enter the `[MAVEN_INSTALL_DIR]` as variable value.

In this tutorial the installation directory is: `C:\Users\Downlinko\tools\apache-maven-3.2.2`.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-2-home-variable.png" alt="maven 3-2-2 home variable">

Next, we need to configure the PATH environment variable so we can run Maven from a command prompt.

Select the `PATH` variable. Click on `Edit…`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-2-edit-path-variable.png" alt="maven 3-2-2 edit path variable">

Click on `New` and type "<kbd>%M2_HOME%\bin</kbd>" as shown below.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-path-variable.png" alt="maven path variable">

Click `OK` once more to close the environment variables window.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-2-windows-account-environment-variables.png" alt="maven 3-2-2 windows account environment variables">

> On Windows 7 you cannot add extra values for an existing `Path` variable. You need to append "<kbd>;%M2_HOME%\bin</kbd>" at the end of the variable value instead.

## Step #5: Test

To test the setup click on the search button. Then type "<kbd>env</kbd>".

Click on the `cmd` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Type "<kbd>mvn -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-version-command.png" alt="maven-version-command">

The above command prints the installed Maven version: 3.2.2.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-2-2-version-output.png" alt="maven 3-2-2 version output">

**Congratulations, you have installed Maven 3.2.2 on Windows 10!**

Good luck and let me know if you liked this post.

Thanks!
