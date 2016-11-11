---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
ms.assetid: D094E0FD-63B7-44B4-943D-0CAE23A75E61
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.1.0/Get-AzureSchedulerJobCollection.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.1.0/Get-AzureSchedulerJobCollection.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureSchedulerJobCollection

## SYNOPSIS
Gets scheduler job collections.

## SYNTAX

```
Get-AzureSchedulerJobCollection [[-Location] <String>] [[-JobCollectionName] <String>]
 [-Profile <AzureSMProfile>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
This topic describes the cmdlet in the 0.8.10 version of the Microsoft Azure PowerShell module.
To get the version of the module you're using, in the Azure PowerShell console, type (Get-Module -Name Azure).Version.

The **Get-AzureSchedulerJobCollection** cmdlet gets one or more scheduler job collections.

## EXAMPLES

### Example 1: Get all collections
```
PS C:\>Get-AzureSchedulerJobCollection
```

This command gets all scheduler job collections across all locations in the current subscription.

### Example 2: Get all collections for a location
```
PS C:\>Get-AzureSchedulerJobCollection -Location "North Central US"
```

This command gets all scheduler job collections in the location named North Central US.

### Example 3: Get a collection by using a name
```
PS C:\>Get-AzureSchedulerJobCollection -Location "North Central US" -JobCollectionName "JobCollection01"
```

This command gets the scheduler job collection named JobCollection01.

## PARAMETERS

### -Location
Specifies the name of the location that hosts the cloud service.
Valid values are: 

- Anywhere Asia
- Anywhere Europe
- Anywhere US
- East Asia
- East US
- North Central US
- North Europe
- South Central US
- Southeast Asia
- West Europe
- West US

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JobCollectionName
Specifies the name of the scheduler job collection to get.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
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

[New-AzureSchedulerJobCollection](xref:ServiceManagement/Azure.Compute/v3.1.0/New-AzureSchedulerJobCollection.md)

[Remove-AzureSchedulerJobCollection](xref:ServiceManagement/Azure.Compute/v3.1.0/Remove-AzureSchedulerJobCollection.md)

[Set-AzureSchedulerJobCollection](xref:ServiceManagement/Azure.Compute/v3.1.0/Set-AzureSchedulerJobCollection.md)

