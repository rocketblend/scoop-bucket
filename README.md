# Scoop Bucket

Welcome to the **Scoop bucket** repository! This repository is maintained by RocketBlend and contains a collection of manifests for various RocketBlend related software packages and tools that can be installed using the Scoop command-line installer for Windows.

## Table of Contents

- [What is Scoop?](#what-is-scoop)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installing Scoop](#installing-scoop)
  - [Adding Our Bucket](#adding-our-bucket)
  - [Searching and Installing Packages](#searching-and-installing-packages)

## What is Scoop?

[Scoop](https://scoop.sh/) is a command-line package manager for Windows inspired by apt, yum, and similar tools on other platforms. Scoop allows you to easily manage and install software packages from the command line, without the need for complex installations or dealing with the Windows registry.

## Getting Started

### Prerequisites

Before you can use this repository, you need to have the following software installed on your system:

- Windows 7 or later
- [PowerShell 5.0 or later](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-windows-powershell?view=powershell-7.1)

### Installing Scoop

To install Scoop on your system, open a PowerShell window with administrative privileges and run the following command:

```powershell
Set-ExecutionPolicy RemoteSigned -scope CurrentUser
```

Then, run the following command to install Scoop:

```powershell
Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://get.scoop.sh')
```

### Adding Our Bucket

To add the RocketBlend bucket repository to your Scoop installation, run the following command:

```powershell
scoop bucket add rocketblend "https://github.com/rocketblend/scoop-bucket"
```

### Searching and Installing Packages

You can search for packages in the RocketBlend Scoop-Bucket repository using the following command:

```powershell
scoop search <package-name>
```

To install a package from the repository, run the following command:

```powershell
scoop install <package-name>
```

For more information on Scoop commands and usage, refer to the [official Scoop documentation](https://github.com/lukesampson/scoop/wiki).