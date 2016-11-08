---
external help file: Microsoft.Azure.Commands.ResourceManager.Cmdlets.dll-Help.xml
ms.assetid: AD84B9EE-19BA-4E0F-8B96-0B0EA374885C
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.3.0/Find-AzureRmResource.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.3.0/Find-AzureRmResource.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Find-AzureRmResource

## SYNOPSIS
Searches for resources based on specified parameters.

## SYNTAX

### Lists the resources based on the specified scope. (Default)
```
Find-AzureRmResource [-ResourceNameContains <String>] [-ResourceType <String>]
 [-ExtensionResourceType <String>] [-Top <Int32>] [-ODataQuery <String>] [-TagName <String>]
 [-TagValue <String>] [-ResourceGroupNameContains <String>] [-ExpandProperties] [-ApiVersion <String>] [-Pre]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

### Lists the resources based on the specified scope at the tenant level.
```
Find-AzureRmResource [-ResourceNameContains <String>] -ResourceType <String> [-ExtensionResourceType <String>]
 [-Top <Int32>] [-ODataQuery <String>] [-ExpandProperties] [-TenantLevel] [-ApiVersion <String>] [-Pre]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

### Get a resources using a multi-subscription query.
```
Find-AzureRmResource [-ResourceNameContains <String>] -ResourceType <String> [-ExtensionResourceType <String>]
 [-Top <Int32>] [-ODataQuery <String>] [-TagName <String>] [-TagValue <String>]
 [-ResourceGroupNameContains <String>] [-ExpandProperties] [-ApiVersion <String>] [-Pre]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Find-AzureRmResource** cmdlet searches for resources based on specified parameters.

## EXAMPLES

### Example 1: Search for resources by type and resource group name
```
PS C:\>Find-AzureRmResource -ResourceType "microsoft.web/sites" -ResourceGroupNameContains "ResourceGroup"
```

This command searches for resources of the type microsoft.web/sites under resource groups that have names that match the string ResourceGroup.

### Example 2: Search for resources by type and resource name
```
PS C:\>Find-AzureRmResource -ResourceType "microsoft.web/sites" -ResourceNameContains "test"
```

This command searches for resources of the type microsoft.web/sites that have a resource name that matches the string test.

## PARAMETERS

### -ResourceNameContains
Specifies a partial name of a resource.
The cmdlet searches for resources which contain this value as a substring.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Name

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceType
Specifies the type of a resource.
For instance, for a database, the resource type is as follows: 

`Microsoft.Sql/Servers/Databases`

This cmdlet searches for resources of the specified type.

```yaml
Type: String
Parameter Sets: Lists the resources based on the specified scope.
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: Lists the resources based on the specified scope at the tenant level., Get a resources using a multi-subscription query.
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ExtensionResourceType
Specifies the extension resource type for the resources for which this cmdlet searches.
For instance: 

`Microsoft.Sql/Servers/Databases`

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

### -TagName
```yaml
Type: String
Parameter Sets: Lists the resources based on the specified scope., Get a resources using a multi-subscription query.
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TagValue
```yaml
Type: String
Parameter Sets: Lists the resources based on the specified scope., Get a resources using a multi-subscription query.
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExpandProperties
Indicates that this cmdlet expands the properties of the resource.

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

### -Top
Specifies the number of resources to retrieve.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ODataQuery
Specifies an Open Data Protocol (OData) style filter.
This cmdlet appends this value to the request in addition to any other filters.

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

### -ApiVersion
Specifies the version of the resource provider API to use.
If you do not specify a version, this cmdlet uses the latest available version.

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

### -TenantLevel
Indicates that this cmdlet operates at the tenant level.

```yaml
Type: SwitchParameter
Parameter Sets: Lists the resources based on the specified scope at the tenant level.
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupNameContains
Specifies a partial name of a resource group.
This cmdlet matches resource groups of which this value is a substring.
The cmdlet searches for resources in those resource groups.

```yaml
Type: String
Parameter Sets: Lists the resources based on the specified scope., Get a resources using a multi-subscription query.
Aliases: ResourceGroupName

Required: False
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

[Get-AzureRmResource](xref:ResourceManager/AzureRM.Resources/v3.3.0/Get-AzureRmResource.md)

[Move-AzureRmResource](xref:ResourceManager/AzureRM.Resources/v3.3.0/Move-AzureRmResource.md)

[New-AzureRmResource](xref:ResourceManager/AzureRM.Resources/v3.3.0/New-AzureRmResource.md)

[Remove-AzureRmResource](xref:ResourceManager/AzureRM.Resources/v3.3.0/Remove-AzureRmResource.md)

[Set-AzureRmResource](xref:ResourceManager/AzureRM.Resources/v3.3.0/Set-AzureRmResource.md)

