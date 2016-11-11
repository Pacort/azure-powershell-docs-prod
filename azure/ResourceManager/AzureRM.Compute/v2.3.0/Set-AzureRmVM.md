---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
ms.assetid: 62DACBC2-D64B-4A0C-8440-9A5D74F51D3A
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.3.0/Set-AzureRmVM.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.3.0/Set-AzureRmVM.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureRmVM

## SYNOPSIS
Marks a virtual machine as generalized.

## SYNTAX

### GeneralizeResourceGroupNameParameterSetName (Default)
```
Set-AzureRmVM [-ResourceGroupName] <String> [-Name] <String> [-Generalized] [<CommonParameters>]
```

### RedeployResourceGroupNameParameterSetName
```
Set-AzureRmVM [-ResourceGroupName] <String> [-Name] <String> [-Redeploy] [<CommonParameters>]
```

### RedeployIdParameterSetName
```
Set-AzureRmVM [-Id] <String> [-Name] <String> [-Redeploy] [<CommonParameters>]
```

### GeneralizeIdParameterSetName
```
Set-AzureRmVM [-Id] <String> [-Name] <String> [-Generalized] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmVM** cmdlet marks a virtual machine as generalized.
Before you run this cmdlet, log on to the virtual machine and use Sysprep to prepare the hard disk.

## EXAMPLES

### Example 1: Mark a virtual machine as generalized
```
PS C:\>Set-AzureRmVM -ResourceGroupName "ResourceGroup11" -Name "VirtualMachine07" -Generalized
```

This command marks the virtual machine named VirtualMachine07 as generalized.

## PARAMETERS

### -Generalized
Indicates that this cmdlet marks a virtual machine as generalized.

```yaml
Type: SwitchParameter
Parameter Sets: GeneralizeResourceGroupNameParameterSetName, GeneralizeIdParameterSetName
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Id
Specifies the Resource ID of the virtual machine.

```yaml
Type: String
Parameter Sets: RedeployIdParameterSetName, GeneralizeIdParameterSetName
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the virtual machine on which this cmdlet operates.

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

### -Redeploy
Indicates that this cmdlet manually redeploys the virtual machine to a different Azure host to fix any problems.

If you redeploy a virtual machine, it restarts, which results in the loss of ephemeral drive data.

```yaml
Type: SwitchParameter
Parameter Sets: RedeployResourceGroupNameParameterSetName, RedeployIdParameterSetName
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group of the virtual machine.

```yaml
Type: String
Parameter Sets: GeneralizeResourceGroupNameParameterSetName, RedeployResourceGroupNameParameterSetName
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

[Get-AzureRmVM](xref:ResourceManager/AzureRM.Compute/v2.3.0/Get-AzureRmVM.md)

