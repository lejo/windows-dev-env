## Setup Windows 10 for Modern Development
A fresh Windows isn't entirely ready for modern development, but all the tools you need are available. A good terminal, popular bash tools, Git, a decent package manager - when properly setup, modern development on Windows can be a lot of fun. In particular, this document outlines how to configure your Windows in such a way that it can easily handle most development tasks usually run on a Mac OS X or a Linux distro.

## Install the prerequisites

 * Enable Developer Mode (Settings - Update & security > For developers)
 * Search for “Windows Features” and choose “Turn Windows features on or off” and enable Windows Subsystem for Linux.
 * Install [Powershell](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-7.1)
 * Install [Boxstarter](https://boxstarter.org/InstallBoxstarter) using the Boxstarter zip file method.


## Run dev setup script as follows:

Start PowerShell as Administrator and run:

```powershell
START http://boxstarter.org/package/nr/url?https://raw.githubusercontent.com/lejo/windows-development-environment/master/boxstarter
```

This will install the following:

 * Package Management
 * Better Terminal
 * PowerShell Profile
 * Node & NPM
 * Git
 * VS Code IDE
 * Common Languages like Java, .Net, Ruby, Go & Python
 * Docker & Kubernetes
 * Cloud CLI - Azure & AWS
 * Basic Tools - 7zip & sysinternals
 

#### Package Management: Chocolatey
Chocolatey is a powerful package manager for Windows, working sort of like apt-get or homebrew. Let's get that first. Fire up CMD.exe as Administrator and run:

```powershell
@powershell -NoProfile -ExecutionPolicy Bypass -Command "iex ((new-object net.webclient).DownloadString('https://chocolatey.org/install.ps1'))" && SET PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin
```

Once done, you can install packages by running `cinst` (short for `choco install`). Most packages below will be installed with Chocolatey.
