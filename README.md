## Still in development
 **Notes:**
> The purpose of this is to fast track install all main programs to get a new device up and running faster then installing all packages one by one. 

> To properly run all install files execution policy will have to be set to unrestricted. The install file will also set the execution policy back to restricted. If you desire a different level on the policy can choose a different one. List of all execution policys will be in the troubleshooting section.



## Contents
- [Requirements](#requirements)
- [Installation](#installation)
- [List of Packages](#list-of-packages)
- [Troueshooting](#troubleshooting)

## Requirements
### Must be in administrator PowerShell
### Execution Policy
- Verify current policy `Get-ExecutionPolicy`
- If not in unrestricted set policy to unrestricted `Set-ExecutionPolicy unrestricted`

## Installation
### Install Chocolatey
- Chocolatey is a package manager that can be used on windows. 
- To install Chocolatey run `Choco_Install.ps1`

- Next: Install all packages by running `Install.ps1`

## List of packages
| Packages                                           | Description |
| ---------------------------------------------------|:-------------:|
| alacritty                                          | terminal emulator |


## Troubleshooting

### Install not working
- PowerShell scripts will not run unless execution policy is set to unrestricted. Another option is to digitaly sign the script and set execution policy to all signed. 

### Execution Policy Options
| Policies                                           | Description |
| ---------------------------------------------------|:-------------:|
| AllSigned                                          | 
| Default                                            |
| RemoteSigned                                       |
| Restricted                                         |
| Undefined                                          |                                     
| Unrestricted                                       |

- To get a more detailed look at each policy refer to [Microsoft](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-7.2)
