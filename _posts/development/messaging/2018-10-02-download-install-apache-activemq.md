---
title: "How to Download and Install Apache ActiveMQ on Windows"
permalink: /download-install-apache-activemq-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install Apache ActiveMQ on Windows 10."
date: 2018-10-02
last_modified_at: 2018-10-02
header:
  teaser: "assets/images/posts/development/messaging/download-install-apache-activemq-windows.png"
categories: [Development]
tags: [ActiveMQ, Apache ActiveMQ, Download, Install, Setup, Tutorial, Windows]
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/messaging/download-install-apache-activemq-windows.png" alt="download install apache activemq windows" class="align-right title-image">

Do you want to download and install [Apache ActiveMQ](http://activemq.apache.org/){:target="_blank"} on Windows?

Then check this out:

In this tutorial, I'll show where to download ActiveMQ.

How to start and stop a broker. And how to access the admin console.

So let’s begin.

## What is Apache ActiveMQ?

[Apache ActiveMQ](https://en.wikipedia.org/wiki/Apache_ActiveMQ){:target="_blank"} is an open source message broker written in Java. It offers JMS, REST and WebSocket interfaces.

Other protocols like AMQP, MQTT, OpenWire, and STOMP are also supported. You can use these to connect applications written in different programming languages.

The ActiveMQ project is part of the Apache Software Foundation. Which is a decentralized open source community of developers.

## Step #1: Check Prerequisites

Apache ActiveMQ requires [Java](http://www.oracle.com/technetwork/java/javase/downloads/index.html){:target="_blank"} to work. So let's check if you have Java configured on your system.

Click on the search button. Then type "<kbd>cmd</kbd>" (without quotes).

> If you have Windows 7 click on the Windows button.

Click on the `Command Prompt` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Type "<kbd>java -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/java-version-command.png" alt="java version command">

The above command prints the installed Java version.

<img src="{{ site.url }}/assets/images/posts/development/java-installed-version.png" alt="java installed version">

> For ActiveMQ 5.11 and onward you need Java version 1.7 or higher.

If you do not have Java installed on your system. Check following post which details [how to install a JDK on Windows 10]({{ site.url }}/download-install-jdk-8-windows.html).

## Step #2: Download

Head over to the [ActiveMQ download page](http://activemq.apache.org/download.html){:target="_blank"}.

Click on the link under the `Latest Releases` section.

<img src="{{ site.url }}/assets/images/posts/development/messaging/apache-activemq-download-page.png" alt="java download page">

Locate the `Getting the Binary Distributions` section.

Click on the link for the Windows distribution.

<img src="{{ site.url }}/assets/images/posts/development/messaging/apache-activemq-windwos-distribution.png" alt="apache activemq windwos distribution">

Wait for the download to complete.

## Step #3: Install

Open the location of the downloaded installer.

<img src="{{ site.url }}/assets/images/posts/development/messaging/apache-activemq-downloaded-binary.png" alt="apache activemq downloaded binary">

Right-click the ZIP archive file. Select `Extract All…`.

<img src="{{ site.url }}/assets/images/posts/development/messaging/apache-activemq-downloaded-binary-extract-all.png" alt="apache activemq downloaded binary extract all">

Select an extract destination for the ActiveMQ files.

In this example, we extract in `C:\Users\Downlinko\tools`.

<img src="{{ site.url }}/assets/images/posts/development/tools-extract-destination.png" alt="tools extract destination">

Click on `Extract`. This extracts all Maven files under `C:\Users\Downlinko\tools\apache-activemq-5.15.6`.

> From now on we refer to this location as `[ACTIVEMQ_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/messaging/apache-activemq-install-dir.png" alt="apache activemq install dir">

## Step #5: Start

In order to start ActiveMQ we need to open a command promt.

Click on the search button. Then type "<kbd>cmd</kbd>".

Click on the `Command Prompt` shortcut.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Wait for the command prompt to open.

Navigate to [ACTIVEMQ_INSTALL_DIR]. Change to the `bin` subdirectory.

Type "<kbd>activemq start</kbd>" and press `ENTER`.

ActiveMQ will generate a number of log statements at start-up as shown below:

<img src="{{ site.url }}/assets/images/posts/development/messaging/apache-activemq-start-command.png" alt="apache activemq start command">

One of the log entries mentions 'Apache ActiveMQ started'. This indicates that ActiveMQ was successfully started.

## Step #6: Admin Console

Apache ActiveMQ ships with a web-based administration GUI.

To access the admin console enter following URL in a web browser: `http://localhost:8161/`

If ActiveMQ is up and running a welcome page is displayed.

Click on the `Manage ActiveMQ broker` link

<img src="{{ site.url }}/assets/images/posts/development/messaging/apache-activemq-admin-console-welcome.png" alt="apache activemq admin console welcome">

Enter the following credentials to access the console:

User name="<kbd>admin</kbd>" and Password="<kbd>admin</kbd>".

On the home page you can find some basic statistics on the ActiveMQ broker. In addition there are a number of menus that allow you to explore the different configuration items (queues, topics, connections, …) of the broker.

<img src="{{ site.url }}/assets/images/posts/development/messaging/apache-activemq-admin-console.png" alt="apache activemq admin console">

## Step #7: Stop

To wrap up this tutorial we will stop the running ActiveMQ instance.

Switch back to the command prompt that you used to start ActiveMQ. Press <kbd>CTRL+C</kbd>.

When prompted to `Terminate batch job`, Type "<kbd>Y</kbd>" followed by <kbd>ENTER</kbd>.

The console will return to the prompt and Apache ActiveMQ is shutdown.

<img src="{{ site.url }}/assets/images/posts/development/messaging/apache-activemq-quit-command.png" alt="apache activemq quit command">

**Congratulations, you have installed Apache ActiveMQ on Windows 10!**

Leave a comment if you found this post helpful.

Or if you have any questions.

Thanks!
