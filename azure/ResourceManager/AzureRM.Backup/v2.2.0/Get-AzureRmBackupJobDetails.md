---
external help file: Microsoft.Azure.Commands.AzureBackup.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 5BD87FC6-16E2-41A5-A923-3251764CFDF5
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Backup/v2.2.0/Get-AzureRmBackupJobDetails.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Backup/v2.2.0/Get-AzureRmBackupJobDetails.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ResourceManager/AzureRM.Backup/v2.2.0/Get-AzureRmBackupJobDetails.md
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

# Get-AzureRmBackupJobDetails

## SYNOPSIS
Gets the details of a Backup job.

## SYNTAX

### JobsFiltersSet (Default)
```
Get-AzureRmBackupJobDetails -Job <AzureRMBackupJob> [<CommonParameters>]
```

### IdFiltersSet
```
Get-AzureRmBackupJobDetails -Vault <AzureRMBackupVault> -JobId <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmBackupJobDetails** cmdlet gets the details of an Azure Backup job.
You can use this cmdlet to gather information about a job that fails.

## EXAMPLES

### Example 1: Display the details of a failed job
```
PS C:\>$Vault = Get-AzureRmBackupVault -Name "Vault03" 
PS C:\> $Jobs = Get-AzureRmBackupJob -Vault $Vault -Status Failed
PS C:\> $JobDetails = Get-AzureRmBackupJobDetails -Job $Jobs[0]
PS C:\> $JobDetails.ErrorDetails
ErrorCode ErrorMessage                            Recommendations
--------- ------------                            ---------------
   400001 Command execution failed.               {Another operation is currently in p...
```

The first command gets the vault named Vault03 by using the **Get-AzureRmBackupVault** cmdlet.
The command stores that object in the $Vault variable.

The second command gets failed jobs from the vault in $Vault, and then stores them in the $Jobs array variable.

The third job gets details for the first job in the $Jobs variable, and then stores those details in the $JobDetails variable.

The final command displays the **ErrorDetails** property of $JobDetails by using standard dot syntax.

### Example 2: Display the recommended action for a failed job
```
PS C:\>$JobDetails.ErrorDetails.Recommendations
Another operation is currently in progress on this item. Please wait until the previous operation is completed, and then retry.
```

This command displays the recommended action from the $JobDetails variable that was created in the first example.

## PARAMETERS

### -Job
Specifies a job for which this cmdlet gets details.
To obtain an **AzureRmBackupJob** object, use the Get-AzureRmBackupJob cmdlet.

```yaml
Type: AzureRMBackupJob
Parameter Sets: JobsFiltersSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -JobId
Specifies the ID of a job for which this cmdlet gets details.
The ID is the **InstanceId** property of an **AzureRmBackupJob** object.
To obtain an **AzureRmBackupJob** object, use Get-AzureRmBackupJob.

```yaml
Type: String
Parameter Sets: IdFiltersSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Vault
Specifies the Backup vault for which this cmdlet gets job details.
To obtain an **AzureRmBackupVault** object, use the Get-AzureRmBackupVault cmdlet.

```yaml
Type: AzureRMBackupVault
Parameter Sets: IdFiltersSet
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

### None

## OUTPUTS

### AzureRmBackupJobDetails

## NOTES
* None

## RELATED LINKS

[Get-AzureRmBackupJob](xref:ResourceManager/AzureRM.Backup/v2.2.0/Get-AzureRmBackupJob.md)

[Get-AzureRmBackupVault](xref:ResourceManager/AzureRM.Backup/v2.2.0/Get-AzureRmBackupVault.md)


