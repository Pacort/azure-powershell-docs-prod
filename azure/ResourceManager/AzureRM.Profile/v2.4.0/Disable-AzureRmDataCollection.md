---
external help file: Microsoft.Azure.Commands.Profile.dll-Help.xml
ms.assetid: 44832B1D-42B7-4492-827B-05D792C692C5
online version: 
schema: 2.0.0
updated_at: 1/11/2017 9:26 PM
ms.date: 1/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Profile/v2.4.0/Disable-AzureRmDataCollection.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Profile/v2.4.0/Disable-AzureRmDataCollection.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/cf5fb15dcd1fe2c86458f47e1a11dc88817021fc/azureps-cmdlets-docs/ResourceManager/AzureRM.Profile/v2.4.0/Disable-AzureRmDataCollection.md
ms.topic: reference
ms.prod: powershell
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: False
ms.service: azure-powershell
---

# Disable-AzureRmDataCollection

## SYNOPSIS
Disables collection of data to improve user experience.

## SYNTAX

```
Disable-AzureRmDataCollection [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Disable-AzureRmDataCollection** cmdlet disables collection of data to improve the user experience with Azure PowerShell cmdlets.

Azure PowerShell does not collect data unless you explicitly opt in, either by using the Enable-AzureRmDataCollection cmdlet or when Azure PowerShell prompts you about collecting data the first time that you run a cmdlet.

If you run the current cmdlet before you run any Azure PowerShell cmdlets, Azure PowerShell does not prompt you about data collection the first time that you run a cmdlet.

To enable data collection for the current user, run **Enable-AzureRmDataCollection**.

## EXAMPLES

### Example 1: Disable data collection
```
PS C:\>Disable-AzureRmDataCollection
```

This command disables data collection for the current user on the current computer.

## PARAMETERS

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
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Enable-AzureRmDataCollection](xref:ResourceManager/AzureRM.Profile/v2.4.0/Enable-AzureRmDataCollection.md)


