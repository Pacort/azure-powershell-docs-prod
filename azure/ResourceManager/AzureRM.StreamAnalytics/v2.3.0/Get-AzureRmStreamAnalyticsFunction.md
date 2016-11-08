---
external help file: Microsoft.Azure.Commands.StreamAnalytics.dll-Help.xml
ms.assetid: 87E95D58-00AA-4A5A-9527-94CA53522A64
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.StreamAnalytics/v2.3.0/Get-AzureRmStreamAnalyticsFunction.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.StreamAnalytics/v2.3.0/Get-AzureRmStreamAnalyticsFunction.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmStreamAnalyticsFunction

## SYNOPSIS
Gets functions in a Stream Analytics job.

## SYNTAX

```
Get-AzureRmStreamAnalyticsFunction [-JobName] <String> [[-Name] <String>] [-ResourceGroupName] <String>
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmStreamAnalyticsFunction** cmdlet gets a list of the functions that are defined in an Azure Stream Analytics job or information about a specific function.

## EXAMPLES

### Example 1: Get all Stream Analytics functions
```
PS C:\>Get-AzureRmStreamAnalyticsFunction -ResourceGroupName "StreamAnalytics-Default-West-US" -JobName "StreamJob22"
```

This command gets the functions defined on the job named StreamJob22.

### Example 2: Get a specific Stream Analytics function
```
PS C:\>Get-AzureRmStreamAnalyticsFunction -ResourceGroupName "StreamAnalytics-Default-West-US" -JobName "StreamJob22" -Name "ScoreTweet"
```

This command gets information about the function named ScoreTweet defined on the job named StreamJob22.

## PARAMETERS

### -JobName
Specifies the name of the Stream Analytics job to which functions belong.
This cmdlet gets functions for the job that this parameter specifies.

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

### -Name
Specifies the name of the Stream Analytics function that this cmdlet gets.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group to which Stream Analytics functions belongs.
This cmdlet gets functions for the group that this parameter specifies.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### System.Collections.Generic.List[Microsoft.Azure.Commands.StreamAnalytics.Models.PSFunction, Microsoft.Azure.Commands.StreamAnalytics], Microsoft.Azure.Commands.StreamAnalytics.Models.PSFunction

## NOTES

## RELATED LINKS

[New-AzureRmStreamAnalyticsFunction](xref:ResourceManager/AzureRM.StreamAnalytics/v2.3.0/New-AzureRmStreamAnalyticsFunction.md)

[Remove-AzureRmStreamAnalyticsFunction](xref:ResourceManager/AzureRM.StreamAnalytics/v2.3.0/Remove-AzureRmStreamAnalyticsFunction.md)

[Test-AzureRmStreamAnalyticsFunction](xref:ResourceManager/AzureRM.StreamAnalytics/v2.3.0/Test-AzureRmStreamAnalyticsFunction.md)

