---
external help file: Microsoft.Azure.Commands.MachineLearning.dll-Help.xml
ms.assetid: BD8515DB-085F-499E-8BDE-77F76F0A0B42
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.MachineLearning/v0.11.1/Get-AzureRmMlCommitmentPlan.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.MachineLearning/v0.11.1/Get-AzureRmMlCommitmentPlan.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmMlCommitmentPlan

## SYNOPSIS
Retrieves the summary information for one or more commitment plans.

## SYNTAX

```
Get-AzureRmMlCommitmentPlan [-ResourceGroupName <String>] [-Name <String>]
```

## DESCRIPTION
Retrieves commitment plan information.
Depending on the paramenters passed, the cmdlet returns the a specific commitment plan, a collection of commitment plans for a specified resource group within the current subscription, or a collection of commitment plans within the current subscription.

## EXAMPLES

### --------------------------  Example 1: Get a specific commitment plan  --------------------------
```
Get-AzureRmMlCommitmentPlan -ResourceGroupName "MyResourceGroup" -Name "MyCommitmentPlanName"
```

### --------------------------  Example 2: Get all commitment plan resources in current subscription  --------------------------
```
Get-AzureRmMlCommitmentPlan
```

### --------------------------  Example 3: Get all commitment plans in the current subscription and given resource group  --------------------------
```
Get-AzureRmMlCommitmentPlan -ResourceGroupName "MyResourceGroup"
```

## PARAMETERS

### -Name
The name of the commitment plan.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
The name of the resource group for the Azure ML commitment plan.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

### Microsoft.Azure.Management.MachineLearning.CommitmentPlans.Models.CommitmentPlan
Microsoft.Azure.Management.MachineLearning.CommitmentPlans.Models.CommitmentPlan\[\]

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, machine, machine learning, azureml

## RELATED LINKS
