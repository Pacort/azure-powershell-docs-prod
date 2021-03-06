---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: DF12EFA0-9447-412D-A58C-89F25DDC182E
updated_at: 1/11/2017 6:32 PM
ms.date: 1/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Set-AzureWalkUpgradeDomain.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Set-AzureWalkUpgradeDomain.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/34e1c9880d0370f1dd5f83ea8d5ee7f59cb5e559/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Set-AzureWalkUpgradeDomain.md
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

# Set-AzureWalkUpgradeDomain

## SYNOPSIS
Walks the specified upgrade domain.

## SYNTAX

```
Set-AzureWalkUpgradeDomain [-ServiceName] <String> [-Slot] <String> [-DomainNumber] <Int32>
 [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureWalkUpgradeDomain** cmdlet initiates the actual upgrade of an Azure deployment.
The upgrade package and configuration are set by using the **Set-AzureDeployment** cmdlet with the -Upgrade switch.

## EXAMPLES

### Example 1: Initiate an upgrade of a production deployment
```
PS C:\> Set-AzureWalkUpgradeDomain -ServiceName "MySvc1" -slot "Production" -UpgradeDomain 2
```

This command initiates the upgrade of Upgrade Domain 2 of the production deployment of the MySvc1 service.

## PARAMETERS

### -ServiceName
Specifies the Microsoft Azure service name to upgrade.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Slot
Specifies the environment of the deployment to upgrade.

The acceptable values for this parameter are:

- Staging
- Production

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

### -DomainNumber
Specifies the upgrade domain to upgrade.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### ManagementOperationContext

## NOTES

## RELATED LINKS

[Set-AzureDeployment](xref:ServiceManagement/Azure.Service/v3.0.0/Set-AzureDeployment.md)


