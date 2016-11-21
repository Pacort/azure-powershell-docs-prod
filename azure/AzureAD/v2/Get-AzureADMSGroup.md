---
external help file: AzureAD.Help.xml
online version: https://go.microsoft.com/fwLink/?LinkID=519265&clcid=0x409
schema: 2.0.0
updated_at: 11/19/2016 6:14 PM
ms.date: 11/19/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADMSGroup.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/a3846b3ed4f1f23e2239fc72c70a4cac2804fb12/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADMSGroup.md
ms.topic: reference
ms.prod: 
ms.service: active-directory
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: carolz
id: AzureAD_v2_Get_AzureADMSGroup_md
---

# Get-AzureADMSGroup

## SYNOPSIS
Retrieves a group from the directory

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureADMSGroup [-Filter <String>] [-Top <Int32>]
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureADMSGroup -Id <String>
```

### UNNAMED_PARAMETER_SET_3
```
Get-AzureADMSGroup [-SearchString <String>]
```

## DESCRIPTION
This cmdlet is used to retrieve information about a group from the directory.
The optional parameter -Id can be used to specify the Id of the group that needs to be retrieved.
Without the Id parameter, the -SearchString parameter can be used to find a specific group, or the -Filter parameter can be used to search for a group.
If neither are specified, all groups in the directory are returned.

## EXAMPLES

### Return all groups in the directory
```
Get-AzureADMSGroup

Output:

Id                            : d539a25e-2db2-482a-9dcb-2a0b27fe4f27 
Description                   : 
OnPremisesSyncEnabled         : 
DisplayName                   : 
ADSyncOperators 
OnPremisesLastSyncDateTime    : 
Mail                          : 
MailEnabled                   : False
MailNickname                  : ADSyncOperators 
OnPremisesSecurityIdentifier  : S-1-5-21-2695029449-1154706203-1063139792-1243 
ProxyAddresses                : {} 
SecurityEnabled               : True 
GroupTypes                    : {} 
MembershipRule                : 
MembershipRuleProcessingState :


Id                            : d98ddc78-6e8d-4f0d-8a3f-b923c6ebc14b 
Description                   : 
OnPremisesSyncEnabled         : 
DisplayName                   : Project Icarus 
OnPremisesLastSyncDateTime    : 
Mail                          : 
MailEnabled                   : False 
MailNickname                  : 60f3d02c-0c6e-41da-bb64-128c73b4d9e6 
OnPremisesSecurityIdentifier  : 
ProxyAddresses                : {} 
SecurityEnabled               : True 
GroupTypes                    : {DynamicMembership} 
MembershipRule                : (user.jobtitle -eq "Sales manager") -or ((user.department -eq "Marketing") -and (user.country -eq "Greece")) 
MembershipRuleProcessingState : On
```

This cmdlet returns all groups in the directory.

### Return a specific group based on the group's Id
```
Get-AzureADMSGroup -Id d98ddc78-6e8d-4f0d-8a3f-b923c6ebc14b

Output:


Id                            : d98ddc78-6e8d-4f0d-8a3f-b923c6ebc14b 
Description                   : 
OnPremisesSyncEnabled         : 
DisplayName                   : Project Icarus 
OnPremisesLastSyncDateTime    : 
Mail                          : 
MailEnabled                   : False 
MailNickname                  : 60f3d02c-0c6e-41da-bb64-128c73b4d9e6 
OnPremisesSecurityIdentifier  : 
ProxyAddresses                : {} 
SecurityEnabled               : True 
GroupTypes                    : {DynamicMembership} 
MembershipRule                : (user.jobtitle -eq "Sales manager") -or ((user.department -eq "Marketing") -and (user.country -eq "Greece")) 
MembershipRuleProcessingState : On
```

When the -Id parameter is specified, information about the group with the matching Id is returned

## PARAMETERS

### -Filter
String to be used to filter for a specific (set of) groups

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Id
The Id of the group that is to be retrieved

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -SearchString
The SearchString parameter allows you to search for specific objects.
This includes the DisplayName and Description attribute as well as addtional string attributes for an object

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_3
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Top
@{Text=}

```yaml
Type: Int32
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

## INPUTS

### System.String
System.Nullable\`1\[\[System.Int32, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089\]\]

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS
