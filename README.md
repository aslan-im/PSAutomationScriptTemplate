# PSAutomationScriptTemplate

### SYNOPSIS

This is a template for the Graph API scripts that can be used for the other script types as well.
The example of the Graph function and tests for it can be found in functions directory (Pester module was used for unit tests)

### DESCRIPTION

This template is developed mostly for Graph API scripts. It conctains a few dependencies, such as:
.Logging - module for logging to files or where you need. This module can be reconfigured for logging to the console, Event Veiewer and another places
.GraphApiRequests - simple module for Graph API Scripts. You just need to use 2 functions, Get-GraphToken and Invoke-GraphApiRequest
.Microsoft.PowerShell.SecretStore - it is Microsoft recommended module for secrets storing. More information can be got on official module page.
.Microsoft.PowerShell.SecretManagement - Microsoft recommended module for managing secretstore. Using this module you can create new vaults and read/write secrets
Template consists of the parts described below:

- checking and importing required modules
- internal functions
- common variables, such as date, path to config file and etc...
- logging part, where you can find logging module configuration
- config file checking and reading
- configuration reading
- checking and reading the vault with secrets and credential
- main part, the script body

### INPUTS

There is no input in the template

### OUTPUTS

The output will be the log file by default

### NOTES

Template version: 0.1.0
Owner: Aslan Imanalin
Github: @aslan-im
