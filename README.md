Cohesity REST API Examples
___________________________________________________________________________________
Warning: this code is provided on a best effort basis and is not in any way officially supported or sanctioned by Cohesity. The code is intentionally kept simple torretain value as example code. The code in this repository is provided as-is and the author accepts no liability for damages resulting from its use.

Components
___________________________________________________________________________________
cohesity-api: the Cohesity REST API helper module
You can download the script using the following commands:

# Download Commands
$repoURL = 'https://github.com/danfrankenstein/scripts'
(Invoke-WebRequest -UseBasicParsing -Uri "$repoUrl/cohesity-api.ps1").content | Out-File cohesity-api.ps1; (Get-Content cohesity-api.ps1) | Set-Content cohesity-api.ps1
# End Download Commands

Authenticating to DMaaS
___________________________________________________________________________________
DMaaS uses an API key for authentication. To acquire an API key:

log onto DMaaS
click Settings -> access management -> API Keys
click Add API Key
enter a name for your key
click Save
Immediately copy the API key (you only have one chance to copy the key. Once you leave the screen, you can not access it again). When running a DMaaS compatible script for the first time, you will be prompted for a password. Enter the API key as the password.