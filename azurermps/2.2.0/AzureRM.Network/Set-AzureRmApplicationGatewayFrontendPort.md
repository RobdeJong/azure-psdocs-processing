---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.2.0/Set-AzureRmApplicationGatewayFrontendPort.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.2.0/Set-AzureRmApplicationGatewayFrontendPort.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: virtual-network
---

# Set-AzureRmApplicationGatewayFrontendPort

## SYNOPSIS
Modifies a front-end port for an application gateway.

## SYNTAX

```
Set-AzureRmApplicationGatewayFrontendPort -ApplicationGateway <PSApplicationGateway> -Name <String>
 -Port <Int32> [<CommonParameters>]
```

## DESCRIPTION
The Set-AzureRmApplicationGatewayFrontendPort cmdlet modifies a front-end port for an application gateway.

## EXAMPLES

### --------------------------  1:  --------------------------
@{paragraph=PS C:\\\>}



```
PS C:\>$AppGw = Get-AzureRmApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
C:\> $ AppGw = Set-AzureRmApplicationGatewayFrontendPort -ApplicationGateway $ AppGw -Name "FrontEndPort01" -Port 80
```

The first command gets the application gateway named ApplicationGateway01 that belongs to the resource group named ResourceGroup01 and stores it in the $AppGw variable.

## PARAMETERS

### -ApplicationGateway
Specifies the application gateway object with which this cmdlet associates the front-end port.

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
Specifies the name of the front-end port to modify.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Port
Specifies the port number to use for the front-end port.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: True
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
Keywords: azure, azurerm, arm, resource, management, manager, network, networking

## RELATED LINKS

[Add-AzureRmApplicationGatewayFrontendPort]()

[Get-AzureRmApplicationGatewayFrontendPort]()

[New-AzureRmApplicationGatewayFrontendPort]()

[Remove-AzureRmApplicationGatewayFrontendPort]()

