---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
ms.assetid: 42986C68-14EA-4ADA-9381-3B7A9DF11971
online version:
schema: 2.0.0
updated_at: 05/03/2017 06:05 AM
ms.date: 05/03/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Unregister-ServiceFabricApplicationType.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Unregister-ServiceFabricApplicationType.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/40385fc07259a8f5f0d2cec04a231e9cd42fcff3
ms.topic: reference
author: oanapl
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: vipulm
open_to_public_contributors: false
ms.service: service-fabric
---

# Unregister-ServiceFabricApplicationType

## SYNOPSIS
Unregisters a Service Fabric application type.

## SYNTAX

```
Unregister-ServiceFabricApplicationType [-ApplicationTypeName] <String> [-ApplicationTypeVersion] <String>
 [-Async] [-Force] [-TimeoutSec <Int32>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Unregister-ServiceFabricApplicationType** cmdlet unregisters a Service Fabric application type. The application type must have been previously registered with [Register-ServiceFabricApplicationType](.\Register-ServiceFabricApplicationType.md).

Before you unregister an application type, you must use the [Remove-ServiceFabricService](./Remove-ServiceFabricService.md) cmdlet to remove services that you base on the application. Use the [Remove-ServiceFabricApplication](./Remove-ServiceFabricApplication.md) cmdlet to remove instances of the application.
If you unregister an application type, the application package is removed from the image store.

To manage Service Fabric clusters, start Windows PowerShell by using the Run as administrator option.
Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the [Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md) cmdlet.

## EXAMPLES

### Example 1: Unregister an application type
```
PS C:\> Unregister-ServiceFabricApplicationType -ApplicationTypeName "CalcServiceApp" -ApplicationTypeVersion "1.0" -Force
```

This command unregisters the application type CalcServiceApp with version 1.0.
Because the command includes the *Force* parameter, the cmdlet does not prompt you for confirmation.

## PARAMETERS

### -ApplicationTypeName
Specifies the name of a Service Fabric application type.
The cmdlet unregisters the type that you specify.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ApplicationTypeVersion
Specifies the version of a Service Fabric application type.
The cmdlet unregisters the type that has the version that you specify.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Async
{{Fill Async Description}}

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

### -TimeoutSec
Specifies the time-out period, in seconds, for the operation.

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
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### String
This cmdlet accepts the application type name or application type version.

## OUTPUTS

### System.Object
This cmdlet returns the status of the operation as a string.

## NOTES

## RELATED LINKS

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[Get-ServiceFabricApplicationType](./Get-ServiceFabricApplicationType.md)

[Get-ServiceFabricClusterConnection](./Get-ServiceFabricClusterConnection.md)

[Register-ServiceFabricApplicationType](./Register-ServiceFabricApplicationType.md)

[Remove-ServiceFabricApplication](./Remove-ServiceFabricApplication.md)

[Remove-ServiceFabricService](./Remove-ServiceFabricService.md)
