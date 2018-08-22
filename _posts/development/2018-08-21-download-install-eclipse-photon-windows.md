---
title: "Download and Install Eclipse Photon on Windows"
permalink: /download-install-eclipse-photon-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Eclipse Photon on Windows 10."
date: 2018-08-21
last_modified_at: 2018-08-21
header:
  teaser: "assets/images/posts/development/eclipse/download-install-eclipse-photon-windows.png"
categories: [Development]
tags: [Download, Eclipse, Eclipse Photon, Install, Tutorial, Windows]
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/eclipse/download-install-eclipse-photon-windows.png" alt="download install eclipse photon windows" class="align-right title-image">

Looking to download and install [Eclipse Photon](https://www.eclipse.org/photon/){:target="_blank"} on Windows?

Good news!

I’m going to explain you **where you can find the package**.

I'll also guide you through the different installation steps.

Let’s go!

Check following post if you are looking to download and install [Eclipse Mars]({{ site.url }}/download-install-eclipse-mars-windows.html) or [Eclipse Neon]({{ site.url }}/download-install-eclipse-neon-windows.html).
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

Head over to the [Eclipse Photon Packages](https://www.eclipse.org/downloads/packages/){:target="_blank"} download page.

We will download the `Eclipse IDE for Java EE Developers` package.

Click on your Windows version. This needs to match with the Java version installed on your system!

In this guide we will install the 64-bit version.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-photon-packages-download-page.png" alt="eclipse photon packages download page">

Wait for the download to complete.

> Do you want to skip the above steps? Here is a direct link to download the [32 Bit](http://mirror.csclub.uwaterloo.ca/eclipse/technology/epp/downloads/release/photon/R/eclipse-java-photon-R-win32.zip){:target="_blank"} or [64 Bit](http://mirror.csclub.uwaterloo.ca/eclipse/technology/epp/downloads/release/photon/R/eclipse-java-photon-R-win32-x86_64.zip){:target="_blank"} package for Windows.

## Step #3: Install

Open the location of the downloaded package.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-photon-downloaded-package.png" alt="eclipse photon downloaded package">

Right-click the ZIP archive file. Select `Extract All...`.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-photon-downloaded-package-extract-all.png" alt="eclipse photon downloaded package extract all">

Select an extract destination for the Eclipse Photon files.

In this example, we extract in `C:\Users\Downlinko\tools\eclipse\photon`.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-photon-extract-destination.png" alt="eclipse photon extract destination">

Click on `Extract`. This extracts all Eclipse Photon files under `C:\Users\Downlinko\tools\eclipse\photon`.

> From now on we refer to this location as `[ECLIPSE_PHOTON_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-photon-install-dir.png" alt="eclipse photon install dir">

## Step #4: Run

To run Eclipse Photon navigate to the `[ECLIPSE_PHOTON_INSTALL_DIR]` installation directory.

Located the `Application` file called `eclipse` and double-click on it.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-photon-executable.png" alt="eclipse photon executable">

On Windows 10 a pop-up window will appear: `The app you're trying to install isn't a verified app from the Store`

Click on `Install anyway`.

<img src="{{ site.url }}/assets/images/posts/windows-10-install-app-not-in-store.png" alt="windows 10 install app not in store">

Eclipse will start and prompt for a default workspace location.

If needed change the default location and click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-workspace-default-location.png" alt="eclipse workspace default location">

Wait for Eclipse Photon to open.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-photon-workspace.png" alt="eclipse photon workspace">

To verify the installed version click on `Help` and then on `About Eclipse IDE` as shown below.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-photon-help-about-eclipse.png" alt="eclipse photon help about eclipse">

This shows the Eclipse version: `Photon Release (4.8.0)`.

<img src="{{ site.url }}/assets/images/posts/development/eclipse/eclipse-photon-version.png" alt="eclipse photon version">

**Congratulations, you have installed Eclipse Photon on Windows 10!**

Submit a comment below if you found this post helpful.

Thanks!
