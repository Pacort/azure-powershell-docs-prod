---
external help file: Microsoft.Azure.Commands.TrafficManager.dll-Help.xml
ms.assetid: CEE33B80-28F2-4913-A46F-F418D79FBEA3
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.TrafficManager/v2.3.0/Get-AzureRmTrafficManagerProfile.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.TrafficManager/v2.3.0/Get-AzureRmTrafficManagerProfile.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmTrafficManagerProfile

## SYNOPSIS
Gets a Traffic Manager profile.

## SYNTAX

```
Get-AzureRmTrafficManagerProfile [-Name <String>] [-ResourceGroupName <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmTrafficManagerProfile** cmdlet gets an Azure Traffic Manager profile, and returns an object that represents that profile.
Specify a profile by its name and resource group name.

You can modify this object locally, and then apply changes to the profile by using the Set-AzureRmTrafficManagerProfile cmdlet.

## EXAMPLES

### Example 1: Get a profile
```
PS C:\>Get-AzureRmTrafficManagerProfile -Name "ContosoProfile" -ResourceGroupName "ResourceGroup11"
```

This command gets the profile named ContosoProfile in ResourceGroup11.

## PARAMETERS

### -Name
Specifies the name of the Traffic Manager profile that this cmdlet gets.

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

### -ResourceGroupName
Specifies the name of a resource group that contains the Traffic Manager profile that this cmdlet gets.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.Commands.Network.TrafficManagerProfile
This cmdlet returns a **TrafficManagerProfile** object.
You can modify this object, and then apply changes to Traffic Manager by using **Set-AzureRmTrafficManagerProfile**.

## NOTES

## RELATED LINKS

[Disable-AzureRmTrafficManagerProfile](xref:ResourceManager/AzureRM.TrafficManager/v2.3.0/Disable-AzureRmTrafficManagerProfile.md)

[Enable-AzureRmTrafficManagerProfile](xref:ResourceManager/AzureRM.TrafficManager/v2.3.0/Enable-AzureRmTrafficManagerProfile.md)

[New-AzureRmTrafficManagerProfile](xref:ResourceManager/AzureRM.TrafficManager/v2.3.0/New-AzureRmTrafficManagerProfile.md)

[Remove-AzureRmTrafficManagerProfile](xref:ResourceManager/AzureRM.TrafficManager/v2.3.0/Remove-AzureRmTrafficManagerProfile.md)

[Set-AzureRmTrafficManagerProfile](xref:ResourceManager/AzureRM.TrafficManager/v2.3.0/Set-AzureRmTrafficManagerProfile.md)

