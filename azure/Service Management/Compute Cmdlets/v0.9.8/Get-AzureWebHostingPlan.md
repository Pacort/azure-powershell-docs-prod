---
external help file: SMAzure_Compute.xml
online version: 
schema: 2.0.0
updated_at: 8/26/2016 9:24 PM
ms.date: 8/26/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/Service%20Management/Compute%20Cmdlets/v0.9.8/Get-AzureWebHostingPlan.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/1457b00e4be43f52e047ac6fd4ed87f3565c5548/azureps-cmdlets-docs/Service%20Management/Compute%20Cmdlets/v0.9.8/Get-AzureWebHostingPlan.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureWebHostingPlan
## SYNOPSIS
Gets Azure web hosting plans in the current subscription.

## SYNTAX

```
Get-AzureWebHostingPlan [[-WebSpaceName] <String>] [[-Name] <String>]
```

## DESCRIPTION
This topic describes the cmdlet in the 0.8.10 version of the Microsoft Azure PowerShell module.
To get the version of the module you're using, in the Azure PowerShell console, type (Get-Module -Name Azure).Version.

The Get-AzureWebHostingPlan cmdlet gets the Azure web hosting plans in the current subscription.

By default, Get-AzureWebHostingPlan gets all Azure hosting plans in the current subscription and returns an object that provides basic information about the plans.
When you use the WebSpace and Name parameters, Get-AzureWebHostingPlan returns a specific hosting plan object.

To find the current subscription, use the Current parameter of the Get-AzureSubscription cmdlet.
To change the current subscription, use the Select-AzureSubscription cmdlet.

## EXAMPLES

### Example 1: Get all web hosting plans in a subscription
```
PS C:\>Get-AzureWebHostingPlan 
Name : Default1 
SKU : Basic 
WorkerSize : Small 
NumberOfWorkers : 1 
CurrentWorkerSize : Small 
CurrentNumberOfWorkers : 1 
Status : Ready 
WebSpace : eastuswebspace 
Name : Default0 
SKU : Free 
WorkerSize : Small 
NumberOfWorkers : 0 
CurrentWorkerSize : Small 
CurrentNumberOfWorkers : 0 
Status : Ready
```

This command gets all Azure web hosting plans in the current subscription.

### Example 2: Get a specific web hosting plan in a subscription
```
PS C:\>Get-AzureWebHostingPlan -WebSpaceName "westeuropewebspace" -Name "Default0" 
Name : Default0 
SKU : Free 
WorkerSize : Small 
NumberOfWorkers : 0 
CurrentWorkerSize : Small 
CurrentNumberOfWorkers : 0 
Status : Ready 
WebSpace : westeuropewebspace
```

This command gets the web hosting plan named Default0 in the webspace named westeuropewebspace in the current subscription.

## PARAMETERS

### -Name
Specifies the name of a plan in the subscription.
By default, this cmdlet gets all plans in the current subscription.
This parameter does not support wildcard characters.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -WebSpaceName
Specifies the name of a webspace in the subscription.
By default, this cmdlet gets all websites in the specified webspace.
This parameter does not support wildcard characters.

```yaml
Type: String
Parameter Sets: (All)
Aliases: WebSpace

Required: False
Position: 1
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

### 
You can pass input to this cmdlet by property name, but not by value.

## OUTPUTS

### Microsoft.WindowsAzure.Commands.Utilities.Websites.Services.WebEntities.WebHostingPlan
By default, Get-AzureWebHostingPlan returns an array of WebHostingPlan objects.

## NOTES

## RELATED LINKS
