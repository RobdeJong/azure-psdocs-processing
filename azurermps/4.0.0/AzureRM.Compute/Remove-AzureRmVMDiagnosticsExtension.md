---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
ms.assetid: 89DA3965-5344-4A1D-AEF1-10EA58E129CF
online version:
schema: 2.0.0
updated_at: 05/11/2017 18:05 PM
ms.date: 05/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v3.0.0/Remove-AzureRmVMDiagnosticsExtension.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v3.0.0/Remove-AzureRmVMDiagnosticsExtension.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a9b160b3b332c6a38589f1828b17cf2391c2454e
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: big-compute
---

# Remove-AzureRmVMDiagnosticsExtension

## SYNOPSIS
Removes the Diagnostics extension from a virtual machine.

## SYNTAX

```
Remove-AzureRmVMDiagnosticsExtension [-ResourceGroupName] <String> [-VMName] <String> [[-Name] <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmVMDiagnosticsExtension** cmdlet removes an Azure Diagnostics extension from a virtual machine.
You must pass the output of this cmdlet to the Update-AzureRmVM cmdlet to implement your changes.

## EXAMPLES

### Example 1: Remove the Diagnostics extension from a virtual machine
```
PS C:\>Remove-AzureRmVMDiagnosticsExtension -ResourceGroupName "ResourceGroup11" -VMName "ContosoVM22" | Update-AzureRmVM
```

This command removes the Diagnostics extension from a virtual machine named ContosoVM22.
The command passes the result to the Update-AzureRmVM cmdlet by using the pipeline operator.
That command updates the virtual machine.

## PARAMETERS

### -Name
Specifies the name of the Diagnostics extension that this cmdlet removes.

```yaml
Type: String
Parameter Sets: (All)
Aliases: ExtensionName

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group of the virtual machine.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VMName
Specifies the name of the virtual machine from which this cmdlet removes a Diagnostics extension.

```yaml
Type: String
Parameter Sets: (All)
Aliases: ResourceName

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

## NOTES

## RELATED LINKS

[Get-AzureRmVMDiagnosticsExtension](./Get-AzureRMVMDiagnosticsExtension.md)

[Set-AzureRmVMDiagnosticsExtension](./Set-AzureRMVMDiagnosticsExtension.md)

[Update-AzureRmVM](./Update-AzureRmVM.md)

