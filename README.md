## Setup Windows 10 for Modern Development
This document outlines how to configure your Windows in a way that it can easily handle development tasks. 

## Install the prerequisites

 * Get Local Admin Rights for your workstation. See [instructions here](https://softwareone.service-now.com/sp/?sys_kb_id=e9a6abdbdc050e00b82b7c37157ee971&id=kb_article_view&sysparm_rank=1&sysparm_tsqueryId=47f0fde11b05f450351debd9bb4bcbee)
 * Install boxstarter
```powershell
iex ((New-Object System.Net.WebClient).DownloadString('https://boxstarter.org/bootstrapper.ps1')); Get-Boxstarter -Force
```


## Run dev setup script as follows:

Start PowerShell as Administrator and run:

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
