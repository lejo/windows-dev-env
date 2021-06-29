## Setup Windows 10 for Modern Development
This document outlines how to configure your Windows in a way that it can easily handle development tasks. 

## Install the prerequisites

 * Get Local Admin Rights for your workstation. See [instructions here](https://softwareone.service-now.com/sp/?sys_kb_id=e9a6abdbdc050e00b82b7c37157ee971&id=kb_article_view&sysparm_rank=1&sysparm_tsqueryId=47f0fde11b05f450351debd9bb4bcbee)
 * Open a new Windows Powershell with Administrator rights. Search for "Windows Powershell", right click and "Run as Administrator"


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
