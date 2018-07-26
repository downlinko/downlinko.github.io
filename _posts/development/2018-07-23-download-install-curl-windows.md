---
title: "Download and Install cURL on Windows"
permalink: /download-install-curl-windows.html
excerpt: "A detailed step-by-step tutorial on how to download and install a cURL executable on Windows 10."
date: 2018-07-23
last_modified_at: 2018-07-23
header:
  teaser: "assets/images/posts/development/jdk/download-install-jdk-10-windows.png"
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

Click on `Select!`.

<img src="{{ site.url }}/assets/images/posts/development/curl/curl-download-wizard-select-operation-system.png" alt="curl download wizard select operation system">

Select the `Generic` flavour.

Click on `Select!`.

<img src="{{ site.url }}/assets/images/posts/development/curl/curl-download-wizard-select-flavour.png" alt="curl download wizard select flavour">

Select the `x86_64` CPU.

Click on `Select!`.

<img src="{{ site.url }}/assets/images/posts/development/curl/curl-download-wizard-select-cpu.png" alt="curl download wizard select cpu">

Click on the `Download!` button for the `ZIP` package.

At the time of writing the recommended cURL version was `7.61.0`.

<img src="{{ site.url }}/assets/images/posts/development/curl/curl-7-61-0-zip-package.png" alt="curl 7-61-0 zip package">

Wait for the download to complete.

> Do you want to skip above steps? Here is the direct link to download the most common [cURL 7.61.0 package](https://bintray.com/artifact/download/vszakats/generic/curl-7.61.0-win64-mingw.zip){:target="_blank"} for Windows.

## Step #2: Install

Open the location of the downloaded package.

<img src="{{ site.url }}/assets/images/posts/development/curl/curl-downloaded-zip-package.png" alt="curl downloaded zip package">

Right-click the ZIP archive file. Select `Extract All…`.

<img src="{{ site.url }}/assets/images/posts/development/curl/curl-downloaded-zip-package-extract-all.png" alt="curl downloaded zip package extract all">

Select an extract destination for the cURL files.

In this example, we extract in `C:\Users\Downlinko\tools`.

Click on `Extract`.

<img src="{{ site.url }}/assets/images/posts/development/tools-extract-destination.png" alt="tools-extract-destination">

This extracts all cURL files under `C:\Users\Downlinko\tools\curl-7.61.0-win64-mingw`.

> From now on we refer to this location as `[CURL_INSTALL_DIR]`.

<img src="{{ site.url }}/assets/images/posts/development/curl/curl-install-dir.png" alt="curl install dir">

## Step #3: Setup

We need to set up an environment variable that will point to our cURL installation.

Click on the search button. Then type "<kbd>env</kbd>" (without quotes).

> On Windows 7 click on the Windows button.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-env.png" alt="windows search env">

Click on the `Edit environment variables for your account` shortcut. Wait for the environment variables window to open.

Click on `New...`.

<img src="{{ site.url }}/assets/images/posts/development/windows-account-environment-variables-new.png" alt="windows account environment variables new">

Enter "<kbd>CURL_HOME</kbd>" as variable name. Enter the `[CURL_INSTALL_DIR]` as variable value.

In this tutorial the installation directory is: `C:\Users\Downlinko\tools\curl-7.61.0-win64-mingw`.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/curl/curl-home-variable.png" alt="curl home variable">

Next we need to configure the PATH environment variable so we can run Maven from a command prompt.

Click on `New...` once more.

<img src="{{ site.url }}/assets/images/posts/development/curl/windows-account-environment-variables-curl.png" alt="windows account environment variables curl">

Enter "<kbd>PATH</kbd>" as variable name. Enter "<kbd>%CURL_HOME%\bin</kbd>" as variable value.

Click `OK`.

<img src="{{ site.url }}/assets/images/posts/development/curl/curl-path-variable.png" alt="curl path variable">

Click `OK` once more to close the environment variables window.

<img src="{{ site.url }}/assets/images/posts/development/curl/windows-account-environment-variables-curl-path.png" alt="windows account environment variables curl path">

> If a PATH variable already exists you need to edit it. Select the `PATH` variable and click on `Edit`. Append "<kbd>;%CURL_HOME%\bin</kbd>" at the end of the variable value and click `OK`.

## Step #4: Test

To test the setup click on the Windows button. Type "<kbd>cmd</kbd>" in the search box and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/windows-search-cmd.png" alt="windows search cmd">

Click on the `cmd` shortcut. Wait for the command prompt to open.

Type "<kbd>curl --version</kbd>" and press `ENTER`.

<img src="{{ site.url }}/assets/images/posts/development/curl/curl-version-command.png" alt="curl-version-command">

The above command prints the installed cURL version.

<img src="{{ site.url }}/assets/images/posts/development/curl/curl-7-61-0-version-output.png" alt="curl 7-61-0 version output">

**Congratulations, you have installed cURL on Windows!**

Leave a comment below if this post was helpful.

Thanks!
