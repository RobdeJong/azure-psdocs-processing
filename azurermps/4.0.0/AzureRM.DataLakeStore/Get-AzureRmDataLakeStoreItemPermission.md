---
external help file: Microsoft.Azure.Commands.DataLakeStore.dll-Help.xml
ms.assetid: 476E889F-C763-4EFA-AFD6-B037BA6BA0A1
online version:
schema: 2.0.0
updated_at: 05/11/2017 18:05 PM
ms.date: 05/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v4.0.0/Get-AzureRmDataLakeStoreItemPermission.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v4.0.0/Get-AzureRmDataLakeStoreItemPermission.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a9b160b3b332c6a38589f1828b17cf2391c2454e
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: data-lake-store
---

# Get-AzureRmDataLakeStoreItemPermission

## SYNOPSIS
Gets the permission octal of a file or folder in Data Lake Store.

## SYNTAX

```
Get-AzureRmDataLakeStoreItemPermission [-Account] <String> [-Path] <DataLakeStorePathInstance>
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmDataLakeStoreItemPermission** cmdlet gets the the permission octal of a file or folder in Data Lake Store.

## EXAMPLES

### Example 1: Set the permission octal for a file
```
PS C:\>Get-AzureRmDataLakeStoreItemPermission -AccountName "ContosoADL" -Path "/file.txt"
```

This command gets the permission octal for a file.

## PARAMETERS

### -Account
Specifies the Data Lake Store account name.

```yaml
Type: String
Parameter Sets: (All)
Aliases: AccountName

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Path
Specifies the Data Lake Store path of the file or folder, starting with the root directory (/).

```yaml
Type: DataLakeStorePathInstance
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### string
The string representation of the ownership octal

## NOTES
* Alias: Get-AdlStoreItemPermission

## RELATED LINKS

[Set-AzureRmDataLakeStoreItemPermission](./Set-AzureRmDataLakeStoreItemPermission.md)

