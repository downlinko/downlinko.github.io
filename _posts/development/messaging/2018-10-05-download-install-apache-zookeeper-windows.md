---
title: "How to Download and Install Apache ZooKeeper on Windows"
permalink: /download-install-apache-zookeeper-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Apache ZooKeeper on Windows 10."
date: 2018-10-05
last_modified_at: 2018-10-05
header:
  teaser: "assets/images/posts/development/messaging/download-install-apache-zookeeper-windows.png"
categories: [Development]
tags: [Apache ZooKeeper, Download, Install, Setup, Tutorial, Windows, Zookeeper]
published: false
---

<img src="{{ site.url }}/assets/images/posts/development/messaging/download-install-apache-zookeeper-windows.png" alt="download install apache zookeeper windows" class="align-right title-image">

Do you want to learn how to download and install [Apache ZooKeeper](https://zookeeper.apache.org/){:target="_blank"} on Windows?

You’ve reached the right place.

Because in this tutorial **I'll walk you through the different setup steps**.

Let’s dive in!

## What is Apache ZooKeeper?

[Apache ZooKeeper](https://en.wikipedia.org/wiki/Apache_ZooKeeper){:target="_blank"} provides centralized services for building distributed systems. ZooKeeper itself is also a [distributed application](https://en.wikipedia.org/wiki/Distributed_computing){:target="_blank"}.

When you build a distributed system there are some common problems that you need to solve. ZooKeeper offers reusable building blocks that can solve these problems. For example: a configuration service, a synchronization service, and a naming registry.

ZooKeeper was originally developed at Yahoo. Now it is part of the Apache Software Foundation. A decentralized open source community of developers.

## Step #1: Check Prerequisites

ZooKeeper requires [Java](http://www.oracle.com/technetwork/java/javase/downloads/index.html){:target="_blank"} to work. So let's check if you have Java configured on your system.

Click on the search button. Then type "<kbd>cmd</kbd>" (without quotes).

> On Windows 7 click on the Windows button.

Click on the `Command Prompt` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Type "<kbd>java -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/java-version-command.png" alt="java version command">

The above command prints the installed Java version.

<img src="{{ site.url }}/assets/images/posts/development/java-installed-version.png" alt="java installed version">

> For ZooKeeper you need Java version 1.6 or higher.

If you do not have Java installed on your system. Check following post which details [how to install a JDK on Windows 10]({{ site.url }}/download-install-jdk-8-windows.html).

## Step #2: Download

Go to the [ZooKeeper releases page](https://zookeeper.apache.org/releases.html){:target="_blank"}.

Click on the `Download` link under the `Download` section.

<img src="{{ site.url }}/assets/images/posts/development/messaging/apache-zookeeper-releases-page.png" alt="apache zookeeper releases page">

Click on the suggested mirror site.

<img src="{{ site.url }}/assets/images/posts/development/messaging/apache-zookeeper-suggested-mirror.png" alt="apache zookeeper suggested mirror">

Click on the `stable` link.

<img src="{{ site.url }}/assets/images/posts/development/messaging/apache-zookeeper-stable-section.png" alt="apache zookeeper stable section">

Click on the `zookeeper-X.X.X.tar.gz` link.

At the time of writing the latest stable ZooKeeper release was version `3.4.12`.

<img src="{{ site.url }}/assets/images/posts/development/messaging/apache-zookeeper-stable-release.png" alt="apache zookeeper stable release">

Wait for the download to complete.

## Step #3: Install

Open the location of the downloaded binary.

The file is compressed using the GNU zip (gzip) compression algorithm. To unpack this format we will use 7-Zip. Check following tutorial if you need to [download and install 7-zip on Windows]({{ site.url }}/download-install-7-zip-windows.html).

<img src="{{ site.url }}/assets/images/posts/development/messaging/apache-zookeeper-downloaded-binary.png" alt="apache-zookeeper downloaded binary">

Select the GZ archive file. Right-click and then click on the `Extract Here` menu item.

<img src="{{ site.url }}/assets/images/posts/development/messaging/apache-zookeeper-extract-tar.png" alt="apache zookeeper extract tar">

This extracts the `zookeeper-X.X.X.tar` file.

<img src="{{ site.url }}/assets/images/posts/development/messaging/apache-zookeeper-tar-binary.png" alt="apache zookeeper tar binary">

Select the TAR archive file. Right-click and then click on the `Extract Here` menu item.

Select an extract destination for the zookeeper files.

In this example, we extract in `C:\Users\Downlinko\tools\zookeeper`.

<img src="{{ site.url }}/assets/images/posts/development/zookeeper/zookeeper-extract-destination.png" alt="zookeeper tools extract destination">

Click on `Extract`. This extracts all zookeeper files under `C:\Users\Downlinko\tools\zookeeper\zookeeper\TODO`.

> From now on we refer to this location as `[zookeeper_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/zookeeper/zookeeper-install-dir.png" alt="zookeeper install dir">

## Step #4: Setup

We need to set up an environment variable that will point to our ZooKeeper installation.

Click on the search button. Then type "<kbd>env</kbd>".

> On Windows 7 click on the Windows button.

Click on the `Edit environment variables for your account` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-env.png" alt="windows search env">

Wait for the environment variables window to open.

Click on `New…`.

<img src="{{ site.url }}/assets/images/posts/development/windows-account-environment-variables-jdk-new.png" alt="windows account environment variables jdk new">

Enter "<kbd>zookeeper_HOME</kbd>" as variable name. Enter the `[zookeeper_INSTALL_DIR]` as variable value.

In this tutorial the installation directory is: `C:\Users\Downlinko\tools\zookeeper\zookeeper-4.1`.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/zookeeper/zookeeper-4-1-home-variable.png" alt="zookeeper 4-1 home variable">

Next, we need to configure the PATH environment variable so we can run Maven from a command prompt.

Select the `PATH` variable. Click on `Edit…`.

<img src="{{ site.url }}/assets/images/posts/development/zookeeper/zookeeper-4-1-edit-path-variable.png" alt="zookeeper 4-1 edit path variable">

Click on `New` and type "<kbd>%zookeeper_HOME%\bin</kbd>" as shown below.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/zookeeper/zookeeper-path-variable.png" alt="zookeeper path variable">

Click `OK` once more to close the environment variables window.

<img src="{{ site.url }}/assets/images/posts/development/zookeeper/zookeeper-4-1-windows-account-environment-variables.png" alt="zookeeper 4-1 windows account environment variables">

> On Windows 7 you cannot add extra values for an existing `Path` variable. You need to append "<kbd>;%zookeeper_HOME%\bin</kbd>" at the end of the variable value instead.

## Step #5: Test

To test the setup click on the search button. Then type "<kbd>cmd</kbd>".

Click on the `Command Prompt` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Type "<kbd>zookeeper -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/zookeeper/zookeeper-version-command.png" alt="zookeeper-version-command">

The above command prints the installed zookeeper version.

<img src="{{ site.url }}/assets/images/posts/development/zookeeper/zookeeper-4-1-version-output.png" alt="zookeeper 4-1 version output">

**Congratulations, you have installed Apache Zookeeper on Windows 10!**

Write a comment below if you enjoyed this post.

Thanks!
