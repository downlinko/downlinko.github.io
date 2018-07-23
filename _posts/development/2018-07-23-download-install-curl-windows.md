---
title: "Download and Install cURL on Windows"
permalink: /download-install-curl-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install a cURL executable on Windows."
date: 2018-07-23
last_modified_at: 2018-07-23
categories: [Development]
tags: [cURL, Download, Install, Setup, Tutorial, Windows]
published: true
---

<img src="{{ site.url }}/assets/images/posts/development/curl/download-install-curl-windows.png" alt="download install maven curl windows" class="align-right title-image">

Need to download and install [cURL](https://curl.haxx.se/){:target="_blank"} on Windows?

Then look no further!

In this guide you’ll learn how to download the executable…

…and how to configure it so you can use it from command line.

Check it out:

## Step #1: Download

Go to the [cURL download wizard page](https://curl.haxx.se/dlwiz/){:target="_blank"}.

Click on `curl executable`.

<img src="{{ site.url }}/assets/images/posts/development/curl/curl-download-wizard-select-package.png" alt="curl download wizard select package">

Select your operating system.

If needed click on `Select!`.

<img src="{{ site.url }}/assets/images/posts/development/curl/curl-download-wizard-select-operation-system.png" alt="curl download wizard select operation system">

Select the `Generic` flavour.

If needed click on `Select!`.

<img src="{{ site.url }}/assets/images/posts/development/curl/curl-download-wizard-select-flavour.png" alt="curl download wizard select flavour">

Select the `x86_64` CPU.

If needed click on `Select!`.

<img src="{{ site.url }}/assets/images/posts/development/curl/curl-download-wizard-select-cpu.png" alt="curl download wizard select cpu">

Click on `Download!` button for the `ZIP` package.

<img src="{{ site.url }}/assets/images/posts/development/curl/curl-download-wizard-select-cpu.png" alt="curl download wizard select cpu">

Wait for the download to complete.

> Do you want to skip above steps? Here is the direct link to download the most common [cURL 7.61.0 package](https://bintray.com/artifact/download/vszakats/generic/curl-7.61.0-win64-mingw.zip){:target="_blank"} for Windows.

## Step #3: Install

Open the location of the downloaded installer.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-downloaded-binary.png" alt="maven 3-3-9 downloaded binary">

Right-click the ZIP archive file. Select `Extract All...`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-downloaded-binary-extract-all.png" alt="maven 3-3-9 downloaded binary extract all">

Select an extract destination for the Maven files.

In this example, we extract in `C:\Users\Downlinko\tools`.

<img src="{{ site.url }}/assets/images/posts/development/tools-extract-destination.jpg" alt="tools-extract-destination">

Click on `Extract`. This extracts all Maven files under `C:\Users\Downlinko\tools\apache-maven-3.3.9`.

> From now on we refer to this location as `[MAVEN_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-install-dir.png" alt="maven 3-3-9 install dir">

## Step #4: Setup

We need to set up an environment variable that will point to our Maven installation.

Click on the Windows button. Then type "<kbd>env</kbd>" in the search box and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-env.png" alt="windows search env">

Click on the `Edit environment variables for your account` shortcut. Wait for the environment variables window to open.

<img src="{{ site.url }}/assets/images/posts/development/windows-user-environment-variables.png" alt="windows user environment variables">

Click on `New...`.

<img src="{{ site.url }}/assets/images/posts/development/windows-user-environment-variables-new.png" alt="windows user environment variables new">

Enter "<kbd>M2_HOME</kbd>" as variable name. Enter the `[MAVEN_INSTALL_DIR]` as variable value.

In this tutorial the installation directory is: `C:\Users\Downlinko\tools\apache-maven-3.3.9`.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-home-variable.png" alt="maven 3-3-9 home variable">

Next we need to configure the PATH environment variable so we can run Maven from a command prompt.

Select the `PATH` variable. Click on `Edit...`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-edit-path-variable.png" alt="maven 3-3-9 edit path variable">

Append "<kbd>;%M2_HOME%\bin</kbd>" at the end of the variable value.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-path-variable.png" alt="maven 3-3-9 path variable">

Click `OK` once more to close the environment variables window.

> If a PATH variable does not exist you need to create it. Use "<kbd>PATH</kbd>" as variable name and "<kbd>%M2_HOME%\bin</kbd>" as variable value.

## Step #5: Test

To test the setup click on the Windows button. Type "<kbd>cmd</kbd>" in the search box and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Click on the `cmd` shortcut. Wait for the command prompt to open.

Type "<kbd>mvn -version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-version-command.png" alt="maven-version-command">

The above command prints the installed Maven version.

<img src="{{ site.url }}/assets/images/posts/development/maven/maven-3-3-9-version-output.png" alt="maven 3-3-9 version output">

**Congratulations, you have installed Maven 3.3.9 on Windows!**

Good luck and let me know if you liked this post.

Thanks!
