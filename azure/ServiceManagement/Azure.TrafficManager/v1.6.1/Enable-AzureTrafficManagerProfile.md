---
external help file: Microsoft.WindowsAzure.Commands.TrafficManager.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 7E3C0433-6955-4A12-AC5B-C72CC8844ED3
updated_at: 11/3/2016 6:38 AM
ms.date: 11/3/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.TrafficManager/v1.6.1/Enable-AzureTrafficManagerProfile.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/b99e9cf8cc8dbf12111d92b05669d2c50f01373c/azureps-cmdlets-docs/ServiceManagement/Azure.TrafficManager/v1.6.1/Enable-AzureTrafficManagerProfile.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Enable-AzureTrafficManagerProfile

## SYNOPSIS
Enables a Traffic Manager profile.

## SYNTAX

```
Enable-AzureTrafficManagerProfile [-Name] <String> [-PassThru] [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Enable-AzureTrafficManagerProfile** cmdlet enables a Microsoft Azure Traffic Manager profile.
Specify the *PassThru* parameter to display whether the operation succeeds.

## EXAMPLES

### Example 1: Enable a Traffic Manager profile
```
PS C:\>Enable-AzureTrafficManagerProfile -Name "MyProfile"
```

This command enables the Traffic Manager profile named MyProfile.

### Example 2: Enable a Traffic Manager profile and display the results
```
PS C:\>Enable-AzureTrafficManagerProfile -Name "MyProfile" -PassThru
True
```

This command enables the Traffic Manager profile named MyProfile and displays whether the command succeeded.

## PARAMETERS

### -Name
Specifies the name of the Traffic Manager profile to enable.

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

### -PassThru
Returns $True if the operation succeeded; otherwise, $False.
By default, this cmdlet does not generate any output.

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

### System.Boolean
This cmdlet generates $True or $False.
If the operation succeeds and if you specify the *PassThru* parameter, this cmdlet returns a value of $True.

## NOTES

## RELATED LINKS

[Disable-AzureTrafficManagerProfile](xref:ServiceManagement/Azure.TrafficManager/v1.6.1/Disable-AzureTrafficManagerProfile.md)

[Get-AzureTrafficManagerProfile](xref:ServiceManagement/Azure.TrafficManager/v1.6.1/Get-AzureTrafficManagerProfile.md)

[New-AzureTrafficManagerProfile](xref:ServiceManagement/Azure.TrafficManager/v1.6.1/New-AzureTrafficManagerProfile.md)

[Remove-AzureTrafficManagerProfile](xref:ServiceManagement/Azure.TrafficManager/v1.6.1/Remove-AzureTrafficManagerProfile.md)

[Set-AzureTrafficManagerProfile](xref:ServiceManagement/Azure.TrafficManager/v1.6.1/Set-AzureTrafficManagerProfile.md)

