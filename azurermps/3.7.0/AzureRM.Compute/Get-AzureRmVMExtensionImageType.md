---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
ms.assetid: 45F35BDD-969E-4521-9E8D-3499A15434A6
online version:
schema: 2.0.0
updated_at: 03/11/2017 02:03 AM
ms.date: 03/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.8.0/Get-AzureRmVMExtensionImageType.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.8.0/Get-AzureRmVMExtensionImageType.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04f63f6e685743ace2c57eb157574e34e8610b1c
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: big-compute
---

# Get-AzureRmVMExtensionImageType

## SYNOPSIS
Gets the type of an Azure extension.

## SYNTAX

```
Get-AzureRmVMExtensionImageType -Location <String> -PublisherName <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmVMExtensionImageType** cmdlet gets the type of an Azure extension.

## EXAMPLES

### Example 1: Get an extension image type
```
PS C:\>Get-AzureRmVMExtensionImageType -Location "Central US" -PublisherName "Fabrikam"
```

This command gets the extension image type for the specified publisher and location.

## PARAMETERS

### -Location
Specifies the location of an extension.
This cmdlet gets the type for an extension at the location that this parameter specifies.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PublisherName
Specifies the name of a publisher of an extension.
To obtain an extension publisher, use the Get-AzureRmVMImagePublisher cmdlet.
This cmdlet gets the type for an extension from the publisher that this parameter specifies.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmVMExtensionImage](./Get-AzureRmVMExtensionImage.md)

[Get-AzureRmVMImagePublisher](./Get-AzureRmVMImagePublisher.md)


