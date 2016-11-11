---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
ms.assetid: 23FBBEBC-1EC5-4D15-A14C-E267B2AC1ED7
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.1.0/Add-AzurePHPWorkerRole.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.1.0/Add-AzurePHPWorkerRole.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Add-AzurePHPWorkerRole

## SYNOPSIS
Creates the required files and configuration (sometimes referred to as scaffolding) for a PHP application that will be hosted in Azure through php.exe.

## SYNTAX

```
Add-AzurePHPWorkerRole [[-Name] <String>] [[-Instances] <Int32>] [-Profile <AzureSMProfile>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
This topic describes the cmdlet in the 0.8.10 version of the Microsoft Azure PowerShell module.
To get the version of the module you're using, in the Azure PowerShell console, type (Get-Module -Name Azure).Version.

Creates the required files and configuration (sometimes referred to as scaffolding) for a PHP application that will be hosted in Azure through php.exe.

## EXAMPLES

### 1: Create a worker role with a single instance
```
PS C:\>Add-AzurePHPWorkerRole MyWorkerRole
```

This example adds the required files and configuration for a single worker role named MyWorkerRole to the current application.

### 2: Create a worker role with multiple instances
```
PS C:\>Add-AzurePHPWorkerRole MyWorkerRole -I 2
```

This example adds the required files and configuration for a new worker role to the current application, using the name MyWorkerRole with a role instance count of 2.

## PARAMETERS

### -Name
Specifies the name of the worker role.
The name determines the folder name that contains the required files and configuration for the PHP service hosted in the worker role.
The default is WorkerRole1.

```yaml
Type: String
Parameter Sets: (All)
Aliases: n

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Instances
Specifies the number of role instances for this worker role.
The default is 1.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: i

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

```yaml
Type: AzureSMProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
Specifies how this cmdlet responds to an information event.

The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Specifies an information variable.

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
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

[New-AzureServiceProject](xref:ServiceManagement/Azure.Compute/v3.1.0/New-AzureServiceProject.md)

[Add-AzurePHPWebRole](xref:ServiceManagement/Azure.Compute/v3.1.0/Add-AzurePHPWebRole.md)

