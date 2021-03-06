---
external help file: Microsoft.Azure.Commands.ManagedCache.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 8B37D2F7-373F-4735-97CA-081EE6AD0864
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.ManagedCache/v1.6.1/Get-AzureManagedCache.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.ManagedCache/v1.6.1/Get-AzureManagedCache.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ServiceManagement/Azure.ManagedCache/v1.6.1/Get-AzureManagedCache.md
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

# Get-AzureManagedCache

## SYNOPSIS
Gets the Azure Caches in your Azure account.

## SYNTAX

```
Get-AzureManagedCache [[-Name] <String>] [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureManagedCache** cmdlet get the Azure Caches in your account.
By default, it gets all Azure Caches in the account.
To get a particular Azure Cache, use the *Name* parameter.
An Azure Cache is a secure, dedicated cache that provides extremely fast access to data.
This distributed, in-memory, scalable solution enables you to build highly scalable and responsive applications.
For more information about Azure Cache, see Azure Cachehttp://azure.microsoft.com/en-us/services/cache/.

## EXAMPLES

### Example 1: Get all Azure Caches
```
PS C:\>Get-AzureManagedCache
```

This command gets all Azure Caches in your account.

### Example 2: Get an Azure Cache by name
```
PS C:\>Get-AzureManagedCache -Name "ContosoCache"
```

This command gets the Azure Cache named ContosoCache.

## PARAMETERS

### -Name
Specifies the Azure cache.
You need to supply the name of an Azure Cache.
This parameter is case-sensitive.
This parameter is optional.
By default, **Get-AzureManagedCache** gets all Azure caches in the account.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
ps_azureprofile_description

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

### None

## OUTPUTS

### Microsoft.Azure.Commands.ManagedCache.Models.PSCacheService

## NOTES
* Before you use this cmdlet, call Add-AzureAccount or Import-AzurePublishSettingsFile to make your Azure account available to wps_2. For more information, see How to install and configure Azure PowerShellhttp://azure.microsoft.com/en-us/documentation/articles/install-configure-powershell/.

## RELATED LINKS

[New-AzureManagedCache](xref:ServiceManagement/Azure.ManagedCache/v1.6.1/New-AzureManagedCache.md)

[Set-AzureManagedCache](xref:ServiceManagement/Azure.ManagedCache/v1.6.1/Set-AzureManagedCache.md)

[Remove-AzureManagedCache](xref:ServiceManagement/Azure.ManagedCache/v1.6.1/Remove-AzureManagedCache.md)

[Get-AzureManagedCacheAccessKey](xref:ServiceManagement/Azure.ManagedCache/v1.6.1/Get-AzureManagedCacheAccessKey.md)

[New-AzureManagedCacheAccessKey](xref:ServiceManagement/Azure.ManagedCache/v1.6.1/New-AzureManagedCacheAccessKey.md)


