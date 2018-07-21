---
title: "Download and Install Eclipse Mars on Windows"
permalink: /download-install-eclipse-mars-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Eclipse Mars on Windows."
date: 2018-07-21
last_modified_at: 2018-07-21
categories: [Development]
tags: [Download, Eclipse, Install, Mars, Tutorial, Windows]
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/eclipse/download-install-eclipse-mars-windows.png" alt="download install eclipse mars windows" class="align-right title-image">

Looking to download and install Eclipse Mars?

Good news!

I’m going to explain you **where you can find the package**. I'll also guide you through the different installation steps.

Let’s go!

## Step #1: Prerequisites

Eclipse requires [Java](http://www.oracle.com/technetwork/java/javase/downloads/index.html){:target="_blank"} to work. Let's check if you have Java installed on your system.

Click on the Windows button. Then type "<kbd>cmd</kbd>" in the search box and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Click on the `cmd` shortcut. Wait for the command prompt to open.

Type "<kbd>java -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/java-version-command.png" alt="java version command">

The above command prints the installed Java version.

<img src="{{ site.url }}/assets/images/posts/development/java-installed-version.png" alt="java installed version">

It also prints the whether you have the 32 or 64 bit version of Java.

<img src="{{ site.url }}/assets/images/posts/development/java-installed-bit-version.png" alt="java installed bit version">

> Take note of this as you will need it in the next step.

## Step #2: Download

Head over to the [Eclipse Mars 2 Packages](https://www.eclipse.org/downloads/packages/release/Mars/2){:target="_blank"} download page.

We will download the `Eclipse IDE for Java EE Developers` package.

Click on your Windows version. This needs to match with the Java version installed on your system!

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-mars-packages-download-page.png" alt="eclipse mars packages download page">

Now wait for the download to complete.

> Some download mirrors might return a `404 Not Found` error. Here is a direct link to download the [32 Bit package](http://mirror.csclub.uwaterloo.ca/eclipse/technology/epp/downloads/release/mars/2/eclipse-jee-mars-2-win32.zip){:target="_blank"} or [64 Bit package](http://mirror.csclub.uwaterloo.ca/eclipse/technology/epp/downloads/release/mars/2/eclipse-jee-mars-2-win64.zip){:target="_blank"} Eclipse IDE for Java EE Developers package for Windows.

## Step #3: Install

Open the location of the downloaded package.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-mars-package-downloaded.png" alt="eclipse mars package downloaded">

Right-click the ZIP archive file. Select `Extract All...`.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-mars-package-extract-all.png" alt="eclipse mars package extract all">

Select an extract destination for the Eclipse Mars files.

In this example, we extract in `C:\Users\Downlinko\tools`.

<img src="{{ site.url }}/assets/images/posts/development/tools-extract-destination.png" alt="tools-extract-destination">

Click on `Extract`. This extracts all Eclipse Mars files under `C:\Users\Downlinko\tools\eclipse`.

> From now on we refer to this location as `[ECLIPSE_MARS_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-mars-install-dir.png" alt="eclipse mars install dir">

## Step #4: Run

To run Eclipse Mars navigate to the `[ECLIPSE_MARS_INSTALL_DIR]` installation directory.

Located the executable file called `eclipse` and double click it.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-mars-executable.png" alt="eclipse mars executable">

Eclipse will start and prompt for a default workspace location. If needed change the default location and click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-mars-workspace.png" alt="eclipse mars workspace">

**Congratulations, you have installed Eclipse Mars on Windows!**

Submit a comment below if you found this post helpful.

Thanks!
