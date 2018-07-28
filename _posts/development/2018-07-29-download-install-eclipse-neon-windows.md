---
title: "Download and Install Eclipse Neon on Windows"
permalink: /download-install-eclipse-neon-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Eclipse Neon on Windows 10."
date: 2018-07-29
last_modified_at: 2018-07-29
categories: [Development]
tags: [Download, Eclipse, Install, Eclipse Neon, Tutorial, Windows]
published: false
---

<img src="{{ site.url }}/assets/images/posts/development/eclipse/download-install-eclipse-neon-windows.png" alt="download install eclipse neon windows" class="align-right title-image">

Looking to download and install [Eclipse Neon](https://www.eclipse.org/neon/){:target="_blank"} on Windows?

Good news!

I’m going to explain you **where you can find the package**.

I'll also guide you through the different installation steps.

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

It also prints the whether you have the 32 or 64-bit version of Java.

<img src="{{ site.url }}/assets/images/posts/development/java-installed-bit-version.png" alt="java installed bit version">

> Take note of this as you will need it in the next step.

## Step #2: Download

Head over to the [Eclipse Neon Packages](https://www.eclipse.org/downloads/packages/release/Mars/2){:target="_blank"} download page.

We will download the `Eclipse IDE for Java EE Developers` package.

Click on your Windows version. This needs to match with the Java version installed on your system!

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-neon-packages-download-page.png" alt="eclipse neon packages download page">

Wait for the download to complete.

> Some download mirrors might return a `404 Not Found` error. Here is a direct link to download the [32 Bit](http://mirror.csclub.uwaterloo.ca/eclipse/technology/epp/downloads/release/neon/2/eclipse-jee-neon-2-win32.zip){:target="_blank"} or [64 Bit](http://mirror.csclub.uwaterloo.ca/eclipse/technology/epp/downloads/release/neon/2/eclipse-jee-neon-2-win32-x86_64.zip){:target="_blank"} package for Windows.

## Step #3: Install

Open the location of the downloaded package.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-neon-package-downloaded.png" alt="eclipse neon package downloaded">

Right-click the ZIP archive file. Select `Extract All...`.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-neon-package-extract-all.png" alt="eclipse neon package extract all">

Select an extract destination for the Eclipse Neon files.

In this example, we extract in `C:\Users\Downlinko\tools`.

<img src="{{ site.url }}/assets/images/posts/development/tools-extract-destination.png" alt="tools-extract-destination">

Click on `Extract`. This extracts all Eclipse Neon files under `C:\Users\Downlinko\tools\eclipse`.

> From now on we refer to this location as `[ECLIPSE_NEON_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-neon-install-dir.png" alt="eclipse neon install dir">

## Step #4: Run

To run Eclipse Neon navigate to the `[ECLIPSE_NEON_INSTALL_DIR]` installation directory.

Located the executable file called `eclipse` and double-click on it.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-neon-executable.png" alt="eclipse neon executable">

Eclipse will start and prompt for a default workspace location.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-neon-workspace-default-location.png" alt="eclipse neon workspace default location">

If needed change the default location and click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-neon-workspace.png" alt="eclipse neon workspace">

**Congratulations, you have installed Eclipse Neon on Windows 10!**

Submit a comment below if you found this post helpful.

Thanks!
