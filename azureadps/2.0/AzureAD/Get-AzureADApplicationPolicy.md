---
external help file: Microsoft.Open.MS.GraphBeta.PowerShell.dll-Help.xml
ms.assetid: 20303C1F-EB5F-4326-B522-2241D736ED4E
online version:
schema: 2.0.0
updated_at: 04/24/2017 21:04 PM
ms.date: 04/24/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2.1/Get-AzureADApplicationPolicy.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2.1/Get-AzureADApplicationPolicy.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/58dbfa14efee8bd6121cb76044ff15751eaab5bc
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: carolz
ms.service: active-directory
---

# Get-AzureADApplicationPolicy

## SYNOPSIS
Gets an application policy.

## SYNTAX

```
Get-AzureADApplicationPolicy -Id <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureADApplicationPolicy** cmdlet gets an Azure Active Directory application policy.

## EXAMPLES

### Example 1: Get an application policy
```
PS C:\>Get-AzureADApplicationPolicy -ObjectId "<object id of application>"
```

This command gets the specified application policy.

## PARAMETERS

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
Specifies a variable in which to store an information event message.

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

### -Id
The ID of the application for which you need to retrieve the policy

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AzureADApplicationPolicy](./Add-AzureADApplicationPolicy.md)
[Remove-AzureADApplicationPolicy](./Remove-AzureADApplicationPolicy.md)

