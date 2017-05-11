---
external help file: Microsoft.Azure.Commands.ServerManagement.dll-Help.xml
ms.assetid: 4EE30890-B09B-4811-88AD-4BF4FD47E431
online version:
schema: 2.0.0
updated_at: 05/11/2017 18:05 PM
ms.date: 05/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ServerManagement/v3.0.0/Get-AzureRmServerManagementNode.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ServerManagement/v3.0.0/Get-AzureRmServerManagementNode.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a9b160b3b332c6a38589f1828b17cf2391c2454e
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: server-management
---

# Get-AzureRmServerManagementNode

## SYNOPSIS
Gets one or more Server Management nodes.

## SYNTAX

### ByNodeName
```
Get-AzureRmServerManagementNode [[-ResourceGroupName] <String>] [[-NodeName] <String>] [<CommonParameters>]
```

### ByNode
```
Get-AzureRmServerManagementNode [-Node] <Node> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmServerManagementNode** cmdlet gets one or more Azure Server Management nodes.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -Node
Specifies an existing node from which to get the *ResourceGroupName* and the *NodeName* parameters.

```yaml
Type: Node
Parameter Sets: ByNode
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -NodeName
Specifies the name of the node for which this cmdlet gets.

```yaml
Type: String
Parameter Sets: ByNodeName
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group in which the nodes belong to.

```yaml
Type: String
Parameter Sets: ByNodeName
Aliases: 

Required: False
Position: 0
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

[New-AzureRmServerManagementNode](./New-AzureRmServerManagementNode.md)

[Remove-AzureRmServerManagementNode](./Remove-AzureRmServerManagementNode.md)

