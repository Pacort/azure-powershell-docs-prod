---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
ms.assetid: 16272B69-5537-4F1F-B1C7-36C192273CF3
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.1.0/Add-AzurePHPWebRole.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.1.0/Add-AzurePHPWebRole.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Add-AzurePHPWebRole

## SYNOPSIS
Creates the required files and configuration (sometimes referred to as scaffolding) for a PHP application.

## SYNTAX

```
Add-AzurePHPWebRole [[-Name] <String>] [[-Instances] <Int32>] [-Profile <AzureSMProfile>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
This topic describes the cmdlet in the 0.8.10 version of the Microsoft Azure PowerShell module.
To get the version of the module you're using, in the Azure PowerShell console, type (Get-Module -Name Azure).Version.

The **Add-AzurePHPWebRole** cmdlet creates the files and configuration (sometimes referred to as scaffolding) for a PHP application that will be hosted in Azure through IIS.

## EXAMPLES

### 1: Add a web role using default values
```
PS C:\>Add-AzurePHPWebRole
```

This example adds the required files and configuration for new web role using the default values of a service named "WebRole1" with 1 instance.

### 2: Add a web role with multiple instances
```
PS C:\>Add-AzurePHPWebRole MyWebRole -I 2
```

This example adds the required files and configuration for a new web role to the current application, using the name "MyWebRole" and a role instance count of 2.

## PARAMETERS

### -Name
Specifies the name of the web role.
The name determines the name of the directory that contains the required files and configuration for the PHP application.
The default is WebRole#, where # is the number of web roles in the service.

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
Specifies the number of role instances for this web role.
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

[Add-AzurePHPWorkerRole](xref:ServiceManagement/Azure.Compute/v3.1.0/Add-AzurePHPWorkerRole.md)

[New-AzureServiceProject](xref:ServiceManagement/Azure.Compute/v3.1.0/New-AzureServiceProject.md)

