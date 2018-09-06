---
title: "Download and Install Golang on Windows"
permalink: /download-install-golang-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Golang on Windows 10."
date: 2018-09-01
last_modified_at: 2018-09-01
header:
  teaser: "assets/images/posts/development/golang/download-install-golang-windows.png"
categories: [Development]
tags: [Download, Go, Golang, Install, Setup, Tutorial, Windows]
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/golang/download-install-golang-windows.png" alt="download install golang windows" class="align-right title-image">

So you want to download and install the [Go programming language](https://golang.org/){:target="_blank"} on Windows?

Then look no further!

In this guide, you’ll learn how to download the compiler…

…and how to install it so you can use it from command line.

So let's fire away:

## What is Golang?

[Go](https://en.wikipedia.org/wiki/Go_(programming_language)){:target="_blank"} (often referred to as Golang) is an open source programming language. It comes with **built-in concurrency** and is strong and static typed. Go is an imperative language that supports object-oriented programming (OOP).

Golang is maintained and developed by a team at [Google](https://www.google.com/){:target="_blank"} and many contributors from the open source community.

## Step #1: Download

Head over to the [Golang downloads page](https://golang.org/dl/){:target="_blank"}. Here you will find all the available binary releases.

[Verify your windows bit version]({{ site.url }}/windows-10-bit-version-check.html) and click on the corresponding link under the `Stable versions` section:

* For 32-bit = <kbd>goX.XX.windows-386.msi</kbd>
* For 64-bit = <kbd>goX.XX.windows-amd64.msi</kbd>

In this tutorial, we will download the `64-bit` version.

At the time of writing the latest stable Golang release was version: `1.11`.

<img src="{{ site.url }}/assets/images/posts/development/golang/golang-latest-binary-release-page.png" alt="golang latest binary release-page">

Wait for the download to complete.

## Step #2: Install

Open the location of the downloaded executable.

<img src="{{ site.url }}/assets/images/posts/development/golang/golang-downloaded-installer.png" alt="golang downloaded installer">

Double-click it to run the installer.

On Windows 10 a pop-up window will appear: `The app you're trying to install isn't a verified app from the Store`

Click on `Install anyway`.

<img src="{{ site.url }}/assets/images/posts/windows-10-install-app-not-in-store.png" alt="windows 10 install app not in store">

The Golang installer wizard will start. Click `Next`.

<img src="{{ site.url }}/assets/images/posts/development/golang/golang-installer-start.png" alt="golang installer start">

Make sure the `I accept the terms in License Agreement` checkbox is selected. Click `Next`.

<img src="{{ site.url }}/assets/images/posts/development/golang/golang-installer-license-agreement.png" alt="golang installer license agreement">

You can change the installation location by clicking on the `Change…` button.

In this example, we keep the default install location of `C:\Go\`.

<img src="{{ site.url }}/assets/images/posts/development/golang/golang-installer-default-location.png" alt="golang installer default location">

Click `Install` to start the installation.

<img src="{{ site.url }}/assets/images/posts/development/golang/golang-installer-ready.png" alt="golang installer ready">

The Golang installation will now start.

A progress bar shows the various steps that are executed.

<img src="{{ site.url }}/assets/images/posts/development/golang/golang-installer-progress.png" alt="golang installer progress">

Once the installation is complete, click `Finish`.

<img src="{{ site.url }}/assets/images/posts/development/golang/golang-installer-complete.png" alt="golang installer complete">

## Step #3: Test

Let's test the setup.

Click on the search button. Then type "<kbd>cmd</kbd>" (without quotes).

Click on the `Command Prompt` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Type "<kbd>go version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/golang/golang-version-command.png" alt="golang-version-command">

The above command prints the installed Golang version: `go version go1.11`.

<img src="{{ site.url }}/assets/images/posts/development/golang/golang-version-output.png" alt="golang version output">

**Congratulations, you have installed Golang on Windows 10!**

> If you want to know your `GOPATH` directory, type "<kbd>echo %GOPATH%</kbd>" in a command prompt and press `ENTER`.

Now go ahead and [learn some Golang basics](https://golang.org/doc/install#testing){:target="_blank"}.

Have fun coding!

If you liked this guide leave a short message below.

Thanks.
