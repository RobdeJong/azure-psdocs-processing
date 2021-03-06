---
external help file: Microsoft.Azure.Commands.MachineLearning.dll-Help.xml
online version:
schema: 2.0.0
ms.assetid: 01D650C8-2531-43FE-A1A3-18A2B793A388
updated_at: 11/22/2016 20:11 PM
ms.date: 11/22/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.MachineLearning/v0.10.0/Remove-AzureRmMlWebService.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.MachineLearning/v0.10.0/Remove-AzureRmMlWebService.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0cedc8f73bc96cf5ac4c69144e17b3de601fd3cc
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: machine-learning
---

# Remove-AzureRmMlWebService

## SYNOPSIS
Removes an Azure Machine Learning web service resource.

## SYNTAX

### Remove an Azure ML web service resouce by name and resource group.
```
Remove-AzureRmMlWebService -ResourceGroupName <String> -Name <String> [-Force] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Remove an Azure ML web service specified as an object.
```
Remove-AzureRmMlWebService -MlWebService <WebService> [-Force] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmMlWebService** cmdlet removes the Azure Machine Learning web service resource referenced by resource group and name.

To determine the resource group name of an existing web service, run the Get-AzureRmMlWebService cmdlet to display the web services in your subscription.
Locate the web service, and then look at its web service ID.
The name of the resource group is the fourth element in the ID, just after the **resourceGroups** element.
In the following example the resource group name is **Default-MachineLearning-SouthCentralUS**.

`Properties : Microsoft.Azure.Management.MachineLearning.WebServices.Models.WebServicePropertiesForGraph`
`Id         : /subscriptions/\<subscription ID\>/resourceGroups/Default-MachineLearning-SouthCentralUS/providers/Microsoft.MachineLearning/webServices/Sample5TrainTest.2016.7.22.15.46.31.322`
`Name       : Sample5TrainTest.2016.7.22.15.46.31.322`
`Location   : South Central US`
`Type       : Microsoft.MachineLearning/webServices`
`Tags       : {}`

Alternatively, to determine the resource group name of an existing web service, log on to the Microsoft Azure Machine Learning Web Services portal.
Select the web service.
The resource group name is the fifth element of the URL of the web service, just after the **resourceGroups** element.
In the following example the resource group name is **Default-MachineLearning-SouthCentralUS**.

`https://services.azureml.net/subscriptions/\<subcription ID\>/resourceGroups/Default-MachineLearning-SouthCentralUS/providers/Microsoft.MachineLearning/webServices/Sample5TrainTest.2016.7.22.15.46.31.322`

## EXAMPLES

### Example 1: Remove an Azure Machine Learning web service resource
```
PS C:\>Remove-AzureRmMlWebService -ResourceGroupName "RG001" -Name "WebService001"
```

This command removes the Azure Machine Learning web service named WebService001 that belongs to the resource group named RG001.

## PARAMETERS

### -ResourceGroupName
Specifies the resource group that the web service belongs to.

```yaml
Type: String
Parameter Sets: Remove an Azure ML web service resouce by name and resource group.
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the web service resource that this cmdlet removes.

```yaml
Type: String
Parameter Sets: Remove an Azure ML web service resouce by name and resource group.
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Forces the command to run without asking for user confirmation.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MlWebService
Specifies an instance of the web service that this cmdlet removes.
This parameter can be piped as input.

```yaml
Type: WebService
Parameter Sets: Remove an Azure ML web service specified as an object.
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
* Keywords: azure, azurerm, arm, resource, management, manager, machine, machine learning, azureml

## RELATED LINKS

[Export-AzureRmMlWebService](./Export-AzureRmMlWebService.md)

[Get-AzureRmMlWebService](./Get-AzureRmMlWebService.md)

[Import-AzureRmMlWebService](./Import-AzureRmMlWebService.md)

[New-AzureRmMlWebService](./New-AzureRmMlWebService.md)

[Update-AzureRmMlWebService](./Update-AzureRmMlWebService.md)


