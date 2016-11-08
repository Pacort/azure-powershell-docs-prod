---
external help file: Microsoft.Azure.Commands.RedisCache.dll-Help.xml
ms.assetid: 28765C04-36D4-4D20-AE5A-934F563E5A95
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.RedisCache/v2.3.0/Get-AzureRmRedisCachePatchSchedule.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.RedisCache/v2.3.0/Get-AzureRmRedisCachePatchSchedule.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmRedisCachePatchSchedule

## SYNOPSIS
Gets a patch schedule.

## SYNTAX

```
Get-AzureRmRedisCachePatchSchedule -ResourceGroupName <String> -Name <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmRedisCachePatchSchedule** cmdlet gets a patch schedule for a cache in Azure Redis Cache.

## EXAMPLES

### Example 1: Get the patch schedule
```
PS C:\>Get-AzureRmRedisCachePatchSchedule -ResourceGroupName "ResourceGroup13" -Name "RedisCache06"
```

This command gets the patch schedule from the cache named RedisCache06.

## PARAMETERS

### -Name
Specifies the name of a cache.

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

### -ResourceGroupName
Specifies the name of the resource group which contains the cache.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
You can pipe input to this cmdlet by property name, but not by value.

## OUTPUTS

### Microsoft.Azure.Commands.RedisCache.Models.PSScheduleEntry
This cmdlet returns the of patch schedule entries set on the cache.

## NOTES
* Keywords: azure, azurerm, arm, resource, management, manager, redis, cache, web, webapp, website

## RELATED LINKS

[New-AzureRmRedisCachePatchSchedule](xref:ResourceManager/AzureRM.RedisCache/v2.3.0/New-AzureRmRedisCachePatchSchedule.md)

[New-AzureRmRedisCacheScheduleEntry](xref:ResourceManager/AzureRM.RedisCache/v2.3.0/New-AzureRmRedisCacheScheduleEntry.md)

[Remove-AzureRmRedisCachePatchSchedule](xref:ResourceManager/AzureRM.RedisCache/v2.3.0/Remove-AzureRmRedisCachePatchSchedule.md)

