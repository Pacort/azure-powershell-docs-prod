---
external help file: Microsoft.Azure.Commands.SiteRecovery.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 200ECD6F-5A5E-499A-8EA9-F747197EBF03
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v1.1.11/Edit-AzureRmSiteRecoveryRecoveryPlan.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v1.1.11/Edit-AzureRmSiteRecoveryRecoveryPlan.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v1.1.11/Edit-AzureRmSiteRecoveryRecoveryPlan.md
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

# Edit-AzureRmSiteRecoveryRecoveryPlan

## SYNOPSIS
Edits a Site Recovery plan.

## SYNTAX

### AppendGroup (Default)
```
Edit-AzureRmSiteRecoveryRecoveryPlan -RecoveryPlan <ASRRecoveryPlan> [-AppendGroup] [<CommonParameters>]
```

### RemoveGroup
```
Edit-AzureRmSiteRecoveryRecoveryPlan -RecoveryPlan <ASRRecoveryPlan> -RemoveGroup <ASRRecoveryPlanGroup>
 [<CommonParameters>]
```

### AddProtectedEntities
```
Edit-AzureRmSiteRecoveryRecoveryPlan -RecoveryPlan <ASRRecoveryPlan> -Group <ASRRecoveryPlanGroup>
 -AddProtectedEntities <ASRProtectionEntity[]> [<CommonParameters>]
```

### RemoveProtectedEntities
```
Edit-AzureRmSiteRecoveryRecoveryPlan -RecoveryPlan <ASRRecoveryPlan> -Group <ASRRecoveryPlanGroup>
 -RemoveProtectedEntities <ASRProtectionEntity[]> [<CommonParameters>]
```

## DESCRIPTION
The **Edit-AzureRmSiteRecoveryRecoveryPlan** cmdlet edits an Azure Site Recovery plan.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -AddProtectedEntities
Specifies an array of protected entities to add.

```yaml
Type: ASRProtectionEntity[]
Parameter Sets: AddProtectedEntities
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppendGroup
Indicates that this operation appends the group to the recovery plan object.

```yaml
Type: SwitchParameter
Parameter Sets: AppendGroup
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Group
Specifies a Site Recovery plan group.

```yaml
Type: ASRRecoveryPlanGroup
Parameter Sets: AddProtectedEntities, RemoveProtectedEntities
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RecoveryPlan
Specifies a recovery plan.

```yaml
Type: ASRRecoveryPlan
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -RemoveGroup
Removes the specified Site Recovery recovery plan group.

```yaml
Type: ASRRecoveryPlanGroup
Parameter Sets: RemoveGroup
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemoveProtectedEntities
Specifies an array of protected entities.

```yaml
Type: ASRProtectionEntity[]
Parameter Sets: RemoveProtectedEntities
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

[Get-AzureRmSiteRecoveryRecoveryPlan](xref:ResourceManager/AzureRM.SiteRecovery/v1.1.11/Get-AzureRmSiteRecoveryRecoveryPlan.md)

[New-AzureRmSiteRecoveryRecoveryPlan](xref:ResourceManager/AzureRM.SiteRecovery/v1.1.11/New-AzureRmSiteRecoveryRecoveryPlan.md)


