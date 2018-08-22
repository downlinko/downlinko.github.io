---
title: "Download and Install Eclipse Mars on Windows"
permalink: /download-install-eclipse-mars-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Eclipse Mars on Windows 10."
date: 2018-07-21
last_modified_at: 2018-07-21
header:
  teaser: "assets/images/posts/development/eclipse/download-install-eclipse-mars-windows.png"
categories: [Development]
tags: [Download, Eclipse, Eclipse Mars, Install, Tutorial, Windows]
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/eclipse/download-install-eclipse-mars-windows.png" alt="download install eclipse mars windows" class="align-right title-image">

Looking to download and install [Eclipse Mars](https://www.eclipse.org/mars/){:target="_blank"} on Windows?

Good news!

I’m going to explain you **where you can find the package**.

I'll also guide you through the different installation steps.

Let’s go!

Check following post if you are looking to download and install [Eclipse Neon]({{ site.url }}/download-install-eclipse-neon-windows.html) or [Eclipse Photon]({{ site.url }}/download-install-eclipse-photon-windows.html).
{: .notice--primary}

## Step #1: Prerequisites

Eclipse requires [Java](http://www.oracle.com/technetwork/java/javase/downloads/index.html){:target="_blank"} to run. Let's check if you have Java installed on your system.

Click on the Windows button. Then type "<kbd>cmd</kbd>" in the search box.

Click on the `cmd` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Type "<kbd>java -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/java-version-command.png" alt="java version command">

The above command prints the installed Java version.

<img src="{{ site.url }}/assets/images/posts/development/java-installed-version.png" alt="java installed version">

It also prints the whether you have the 32 or 64-bit version of Java.

<img src="{{ site.url }}/assets/images/posts/development/java-installed-bit-version.png" alt="java installed bit version">

> Take note of this as you will need it in the next step.

If you do not have Java installed on your system. Check following post which details [how to install a Java Development Kit on Windows 10]({{ site.url }}/download-install-jdk-8-windows.html).

## Step #2: Download

Head over to the [Eclipse Mars 2 Packages](https://www.eclipse.org/downloads/packages/release/mars/2){:target="_blank"} download page.

We will download the `Eclipse IDE for Java EE Developers` package.

Click on your Windows version. This needs to match with the Java version installed on your system!

In this guide we will install the 64-bit version.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-mars-packages-download-page.png" alt="eclipse mars packages download page">

Wait for the download to complete.

> Do you want to skip the above steps? Here is a direct link to download the [32 Bit](http://mirror.csclub.uwaterloo.ca/eclipse/technology/epp/downloads/release/mars/2/eclipse-jee-mars-2-win32.zip){:target="_blank"} or [64 Bit](http://mirror.csclub.uwaterloo.ca/eclipse/technology/epp/downloads/release/mars/2/eclipse-jee-mars-2-win32-x86_64.zip){:target="_blank"} package for Windows.

## Step #3: Install

Open the location of the downloaded package.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-mars-downloaded-package.png" alt="eclipse mars downloaded package">

Right-click the ZIP archive file. Select `Extract All…`.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-mars-downloaded-package-extract-all.png" alt="eclipse mars downloaded package extract all">

Select an extract destination for the Eclipse Mars files.

In this example, we extract in `C:\Users\Downlinko\tools\eclipse\mars`.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-mars-extract-destination.png" alt="eclipse mars extract destination">

Click on `Extract`. This extracts all Eclipse Mars files under `C:\Users\Downlinko\tools\eclipse\mars`.

> From now on we refer to this location as `[ECLIPSE_MARS_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-mars-install-dir.png" alt="eclipse mars install dir">

## Step #4: Run

To run Eclipse Mars navigate to the `[ECLIPSE_MARS_INSTALL_DIR]` installation directory.

Located the `Application` file called `eclipse` and double-click on it.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-mars-executable.png" alt="eclipse mars executable">

On Windows 10 a pop-up window will appear: `The app you're trying to install isn't a verified app from the Store`

Click on `Install anyway`.

<img src="{{ site.url }}/assets/images/posts/windows-10-install-app-not-in-store.png" alt="windows 10 install app not in store">

Eclipse will start and prompt for a default workspace location.

If needed change the default location and click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-workspace-default-location.png" alt="eclipse workspace default location">

Wait for Eclipse Mars to open.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-mars-workspace.png" alt="eclipse mars workspace">

To verify the installed version click on `Help` and then on `About Eclipse` as shown below.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-mars-help-about-eclipse.png" alt="eclipse mars help about eclipse">

This shows the Eclipse version: `Mars.2 Release (4.5.2)`.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-mars-version.png" alt="eclipse mars version">

**Congratulations, you have installed Eclipse Mars on Windows 10!**

Submit a comment below if you found this post helpful.

Thanks!
