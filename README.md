# Setup Hyper-V WSL machine with openVPN server
This is a documentation repository describing how you can make a VPN server on a Hyper V machine with WIndows Subsystem for Linux version 2 and Ubuntu 20.04

## Glossary
WSL - Windows Subsystem for Linux

## Setup the Hyper-V machine on Windows
### Enabling the Windows features to support WSL 2
First of all, make sure that you run the PowerShell command line tool as an administrator. To do so, you need to search for PowerShell in your Windows start menu, and then when you identifided the PowerShell, right click and choose the "Run as administrator" option.

After this, you should see the PowerShell window opening. 

Run the following two commands to enable the necessary Windows Features for WSL 2. 

Note: You don't need to restart after each execution. You can restart after both commands were executed successfully.

```bash
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```

and

```bash
Enable-WindowsOptionalFeature -Online -FeatureName VirtualMachinePlatform
```
