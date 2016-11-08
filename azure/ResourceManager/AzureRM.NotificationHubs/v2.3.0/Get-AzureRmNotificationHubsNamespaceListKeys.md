---
external help file: Microsoft.Azure.Commands.NotificationHubs.dll-Help.xml
ms.assetid: F2781ACF-B389-4646-A978-08576CC05952
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.NotificationHubs/v2.3.0/Get-AzureRmNotificationHubsNamespaceListKeys.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.NotificationHubs/v2.3.0/Get-AzureRmNotificationHubsNamespaceListKeys.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmNotificationHubsNamespaceListKeys

## SYNOPSIS
Gets the primary and secondary connection strings associated with a notification hub namespace authorization rule.

## SYNTAX

```
Get-AzureRmNotificationHubsNamespaceListKeys [-ResourceGroup] <String> [-Namespace] <String>
 [-AuthorizationRule] <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmNotificationHubsNamespaceListKeys** cmdlet returns the primary and secondary connection strings for a Shared Access Signature (SAS) authorization rule assigned to a notification hub namespace.

Authorization rules manage user rights to a notification hub namespace.
Each rule includes a primary and a secondary connection string.

## EXAMPLES

### Example 1: Get the primary and secondary connection strings for an authorization rule
```
PS C:\>Get-AzureRmNotificationHubsNamespaceListKeys -Namespace "ContosoNamespace" -ResourceGroup "ContosoNotificationsGroup" -AuthorizationRule "ListenRule"
```

This command returns the primary and secondary connection strings for the authorization rule named ListenRule assigned to the ContosoNamespace namespace.
When you run this command you must include the name of the resource group that the namespace is assigned to.

## PARAMETERS

### -ResourceGroup
Specifies the resource group to which the namespace is assigned.

Resource groups organize items such as namespaces, notification hubs, and authorization rules in ways that help simply inventory management and Azure administration.

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

### -Namespace
Specifies the namespace containing the connection strings that this cmdlet gets.

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

### -AuthorizationRule
Specifies the name of a SAS authentication rule.
These rules determine the type of access that users have to the notification hub.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmNotificationHubsNamespace](xref:ResourceManager/AzureRM.NotificationHubs/v2.3.0/Get-AzureRmNotificationHubsNamespace.md)

[Get-AzureRmNotificationHubsNamespaceAuthorizationRules](xref:ResourceManager/AzureRM.NotificationHubs/v2.3.0/Get-AzureRmNotificationHubsNamespaceAuthorizationRules.md)

