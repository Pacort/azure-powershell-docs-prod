---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 6DD8D854-912D-4281-977C-FF3EC15CCF51
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v1.6.1/Add-AzurePHPWebRole.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v1.6.1/Add-AzurePHPWebRole.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v1.6.1/Add-AzurePHPWebRole.md
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

# Add-AzurePHPWebRole

## SYNOPSIS
Creates the required files and configuration (sometimes referred to as scaffolding) for a PHP application.

## SYNTAX

```
Add-AzurePHPWebRole [[-Name] <String>] [[-Instances] <Int32>] [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
powershell_prelim

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
Position: 1
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
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
In-memory profile.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AzurePHPWorkerRole](xref:ServiceManagement/Azure.Compute/v1.6.1/Add-AzurePHPWorkerRole.md)

[New-AzureServiceProject](xref:ServiceManagement/Azure.Compute/v1.6.1/New-AzureServiceProject.md)


