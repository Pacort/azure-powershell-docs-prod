---
external help file: Microsoft.Azure.Commands.StreamAnalytics.dll-Help.xml
ms.assetid: 5DA67B35-AA16-426E-BC1A-9F5FAD3B7461
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.StreamAnalytics/v2.3.0/Test-AzureRmStreamAnalyticsFunction.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.StreamAnalytics/v2.3.0/Test-AzureRmStreamAnalyticsFunction.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Test-AzureRmStreamAnalyticsFunction

## SYNOPSIS
Tests whether Stream Analytics can connect to a function.

## SYNTAX

```
Test-AzureRmStreamAnalyticsFunction [-JobName] <String> [-Name] <String> [-ResourceGroupName] <String>
 [<CommonParameters>]
```

## DESCRIPTION
The **Test-AzureRmStreamAnalyticsFunction** cmdlet tests whether Azure Stream Analytics can connect to a function.

## EXAMPLES

### Example 1: Test a Stream Analytics function
```
PS C:\>Test-AzureRmStreamAnalyticsFunction -ResourceGroupName "StreamAnalytics-Default-West-US" -JobName "StreamJob22" -Name "ScoreTweet"
```

This command tests the connection status of the function named ScoreTweet in the job named StreamJob22.

## PARAMETERS

### -JobName
Specifies the name of the Stream Analytics job to which a function belongs.

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
Specifies the name of the Stream Analytics function that this cmdlet tests.

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

### -ResourceGroupName
Specifies the name of the resource group to which a Stream Analytics function belongs.
This cmdlet tests a function in the resource group that this parameter specifies.

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

### System.Object

## NOTES

## RELATED LINKS

[Get-AzureRmStreamAnalyticsFunction](xref:ResourceManager/AzureRM.StreamAnalytics/v2.3.0/Get-AzureRmStreamAnalyticsFunction.md)

[New-AzureRmStreamAnalyticsFunction](xref:ResourceManager/AzureRM.StreamAnalytics/v2.3.0/New-AzureRmStreamAnalyticsFunction.md)

[Remove-AzureRmStreamAnalyticsFunction](xref:ResourceManager/AzureRM.StreamAnalytics/v2.3.0/Remove-AzureRmStreamAnalyticsFunction.md)

