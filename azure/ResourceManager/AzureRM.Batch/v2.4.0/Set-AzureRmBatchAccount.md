---
external help file: Microsoft.Azure.Commands.Batch.dll-Help.xml
ms.assetid: 9BEE5888-304D-4438-BE97-D1FE254AEE98
online version: 
schema: 2.0.0
updated_at: 1/11/2017 9:26 PM
ms.date: 1/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v2.4.0/Set-AzureRmBatchAccount.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v2.4.0/Set-AzureRmBatchAccount.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/cf5fb15dcd1fe2c86458f47e1a11dc88817021fc/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v2.4.0/Set-AzureRmBatchAccount.md
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

# Set-AzureRmBatchAccount

## SYNOPSIS
Updates a Batch account.

## SYNTAX

```
Set-AzureRmBatchAccount [-AccountName] <String> [-Tag] <Hashtable> [-ResourceGroupName <String>]
 [-AutoStorageAccountId <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmBatchAccount** cmdlet updates an Azure Batch account.
Currently, this cmdlet can update only tags.

## EXAMPLES

### Example 1: Update the tags on a Batch account
```
PS C:\>Set-AzureRmBatchAccount -AccountName "cmdletexample" -Tag @(@{Name = "tag1";Value = "value1"},@{Name = "tag2";Value = "value2"})
AccountName                  : cmdletexample

Location                     : westus

ResourceGroupName            : CmdletExampleRG

CoreQuota                    : 20

PoolQuota                    : 20

ActiveJobAndJobScheduleQuota : 20

Tags                         : 

                               Name  Value

                               ====  ======

                               tag1  value1

                               tag2  value2

TaskTenantUrl                : https://cmdletexample.westus.batch.azure.com
```

This command updates the tags on the account named pfuller.

## PARAMETERS

### -AccountName
Specifies the name of the Batch account that this cmdlet updates.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Name

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -AutoStorageAccountId
Specifies the resource ID of the storage account to be used for auto storage.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the resource group of the account that this cmdlet updates.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Tag
Specifies an array of hash tables of tags for the account.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: Tags

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### BatchAccountContext

## NOTES

## RELATED LINKS

[Get-AzureRmBatchAccount](xref:ResourceManager/AzureRM.Batch/v2.4.0/Get-AzureRmBatchAccount.md)

[New-AzureRmBatchAccount](xref:ResourceManager/AzureRM.Batch/v2.4.0/New-AzureRmBatchAccount.md)

[Remove-AzureRmBatchAccount](xref:ResourceManager/AzureRM.Batch/v2.4.0/Remove-AzureRmBatchAccount.md)

[Azure Batch Cmdlets](xref:ResourceManager/AzureRM.Batch/v2.4.0/AzureRM.Batch.md)


