---
external help file: Microsoft.Azure.Commands.ResourceManager.Automation.dll-Help.xml
ms.assetid: 1B580598-1087-4A10-9BC3-747EC5D7604A
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v2.3.0/Stop-AzureRMAutomationJob.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v2.3.0/Stop-AzureRMAutomationJob.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Stop-AzureRmAutomationJob

## SYNOPSIS
Stops an Automation job.

## SYNTAX

```
Stop-AzureRmAutomationJob [-Id] <Guid> [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [<CommonParameters>]
```

## DESCRIPTION
The **Stop-AzureRmAutomationJob** cmdlet stops an Azure Automation job.
Specify a running Automation job.

## EXAMPLES

### Example 1: Stop a job
```
PS C:\>Stop-AzureRmAutomationJob -AutomationAccountName "Contoso17" -Id 2989b069-24fe-40b9-b3bd-cb7e5eac4b64 -ResourceGroupName "ResourceGroup01"
```

This command stops the job that has the specified ID.

## PARAMETERS

### -AutomationAccountName
Specifies the name of an Automation account in which this cmdlet stops a job.

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

### -Id
Specifies the ID of a job that this cmdlet stops.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: JobId

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of a resource group.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmAutomationJob](xref:ResourceManager/AzureRM.Automation/v2.3.0/Get-AzureRMAutomationJob.md)

[Get-AzureRmAutomationJobOutput](xref:ResourceManager/AzureRM.Automation/v2.3.0/Get-AzureRMAutomationJobOutput.md)

[Resume-AzureRmAutomationJob](xref:ResourceManager/AzureRM.Automation/v2.3.0/Resume-AzureRMAutomationJob.md)

[Suspend-AzureRmAutomationJob](xref:ResourceManager/AzureRM.Automation/v2.3.0/Suspend-AzureRMAutomationJob.md)

