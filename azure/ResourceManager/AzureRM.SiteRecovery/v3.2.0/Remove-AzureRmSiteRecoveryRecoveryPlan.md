---
external help file: Microsoft.Azure.Commands.SiteRecovery.dll-Help.xml
ms.assetid: 6C332264-E27F-4B89-BE9A-61914F2365E0
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v3.2.0/Remove-AzureRmSiteRecoveryRecoveryPlan.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v3.2.0/Remove-AzureRmSiteRecoveryRecoveryPlan.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureRmSiteRecoveryRecoveryPlan

## SYNOPSIS
Removes a site recovery plan from Site Recovery.

## SYNTAX

### ByObject (Default)
```
Remove-AzureRmSiteRecoveryRecoveryPlan -RecoveryPlan <ASRRecoveryPlan> [<CommonParameters>]
```

### ByName
```
Remove-AzureRmSiteRecoveryRecoveryPlan -Name <String> [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmSiteRecoveryRecoveryPlan** cmdlet removes a site recovery plan from the current Azure Site Recovery.

## EXAMPLES

### Example 1: Remove a recovery plan
```
PS C:\>$RecoveryPlan = Get-AzureRmSiteRecoveryRecoveryPlan 
PS C:\> Remove-AzureRmSiteRecoveryRecoveryPlan -RecoveryPlan $RecoveryPlan
```

The first command uses the Get-AzureRmSiteRecoveryRecoveryPlan cmdlet to get the Site Recovery plan, and then stores it in the $RecoveryPlan variable.

The second command removes the recovery plan in $RecoveryPlan.

## PARAMETERS

### -RecoveryPlan
Specifies the recovery plan that this cmdlet removes.

```yaml
Type: ASRRecoveryPlan
Parameter Sets: ByObject
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
Specifies the name of the recovery plan that this cmdlet removes.

```yaml
Type: String
Parameter Sets: ByName
Aliases: 

Required: True
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

[Get-AzureRmSiteRecoveryRecoveryPlan](xref:ResourceManager/AzureRM.SiteRecovery/v3.2.0/Get-AzureRmSiteRecoveryRecoveryPlan.md)

[New-AzureRmSiteRecoveryRecoveryPlan](xref:ResourceManager/AzureRM.SiteRecovery/v3.2.0/New-AzureRmSiteRecoveryRecoveryPlan.md)

[Update-AzureRmSiteRecoveryRecoveryPlan](xref:ResourceManager/AzureRM.SiteRecovery/v3.2.0/Update-AzureRmSiteRecoveryRecoveryPlan.md)

