---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
ms.assetid: 847729B7-634A-4F54-839F-46606F28F783
online version:
schema: 2.0.0
updated_at: 05/11/2017 18:05 PM
ms.date: 05/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v4.0.0/Get-AzureRmApplicationGatewayProbeConfig.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v4.0.0/Get-AzureRmApplicationGatewayProbeConfig.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a9b160b3b332c6a38589f1828b17cf2391c2454e
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: virtual-network
---

# Get-AzureRmApplicationGatewayProbeConfig

## SYNOPSIS
Gets an existing health probe configuration from an Application Gateway.

## SYNTAX

```
Get-AzureRmApplicationGatewayProbeConfig [-Name <String>] -ApplicationGateway <PSApplicationGateway>
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmApplicationGatewayProbeConfig** cmdlet gets an existing health probe configuration from an Application Gateway.

## EXAMPLES

### Example 1: Get an existing probe from an application gateway
```
PS C:\>Get-AzureRmApplicationGatewayProbeConfig -ApplicationGateway Gateway -Name "Probe02"
```

This command gets the health probe named Probe02 from the application gateway named Gateway.

## PARAMETERS

### -ApplicationGateway
Specifies the application gateway to which this cmdlet gets a probe configuration.

```yaml
Type: PSApplicationGateway
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
Specifies the name of the probe.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add a probe to an existing application gateway](https://azure.microsoft.com/en-us/documentation/articles/application-gateway-create-probe-ps/#add-a-probe-to-an-existing-application-gateway)

[Add-AzureRmApplicationGatewayProbeConfig](./Add-AzureRmApplicationGatewayProbeConfig.md)

[New-AzureRmApplicationGatewayProbeConfig](./New-AzureRmApplicationGatewayProbeConfig.md)

[Remove-AzureRmApplicationGatewayProbeConfig](./Remove-AzureRmApplicationGatewayProbeConfig.md)

[Set-AzureRmApplicationGatewayProbeConfig](./Set-AzureRmApplicationGatewayProbeConfig.md)

