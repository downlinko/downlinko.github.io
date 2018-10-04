---
title: "How to Download and Install Apache JMeter on Windows"
permalink: /download-install-apache-jmeter-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Apache JMeter on Windows 10."
date: 2018-10-04
last_modified_at: 2018-10-04
header:
  teaser: "assets/images/posts/development/testing/download-install-apache-jmeter-windows.png"
categories: [Development]
tags: [Apache JMeter, Download, Install, JMeter, Setup, Tutorial, Windows]
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/testing/download-install-apache-jmeter-windows.png" alt="download install apache jmeter windows" class="align-right title-image">

Today you’re going to see how to download and install [Apache JMeter](http://jmeter.apache.org/){:target="_blank"} on Windows.

In four easy steps.

Let’s get this show on the road.

## What is Apache JMeter?

[Apache JMeter](https://en.wikipedia.org/wiki/Apache_JMeter){:target="_blank"} is a load testing tool. It focuses on analyzing and measuring the performance of a variety of services.

JMeter was originally designed for testing Web Applications. Today it has the ability to **test many different protocols**: HTTP, FTP, JDBC, LDAP, JMS, SMTP, POP3, IMAP, TCP, and others.

The JMeter project is part of the Apache Software Foundation. A decentralized open source community of developers.

## Step #1: Check Prerequisites

Apache JMeter requires [Java](http://www.oracle.com/technetwork/java/javase/downloads/index.html){:target="_blank"} to work. So let's check if you have Java configured on your system.

Click on the search button. Then type "<kbd>cmd</kbd>" (without quotes).

> If you have Windows 7 click on the Windows button.

Click on the `Command Prompt` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Type "<kbd>java -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/java-version-command.png" alt="java version command">

The above command prints the installed Java version.

<img src="{{ site.url }}/assets/images/posts/development/java-installed-version.png" alt="java installed version">

> For JMeter 3.2 and onward you need Java version 1.8 or higher.

If you do not have Java installed on your system. Check following post which details [how to install JDK 8 on Windows 10]({{ site.url }}/download-install-jdk-8-windows.html).

## Step #2: Download

Head over to the [JMeter download page](http://jmeter.apache.org/download_jmeter.cgi){:target="_blank"}.

Scroll down and locate the `Binaries` section.

Click on the `apache-jmeter-X.X.zip` link.

At the time of writing the latest JMeter release was version: `5.0`.

<img src="{{ site.url }}/assets/images/posts/development/testing/apache-jmeter-download-page.png" alt="apache jmeter download page">

Wait for the download to complete.

## Step #3: Install

Open the location of the downloaded binary distribution.

<img src="{{ site.url }}/assets/images/posts/development/testing/apache-jmeter-downloaded-binary.png" alt="apache jmeter downloaded binary">

Select the ZIP archive file. Right-click and then click on the `Extract All…` menu item.

<img src="{{ site.url }}/assets/images/posts/development/testing/apache-jmeter-downloaded-binary-extract-all.png" alt="apache jmeter downloaded binary extract all">

Select an extract destination for the JMeter files.

In this example, we extract in `C:\Users\Downlinko\tools`.

Click on `Extract`.

<img src="{{ site.url }}/assets/images/posts/development/tools-extract-destination.png" alt="tools extract destination">

This extracts all JMeter files under `C:\Users\Downlinko\tools\apache-jmeter-5.0`.

> From now on we refer to this location as `[JMETER_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/testing/apache-jmeter-install-dir.png" alt="apache jmeter install dir">

## Step #4: Run

You can run JMeter in 3 modes: GUI Mode, Server Mode, and Command Line Mode. Let's show how to start the graphical user interface.

> Note that you should only use the GUI mode for creating the test scripts. Use the NON-GUI mode for load testing.

Navigate to the `[JMETER_INSTALL_DIR]` installation directory.

Open the `bin` folder.

Double click on the `jmeter` Windows batch file.

<img src="{{ site.url }}/assets/images/posts/development/testing/apache-jmeter-windows-batch-file.png" alt="apache jmeter windows batch file">

If active, Windows Defender will prevent JMeter from starting. Click on the `More info` link.

<img src="{{ site.url }}/assets/images/posts/development/windows-defender-smartscreen-prevent-unrecognized-app.png" alt="windows defender smartscreen prevent unrecognized app">

A new `Run anyway` button will appear. Click on it.

<img src="{{ site.url }}/assets/images/posts/development/windows-defender-smartscreen-run-unrecognized-app.png" alt="windows defender smartscreen run unrecognized app">

After a short time, the JMeter GUI appears.

<img src="{{ site.url }}/assets/images/posts/development/testing/apache-jmeter-gui.png" alt="apache jmeter gui">

**Congratulations, you have installed Apache JMeter on Windows 10!**

Take the next step and learn [how to create a basic test plan](https://jmeter.apache.org/usermanual/build-web-test-plan.html){:target="_blank"}.

Submit a comment below if you enjoyed reading this post.

Thanks!
