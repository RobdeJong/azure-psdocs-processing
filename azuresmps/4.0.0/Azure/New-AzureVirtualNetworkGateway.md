---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.Network.dll-Help.xml
ms.assetid: A40F3BBB-4DC6-452E-A939-ED610F541EB1
online version:
schema: 2.0.0
updated_at: 05/12/2017 22:05 PM
ms.date: 05/12/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure/v4.0.0/New-AzureVirtualNetworkGateway.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure/v4.0.0/New-AzureVirtualNetworkGateway.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/3b96c1e0b28fc56dfbf6de55728d5478e0d02def
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-asm
---

# New-AzureVirtualNetworkGateway

## SYNOPSIS
Creates an Azure virtual network gateway.

## SYNTAX

```
New-AzureVirtualNetworkGateway -VNetName <String> -GatewayName <String> [-GatewayType <String>]
 [-GatewaySKU <String>] [-Location <String>] [-VnetId <String>] [-Asn <UInt32>] [-PeerWeight <Int32>] [-Force]
 [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureVirtualNetworkGateway** cmdlet creates an Azure virtual network gateway.

## EXAMPLES

## PARAMETERS

### -Asn
Specifies the autonomous system number (ASN).

```yaml
Type: UInt32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Do not confirm Azure Virtual Network Gateway Creation

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

### -GatewayName
Specifies the name of the gateway.

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

### -GatewaySKU
Specifies the SKU of the virtual network gateway that this cmdlet creates.
Valid values are:

- Default
- Standard
- HighPerformance

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

### -GatewayType
Specifies the type of gateway.

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

### -Location
Specifies the location.

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

### -PeerWeight
```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

```yaml
Type: AzureSMProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -VnetId
Specifies the ID of a virtual network.

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

### -VNetName
Specifies a virtual network.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureVirtualNetworkGateway](./Get-AzureVirtualNetworkGateway.md)

[Remove-AzureVirtualNetworkGateway](./Remove-AzureVirtualNetworkGateway.md)

[Resize-AzureVirtualNetworkGateway](./Resize-AzureVirtualNetworkGateway.md)
