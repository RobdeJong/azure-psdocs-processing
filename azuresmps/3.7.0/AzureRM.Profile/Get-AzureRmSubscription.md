---
external help file: Microsoft.Azure.Commands.Profile.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 03/27/2017 18:03 PM
ms.date: 03/27/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/AzureRM.Profile/v2.7.0/Get-AzureRmSubscription.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/AzureRM.Profile/v2.7.0/Get-AzureRmSubscription.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4481ba5d382a258a76528a60b3c1580b75fdff10
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: subscription
---

# Get-AzureRmSubscription

## SYNOPSIS
Get subscriptions that the current account can access.

## SYNTAX

### ListByIdInTenant (Default)
```
Get-AzureRmSubscription [-SubscriptionId <String>] [-TenantId <String>] [<CommonParameters>]
```

### ListByNameInTenant
```
Get-AzureRmSubscription [-SubscriptionName <String>] [-TenantId <String>] [<CommonParameters>]
```

## DESCRIPTION
The Get-AzureRmSubscription cmdlet gets the subscription ID, subscription name, and home tenant for subscriptions that the current account can access.

## EXAMPLES

### Example 1: Get all subscriptions in all tenants
```
PS C:\>Get-AzureRmSubscription -All

Subscription Name : Contoso Subscription 1
SubscriptionId    : xxxx-xxxx-xxxx-xxxx
TenantId          : yyyy-yyyy-yyyy-yyyy
```

This command gets all subscriptions in all tenants that are authorized for the current account.

### Example 2: Get all subscriptions for a specific tenant
```
PS C:\>Get-AzureRmSubscription -TenantId "xxxx-xxxx-xxxx-xxxx"

Subscription Name : Contoso Subscription 1
SubscriptionId    : yyyy-yyyy-yyyy-yyyy
TenantId          : xxxx-xxxx-xxxx-xxxx

Subscription Name : Contoso Subscription 2
SubscriptionId    : yyyy-yyyy-yyyy-yyyy
TenantId          : xxxx-xxxx-xxxx-xxxx
```

List all subscriptions in the given tenant that are authorized for the current account.

### Example 3: Get all subscriptions in the current tenant
```
PS C:\>Get-AzureRmSubscription

Subscription Name : Contoso Subscription 1
SubscriptionId    : yyyy-yyyy-yyyy-yyyy
TenantId          : xxxx-xxxx-xxxx-xxxx

Subscription Name : Contoso Subscription 2
SubscriptionId    : yyyy-yyyy-yyyy-yyyy
TenantId          : xxxx-xxxx-xxxx-xxxx
```

This command gets all subscriptions in the current tenant that are authorized for the current user.

### Example 4: Change the current context to use a specific subscription
```
PS C:\>Get-AzureRmSubscription -SubscriptionId "xxxx-xxxx-xxxx-xxxx" -TenantId "yyyy-yyyy-yyyy-yyyy" | Set-AzureRmContext

Subscription Name : Contoso Subscription 1
SubscriptionId    : xxxx-xxxx-xxxx-xxxx
TenantId          : yyyy-yyyy-yyyy-yyyy
```

This command gets the specified subscription, and then sets the current context to use it.
All subsequent cmdlets in this session use the new subscription (Contoso Subscription 1) by default.

## PARAMETERS

### -SubscriptionId
Specifies the ID of the subscription to get.

```yaml
Type: String
Parameter Sets: ListByIdInTenant
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SubscriptionName
Specifies the name of the subscription to get.

```yaml
Type: String
Parameter Sets: ListByNameInTenant
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TenantId
Specifies the ID of the tenant that contains subscriptions to get.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### PSAzureSubscription

## NOTES

## RELATED LINKS

