---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.Network.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: CEE286D6-9945-4ED3-9D96-6FD831B9DE42
updated_at: 1/12/2017 12:24 AM
ms.date: 1/12/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.0.0/Set-AzureVNetGatewayIPsecParameters.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.0.0/Set-AzureVNetGatewayIPsecParameters.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/e57471ccf6c62263125f4c01fc0b0ce8ed76d386/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.0.0/Set-AzureVNetGatewayIPsecParameters.md
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

# Set-AzureVNetGatewayIPsecParameters

## SYNOPSIS
Sets IPsec parameters for the connection between a virtual network gateway and a local network site.

## SYNTAX

```
Set-AzureVNetGatewayIPsecParameters [-VNetName] <String> [-LocalNetworkSiteName] <String>
 [[-EncryptionType] <String>] [[-PfsGroup] <String>] [[-SADataSizeKilobytes] <Int32>]
 [[-SALifetimeSeconds] <Int32>] [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureVNetGatewayIPsecParameters** cmdlet sets Internet Protocol security (IPsec) and Internet Key Exchange (IKE) parameters for the connection between a virtual network gateway and a local network site.

## EXAMPLES


## PARAMETERS

### -VNetName
Specifies the virtual network for which this cmdlet sets IPsec parameters for the connection.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LocalNetworkSiteName
Specifies the name of the local network site connection on which this cmdlet configures the IPsec and IKE parameters.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EncryptionType
Specifies the encryption type for the virtual network gateway.
Valid values are: 

- NoEncryption 
- RequireEncryption

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PfsGroup
Specifies the perfect forward secrecy (PFS) group.
Valid values are: 

- PFS1 
- None

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SADataSizeKilobytes
Specifies the size, in kilobytes, of the security association (SA).

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SALifetimeSeconds
Specifies the period, in seconds, of the security association.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads. 
If you do not specify a profile, this cmdlet reads from the local default profile.
By default, this cmdlet does not generate any output.

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

[Get-AzureVNetGatewayIPsecParameters](xref:ServiceManagement/Azure.Networking/v3.0.0/Get-AzureVNetGatewayIPsecParameters.md)


