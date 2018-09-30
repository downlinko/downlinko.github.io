---
title: "How to Download and Install Anaconda on Windows"
permalink: /download-install-anaconda-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Anaconda on Windows 10."
date: 2018-10-01
last_modified_at: 2018-10-01
header:
  teaser: "assets/images/posts/development/python/download-install-anaconda-windows.png"
categories: [Development]
tags: [Anaconda, Download, Install, Python, Setup, Tutorial, Windows]
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/python/download-install-anaconda-windows.png" alt="download install anaconda windows" class="align-right title-image">

This guide will help you learn to **setup the Anaconda distribution for Python** on Windows.

In record time.

So without further ado, let’s get started…

## What is Anaconda?

[Anaconda](https://en.wikipedia.org/wiki/Anaconda_(Python_distribution)){:target="_blank"} is a distribution of the Python and R programming languages. It focuses on **data science and machine learning** related applications.

The distribution includes more than 250 popular data science packages.

Anaconda is free and open source and maintained by Anaconda Inc. A software development and consulting company based in Austin, Texas, USA.

## Step #1: Download

Head over to the [Anaconda for Windows download page](https://www.anaconda.com/download/#windows){:target="_blank"}.

[Verify your windows bit version]({{ site.url }}/windows-10-bit-version-check.html) and click on the corresponding link.

In this guide, we will download the 64-bit installer.

At the time of writing the latest stable Anaconda release was version `5.2.0`.

<img src="{{ site.url }}/assets/images/posts/development/python/anaconda-download-graphical-installer.png" alt="anaconda download graphical installer">

Wait for the download to complete.

## Step #2: Install

Open the location of the downloaded executable.

<img src="{{ site.url }}/assets/images/posts/development/python/anaconda-downloaded-installer.png" alt="anaconda downloaded installer">

Double-click it to run the installer.

On Windows 10 a pop-up window will appear: `The app you're trying to install isn't a verified app from the Store`

Click on `Install anyway`.

<img src="{{ site.url }}/assets/images/posts/windows-10-install-app-not-in-store.png" alt="windows 10 install app not in store">

The Anaconda installer will start.

Click `Next`.

<img src="{{ site.url }}/assets/images/posts/development/python/anaconda-installer-start.png" alt="anaconda 11 installer start">

Click on `I Agree` to accept the license agreement.

<img src="{{ site.url }}/assets/images/posts/development/python/anaconda-license-agreement.png" alt="anaconda license agreement">

Select if you want to install for the current user or all users on the system.

> Installing for all users requires Windows Administrator privileges.

In this tutorial, we keep the recommended setting of `Just Me`.

Click `Next`.

<img src="{{ site.url }}/assets/images/posts/development/python/anaconda-installation-type.png" alt="anaconda installation type">

You can change the installation location by clicking on the `Browse…` button.

> Do not install Anaconda in a directory that contains spaces or special characters.

For this example, we keep the default install location in the user's home folder.

<img src="{{ site.url }}/assets/images/posts/development/python/anaconda-install-location.png" alt="anaconda install location">

Choose if you want to add Anaconda to your PATH environment variable.

> We recommend that you do not add Anaconda to the PATH environment variable. The reason for this is that it can interfere with other software.

Choose whether you want to register Anaconda as your default Python environment.

Leave the `Register Anaconda as my default Python 3.6` box checked. Unless you plan on installing and running multiple versions of Anaconda. Or in case you need to use multiple versions of Python.

Click `Install` to start the installation.

<img src="{{ site.url }}/assets/images/posts/development/python/anaconda-advanced-options.png" alt="anaconda advanced options">

The Anaconda installation will now start.

A progress bar shows the various steps that are executed.

<img src="{{ site.url }}/assets/images/posts/development/python/anaconda-installer-progress.png" alt="anaconda installer progress">

Once the installation is complete, click `Next`.

<img src="{{ site.url }}/assets/images/posts/development/python/anaconda-installer-complete.png" alt="anaconda-installer-complete">

You can now also install the Microsoft Visual Code editor. This is an optional step. In this guide, we install Anaconda without Microsoft VSCode.

Click `Skip`.

> Check following post for a detailed guide on [how to install Visual Studio Code on Windows 10]({{ site.url }}/download-install-visual-studio-code-windows.html).

<img src="{{ site.url }}/assets/images/posts/development/python/anaconda-visual-code-installation.png" alt="anaconda visual code installation">

Click `Finish` to complete the installation.

<img src="{{ site.url }}/assets/images/posts/development/python/anaconda-installation-complete.png" alt="anaconda installation complete">

## Step #3: Run

Let's verify the installation

Click on the Windows button and look for Anaconda menu item. Open it and click on the `Anaconda Navigator` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/python/anaconda-navigator-shortcut.png" alt="anaconda navigator shortcut">

Navigator should now open as shown below.

<img src="{{ site.url }}/assets/images/posts/development/python/anaconda-navigator.png" alt="anaconda navigator">

**Congratulations, you have installed Anaconda on Windows 10!**

Now take the next step and learn how to [get started with Anaconda](https://docs.anaconda.com/anaconda/user-guide/getting-started/){:target="_blank"}.

Leave a comment below if you enjoyed this post.

Thanks!
