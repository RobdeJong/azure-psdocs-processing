---
external help file: Microsoft.Azure.Commands.AzureBackup.dll-Help.xml
ms.assetid: 9882F1A5-6FFB-4DAF-8ED5-B14596BC939D
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/AzureBackup/Commands.AzureBackup/help/Get-AzureRmBackupVaultCredentials.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/AzureBackup/Commands.AzureBackup/help/Get-AzureRmBackupVaultCredentials.md
gitcommit: https://github.com/Azure/azure-powershell/blob/94e42834e29c78cafba9e3f1e99e14af92561036
updated_at: 04/28/2017 07:04 AM
ms.date: 04/28/2017
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: backup
---

# Get-AzureRmBackupVaultCredentials

## SYNOPSIS
Downloads the vault credentials file for a Backup vault.

## SYNTAX

```
Get-AzureRmBackupVaultCredentials [-TargetLocation] <String> [-Vault] <AzureRMBackupVault> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmBackupVaultCredentials** cmdlet downloads the vault credentials file for an Azure Backup vault.

Backup uses a vault credential file to connect a server to the Azure Backup vault and register it.
You must register a server before Backup can send backup data to the vault.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -TargetLocation
Specifies the destination path where this cmdlet stores the vault credentials file.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Vault
Specifies the Backup vault for which this cmdlet gets a vault credential file.
To obtain an **AzureRmBackupVault** object, use the Get-AzureRmBackupVault cmdlet.

```yaml
Type: AzureRMBackupVault
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### AzureRMBackupVault

## OUTPUTS

### String
This cmdlet returns the name of the vault credential file.

## NOTES

## RELATED LINKS

[Get-AzureRmBackupVault](./Get-AzureRmBackupVault.md)


