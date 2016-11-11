---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
ms.assetid: CCB375E5-47CB-4147-9CE3-1DFC23D7D88D
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.1.0/Get-WAPackStaticIPAddressPool.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.1.0/Get-WAPackStaticIPAddressPool.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-WAPackStaticIPAddressPool

## SYNOPSIS
Gets static IP address pool objects.

## SYNTAX

### FromVMSubnetObject (Default)
```
Get-WAPackStaticIPAddressPool [-VMSubnet] <VMSubnet> [-Profile <AzureSMProfile>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

### FromName
```
Get-WAPackStaticIPAddressPool [-VMSubnet] <VMSubnet> [-Name] <String> [-Profile <AzureSMProfile>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
These topics are deprecated and will be removed in the future.
For the updated topics, see  Azure WAPack Cmdletshttp://msdn.microsoft.com/library/dn776450.aspx.
This topic describes the cmdlet in the 0.8.1 version of the Microsoft Azure PowerShell module.
To find out the version of the module you're using, from the Azure PowerShell console, type (get-module azure).version.

The **Get-WAPackStaticIPAddressPool** cmdlet gets static IP address pool objects.

## EXAMPLES

### Example 1: Get a static IP address pool from a given VMSubnet
```
PS C:\>$Subnet = Get-WAPackVMSubet -Name "ContosoVMSubnet01"
PS C:\>Get-WAPackStaticIPAddressPool -VMSubnet $Subnet -Name "ContosoStaticIPAddressPool01"
```

This command gets the static IP address pool named ContosoStaticIPAddressPool01 from a specified VMSubnet.

### Example 2: Get all static IP address pools from a given VMSubnet
```
PS C:\>$Subnet = Get-WAPackVMSubet -Name "ContosoVMSubnet01"
PS C:\> Get-WAPackStaticIPAddressPool -VMSubnet $Subnet
```

This command gets all the static IP pools from a specified VMSubet.

## PARAMETERS

### -VMSubnet
Specifies the **VMSubnet** object associated to the static IP address pool.

```yaml
Type: VMSubnet
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
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

### -Name
Specifies the name of a static IP address pool.

```yaml
Type: String
Parameter Sets: FromName
Aliases: 

Required: True
Position: 1
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

[New-WAPackStaticIPAddressPool](xref:ServiceManagement/Azure.Compute/v3.1.0/New-WAPackStaticIPAddressPool.md)

[Remove-WAPackStaticIPAddressPool](xref:ServiceManagement/Azure.Compute/v3.1.0/Remove-WAPackStaticIPAddressPool.md)

