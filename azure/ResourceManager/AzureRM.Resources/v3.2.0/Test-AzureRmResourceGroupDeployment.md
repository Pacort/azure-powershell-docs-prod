---
external help file: Microsoft.Azure.Commands.ResourceManager.Cmdlets.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 314249CB-3C2C-4016-BD7C-5EE7034774E2
updated_at: 1/9/2017 9:52 PM
ms.date: 1/9/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.2.0/Test-AzureRmResourceGroupDeployment.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.2.0/Test-AzureRmResourceGroupDeployment.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4f60f66b5229674cbde5c80b99ac704ad8318378/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.2.0/Test-AzureRmResourceGroupDeployment.md
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

# Test-AzureRmResourceGroupDeployment

## SYNOPSIS
Validates a resource group deployment.

## SYNTAX

### Deployment via template file without parameters (Default)
```
Test-AzureRmResourceGroupDeployment -ResourceGroupName <String> [-Mode <DeploymentMode>] -TemplateFile <String>
 [-ApiVersion <String>] [-Pre] [<CommonParameters>]
```

### Deployment via template file and template parameters object
```
Test-AzureRmResourceGroupDeployment -ResourceGroupName <String> [-Mode <DeploymentMode>]
 -TemplateParameterObject <Hashtable> -TemplateFile <String> [-ApiVersion <String>] [-Pre] [<CommonParameters>]
```

### Deployment via template uri and template parameters object
```
Test-AzureRmResourceGroupDeployment -ResourceGroupName <String> [-Mode <DeploymentMode>]
 -TemplateParameterObject <Hashtable> -TemplateUri <String> [-ApiVersion <String>] [-Pre] [<CommonParameters>]
```

### Deployment via template uri and template parameters file
```
Test-AzureRmResourceGroupDeployment -ResourceGroupName <String> [-Mode <DeploymentMode>]
 -TemplateParameterFile <String> -TemplateUri <String> [-ApiVersion <String>] [-Pre] [<CommonParameters>]
```

### Deployment via template file and template parameters file
```
Test-AzureRmResourceGroupDeployment -ResourceGroupName <String> [-Mode <DeploymentMode>]
 -TemplateParameterFile <String> -TemplateFile <String> [-ApiVersion <String>] [-Pre] [<CommonParameters>]
```

### Deployment via template file template parameters uri
```
Test-AzureRmResourceGroupDeployment -ResourceGroupName <String> [-Mode <DeploymentMode>]
 -TemplateParameterUri <String> -TemplateFile <String> [-ApiVersion <String>] [-Pre] [<CommonParameters>]
```

### Deployment via template uri and template parameters uri
```
Test-AzureRmResourceGroupDeployment -ResourceGroupName <String> [-Mode <DeploymentMode>]
 -TemplateParameterUri <String> -TemplateUri <String> [-ApiVersion <String>] [-Pre] [<CommonParameters>]
```

### Deployment via template uri without parameters
```
Test-AzureRmResourceGroupDeployment -ResourceGroupName <String> [-Mode <DeploymentMode>] -TemplateUri <String>
 [-ApiVersion <String>] [-Pre] [<CommonParameters>]
```

## DESCRIPTION
The **Test-AzureRmResourceGroupDeployment** cmdlet determines whether an Azure resource group deployment template and its parameter values are valid.

## EXAMPLES


## PARAMETERS

### -ResourceGroupName
Specifies the name of the resource group to test.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TemplateFile
Specifies the full path of a JSON template file.

```yaml
Type: String
Parameter Sets: Deployment via template file without parameters, Deployment via template file and template parameters object, Deployment via template file and template parameters file, Deployment via template file template parameters uri
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TemplateParameterObject
Specifies a hash table of template parameter names and values.

```yaml
Type: Hashtable
Parameter Sets: Deployment via template file and template parameters object, Deployment via template uri and template parameters object
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TemplateUri
Specifies the URI of a JSON template file.

```yaml
Type: String
Parameter Sets: Deployment via template uri and template parameters object, Deployment via template uri and template parameters file, Deployment via template uri and template parameters uri, Deployment via template uri without parameters
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TemplateParameterFile
Specifies the full path of a JSON file that contains the names and values of the template parameters.

```yaml
Type: String
Parameter Sets: Deployment via template uri and template parameters file, Deployment via template file and template parameters file
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ApiVersion
Specifies the API version that is supported by the resource Provider.
You can specify a different version than the default version.

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

### -Mode
Specifies the deployment mode.
The acceptable values for this parameter are:

- Incremental
- Complete

```yaml
Type: DeploymentMode
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Pre
Indicates that this cmdlet considers pre-release API versions when it automatically determines which version to use.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TemplateParameterUri
Specifies the URI of a template parameters file.

```yaml
Type: String
Parameter Sets: Deployment via template file template parameters uri, Deployment via template uri and template parameters uri
Aliases: 

Required: True
Position: Named
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

[Get-AzureRmResourceGroupDeployment](xref:ResourceManager/AzureRM.Resources/v3.2.0/Get-AzureRmResourceGroupDeployment.md)

[New-AzureRmResourceGroupDeployment](xref:ResourceManager/AzureRM.Resources/v3.2.0/New-AzureRmResourceGroupDeployment.md)

[Remove-AzureRmResourceGroupDeployment](xref:ResourceManager/AzureRM.Resources/v3.2.0/Remove-AzureRmResourceGroupDeployment.md)

[Stop-AzureRmResourceGroupDeployment](xref:ResourceManager/AzureRM.Resources/v3.2.0/Stop-AzureRmResourceGroupDeployment.md)


