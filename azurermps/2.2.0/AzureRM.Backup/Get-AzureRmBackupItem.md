---
external help file: Microsoft.Azure.Commands.AzureBackup.dll-Help.xml
online version:
schema: 2.0.0
ms.assetid: F493E80A-DAED-4F51-A58A-2851388B1B1C
updated_at: 11/11/2016 23:11 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Backup/v2.1.0/Get-AzureRmBackupItem.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Backup/v2.1.0/Get-AzureRmBackupItem.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: backup
---

# Get-AzureRmBackupItem

## SYNOPSIS
Gets the items under a container in Backup.

## SYNTAX

```
Get-AzureRmBackupItem [-ProtectionStatus <String>] [-Status <String>] [-Type <String>]
 [-Container] <AzureRMBackupContainer> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmBackupItem** cmdlet gets the items in a container in Azure Backup and the protection status of the items.
Enable items for protection by using the Enable-AzureRmBackupProtection cmdlet.

A container that is registered to a Backup vault can have one or more items that can be protected.
For Azure virtual machines, there can be only one item in the virtual machine container.

## EXAMPLES

### Example 1: Get the items in a container
```
PS C:\>$Vault = Get-AzureRmBackupVault -Name "Vault03"
PS C:\> $Container = Get-AzureRmBackupContainer -Vault $Vault -Type AzureVM -Name "DPMSERVER.CONTOSO.COM"
PS C:\> Get-AzureRmBackupItem -Container $Container
Name                    ProtectionStatus       DataSourceStatus       RecoveryPointsCount    ProtectionPolicyName
----                    ----------------       ----------------       -------------------    --------------------
co03-vm                 NotProtected                                  0
```

The first command gets the vault named Vault03 by using the Get-AzureRmBackupVault cmdlet.
The command stores that object in the $Vault variable.

The second command gets a container that has the specified name in the vault in $Vault by using the **Get-AzureRmBackupContainer** cmdlet.
The command stores that object in the $Container variable.

The final command gets the backup item in the container in $Container.

### Example 2: View all properties for an item
```
PS C:\>Get-AzureRmBackupItem -Container $Container | Select-Object -Property *
Name                 : co03-vm
DataSourceStatus     : 
ProtectionStatus     : NotProtected
Type                 : AzureVM
ProtectionPolicyName : 
ProtectionPolicyId   : 
RecoveryPointsCount  : 0
ItemName             : iaasvmcontainer;co03-vm;co03-vm
ContainerType        : AzureVM
ContainerUniqueName  : iaasvmcontainer;co03-vm;co03-vm
ResourceGroupName    : resourcegroup02
ResourceName         : vault03
Location             : southeastasia
```

This command gets the backup item in the container in $Container, and then passes it to the Select-Object cmdlet.
That cmdlet returns all properties of the backup item.
For more information, type `Get-Help Select-Object`.

## PARAMETERS

### -Container
Specifies a container object for which this cmdlet gets backup items.
To obtain an **AzureRmBackupContainer**, use the Get-AzureRmBackupContainer cmdlet.

```yaml
Type: AzureRMBackupContainer
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ProtectionStatus
Specifies the overall protection status of an item in the container.
The acceptable values for this parameter are:

- Protected 
- Protecting  
- NotProtected

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Accepted values: Protected, Protecting, NotProtected

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Status
Specifies the backup status for an item.
The acceptable values for this parameter are: IRPending, Protected, ProtectionError, and ProtectionStopped.
If the *ProtectionStatus* parameter has the value Protected, you can use the *Status* parameter value to filter items.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Accepted values: IRPending, ProtectionStopped, ProtectionError, Protected

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Type
Specifies the type of item that this cmdlet gets.
Currently, the only supported value is AzureVM.

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

### AzureRmBackupContainer

## OUTPUTS

### AzureRmBackupItem

## NOTES

## RELATED LINKS

[Backup-AzureRmBackupItem](./Backup-AzureRmBackupItem.md)

[Disable-AzureRmBackupProtection](./Disable-AzureRmBackupProtection.md)

[Enable-AzureRmBackupProtection](./Enable-AzureRmBackupProtection.md)

[Get-AzureRmBackupContainer](./Get-AzureRmBackupContainer.md)

[Get-AzureRmBackupVault](./Get-AzureRmBackupVault.md)

[Restore-AzureRmBackupItem](./Restore-AzureRmBackupItem.md)


