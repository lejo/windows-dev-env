## Setup Windows 10 for Modern Development
This document outlines how to configure your Windows to handle development tasks. 

## Install the prerequisites

 * Get Local Admin Rights for your workstation. See [instructions here](https://softwareone.service-now.com/sp/?sys_kb_id=e9a6abdbdc050e00b82b7c37157ee971&id=kb_article_view&sysparm_rank=1&sysparm_tsqueryId=47f0fde11b05f450351debd9bb4bcbee)
 * Install boxstarter by running the following command:

Start PowerShell as Administrator and run the command below. This will take around 60 minutes to complete. 

```powershell
iex ((New-Object System.Net.WebClient).DownloadString('https://boxstarter.org/bootstrapper.ps1')); Get-Boxstarter -Force
```


## Run dev setup script to install basic development tools and development kits. 

Start PowerShell as Administrator and run the command below. This will take around 60 minutes to complete. *Make sure to close all other open applications and windows as your computer will restart at the end of this.*

```powershell
Install-BoxstarterPackage -PackageName https://raw.githubusercontent.com/lejo/windows-development-environment/master/boxstarter -DisableReboots
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

Please make sure the entire process completes and the summary at the end shows no Errors. Keep in mind, you will see see warnings through out the installation and those are ok.

```powershell
Errors       : {}
ComputerName : localhost
Completed    : True
FinishTime   : 6/29/2021 3:35:00 PM
StartTime    : 6/29/2021 2:48:13 PM
```


## Configure tools
