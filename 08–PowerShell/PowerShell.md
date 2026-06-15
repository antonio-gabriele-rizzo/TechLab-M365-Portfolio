# PowerShell Administration

Microsoft 365 administration using PowerShell.

## Objectives

This project demonstrates the use of PowerShell for Microsoft 365 administration. The activities performed include installing and configuring Microsoft Graph PowerShell, connecting to Microsoft 365 services, running administrative commands, generating reports, automating repetitive tasks, and managing Exchange Online.

Topics covered:

- Microsoft Graph PowerShell
- Exchange Online PowerShell
- Basic administration commands
- Reporting commands
- Administrative automation

## Environment

- Microsoft 365 Business Basic trial tenant
- Windows 11
- Windows PowerShell 5.1
- Microsoft Graph PowerShell SDK 2.37.0
- ExchangeOnlineManagement 3.10.0

## Troubleshooting

During the installation of the Microsoft Graph PowerShell module, the installation process failed with a directory creation error.

### Issue Identified

```powershell
Install-Module Microsoft.Graph -Scope CurrentUser
```

![Microsoft Graph installation error](screenshots/powershell-module-install-error.png)

### Investigation

![PowerShell blocked by Controlled Folder Access](screenshots/powershell-folder-access-blocked.png)

### Resolution

![Controlled Folder Access configuration](screenshots/controlled-folder-access-enabled.png)

![PowerShell added to allowed applications](screenshots/powershell-allowed-app.png)

## Microsoft Graph PowerShell

### Installing Microsoft Graph

```powershell
Install-Module Microsoft.Graph -Scope CurrentUser
```

![Microsoft Graph module installation](screenshots/graph-module-installed.png)

```powershell
Get-Module -ListAvailable Microsoft.Graph*
```

### Connecting to Microsoft Graph

```powershell
Connect-MgGraph -Scopes "User.Read.All","Directory.Read.All"
```

![Microsoft Graph connection](screenshots/graph-connected.png)

### Verifying the Connection

```powershell
Get-MgContext
```

![Microsoft Graph context](screenshots/graph-context.png)

## Basic Administration Commands

```powershell
Get-MgUser
```

![Microsoft Graph users](screenshots/graph-users.png)

```powershell
Get-MgGroup
```

![Microsoft Graph groups](screenshots/Get-MgGroup.png)

## Reporting Commands

```powershell
Get-MgUser -Property DisplayName,AccountEnabled |
Select DisplayName, AccountEnabled
```

![User report](screenshots/user-report.png)

```powershell
Get-MgUser -Property DisplayName,AccountEnabled |
Select DisplayName, AccountEnabled |
Export-Csv "$HOME\Documents\UsersReport.csv" -NoTypeInformation
```

![Exporting report data](screenshots/user-report-export-csv.png)

![CSV report](screenshots/user-report-csv.png)

## Administrative Automation

```powershell
Get-MgUser -Property DisplayName,AccountEnabled |
Select DisplayName, AccountEnabled |
Export-Csv "$HOME\Documents\UsersReport.csv" -NoTypeInformation

Write-Host "User report exported successfully."
```

![PowerShell automation script](screenshots/automation-script-created.png)

```powershell
.\UserReport.ps1
```

![Script execution](screenshots/automation-script-executed.png)

## Exchange Online PowerShell

```powershell
Install-Module ExchangeOnlineManagement -Scope CurrentUser
```

![Exchange Online module installation](screenshots/exchange-module-installed.png)

```powershell
Connect-ExchangeOnline
Get-ConnectionInformation
```

![Exchange Online connection](screenshots/exchange-connected.png)

```powershell
Get-Mailbox | Select DisplayName, Alias, PrimarySmtpAddress
```

![Exchange mailboxes](screenshots/exchange-mailboxes.png)

## Conclusion

This project demonstrated the use of PowerShell for Microsoft 365 administration using both Microsoft Graph PowerShell and Exchange Online PowerShell.
