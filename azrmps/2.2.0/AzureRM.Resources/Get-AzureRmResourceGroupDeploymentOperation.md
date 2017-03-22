---
external help file: Microsoft.Azure.Commands.ResourceManager.Cmdlets.dll-Help.xml
online version:
schema: 2.0.0
ms.assetid: 80A9DBA6-A65B-43ED-B11F-28B78C208524
updated_at: 01/09/2017 15:01 PM
ms.date: 01/09/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/marchrelease/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.1.0/Get-AzureRmResourceGroupDeploymentOperation.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/marchrelease/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.1.0/Get-AzureRmResourceGroupDeploymentOperation.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/909020b7dbd03ec23a61b4fe16ccd2762277084c
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
---

# Get-AzureRmResourceGroupDeploymentOperation

## SYNOPSIS
Gets the resource group deployment operation

## SYNTAX

```
Get-AzureRmResourceGroupDeploymentOperation -DeploymentName <String> [-SubscriptionId <Guid>]
 -ResourceGroupName <String> [-ApiVersion <String>] [-Pre] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmResourceGroupDeploymentOperation** cmdlet lists all the operations that were part of a deployment to help you identify and give more information about the exact operations that failed for a particular deployment.
It can also show the response and the request content for each deployment operation.
This is the same information provided in the deployment details on the portal.

To get the request and the response content, enable the setting when submitting a deployment through **New-AzureRmResourceGroupDeployment**.
It can potentially log and expose secrets like passwords used in the resource property or **listKeys** operations that are then returned when you retrieve the deployment operations.
For more on this setting and how to enable it, see New-AzureRmResourceGroupDeployment and Debugging ARM template deployments

## EXAMPLES

### --------------------------  Get1  --------------------------
```
PS C:\> Get-AzureRmResourceGroupDeploymentOperation -DeploymentName test -ResourceGroupName test
```

Gets deployment operation with name "test" under resource group "test"

## PARAMETERS

### -DeploymentName
The deployment name.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Name

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SubscriptionId
The subscription to use.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -ResourceGroupName
The resource group name.

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

### -ApiVersion
When set, indicates the version of the resource provider API to use.
If not specified, the API version is automatically determined as the latest available.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Pre
When set, indicates that the cmdlet should use pre-release API versions when automatically determining which version to use.

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

### -InformationAction
Specifies how this cmdlet responds to an information event.

The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Specifies an information variable.

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

