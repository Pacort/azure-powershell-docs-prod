---
external help file: Microsoft.Azure.Commands.Insights.dll-Help.xml
online version: .\Get-AzureRmDiagnosticSetting.md
schema: 2.0.0
ms.assetid: 67810F79-AD11-491E-9D70-F3F3DA2E79D1
updated_at: 10/18/2016 9:38 PM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Insights/v1.0.12/Set-AzureRmDiagnosticSetting.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/23cdb8705d4ab9807c0e21b238f3b134a7d49c7d/azureps-cmdlets-docs/ResourceManager/AzureRM.Insights/v1.0.12/Set-AzureRmDiagnosticSetting.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureRmDiagnosticSetting

## SYNOPSIS
Sets the logs and metrics settings for the resource.

## SYNTAX

```
Set-AzureRmDiagnosticSetting -ResourceId <String> -StorageAccountId <String> -Enabled <Boolean>
 [-Categories <System.Collections.Generic.List`1[System.String]>]
 [-Timegrains <System.Collections.Generic.List`1[System.String]>] [-RetentionEnabled <Boolean>]
 [-RetentionInDays <Int32>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmDiagnosticSetting** cmdlet enables or disables each time grain and log category for the particular resource.

The logs and metrics are stored in the specified storage account.

## EXAMPLES

### Example 1: Enable all metrics and logs for a resource
```
PS C:\>Set-AzureRmDiagnosticSetting -ResourceId "Resource01" -Enabled $True
```

This command enables all available metrics and logs for Resource01.

### Example 2: Disable all metrics and logs
```
PS C:\>Set-AzureRmDiagnosticSetting -ResourceId "Resource01" -Enabled $False
```

This command disables all available metrics and logs for the resource Resource01.

### Example 3: Enable multiple categories
```
PS C:\>Set-AzureRmDiagnosticSetting -ResourceId "Resource01" -Enabled $True -Categories Category1,Category2
StorageAccountId   : <storageAccountId>
StorageAccountName : <storageAccountName>
Metrics
Enabled   : True
Timegrain : PT1M
Enabled   : True
Timegrain : PT1H
Logs
Enabled  : True
Category : Category1
Enabled  : True
Category : Category2
Enabled  : True
Category : Category3
Enabled  : False
Category : Category4
```

This command enables Category1 and Category2.
All timegrains and other categories remain the same.

### Example 4: Enable a time grain and multiple categories
```
PS C:\>Set-AzureRmDiagnosticSetting -ResourceId "Resource01" -Enabled $True -Categories Category1,Category2 -Timegrains PT1M
```

This command enables only Category1, Category2, and time grain PT1M.
All other time grains and categories are unchanged.

## PARAMETERS

### -ResourceId
Specifies the ID of the resource.

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

### -StorageAccountId
Specifies the ID of the Storage account in which to save the data.

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

### -Enabled
Indicates whether to enable diagnostics.
Specify $True to enable diagnostics, or $False to disable diagnostics.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Categories
Specifies the list of log categories to enable or disable, according to the value of *Enabled*.
If you do not specify a category, this command operates on all categories.

```yaml
Type: System.Collections.Generic.List`1[System.String]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Timegrains
Specifies the time grains to enable or disable for metrics, according to the value of *Enabled*.
If you do not specify a time grain, this command operates on all available time grains.

```yaml
Type: System.Collections.Generic.List`1[System.String]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -RetentionEnabled
Indicates whether retention of diagnostic information is enabled.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -RetentionInDays
Specifies the retention policy, in days.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InformationAction
@{Text=}```yaml
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
@{Text=}```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

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

[Get-AzureRmDiagnosticSetting](.\Get-AzureRmDiagnosticSetting.md)

