---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.Network.dll-Help.xml
online version: d6f05722-55c2-4419-9ff3-52f0874327b6
schema: 2.0.0
ms.assetid: DC5D95FA-D713-430F-8DD1-525C0401FBE6
updated_at: 10/24/2016 11:18 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.0.0/Start-AzureVNetGatewayDiagnostics.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/7db57df6b5e709a7c001e6de362a1240d7583ae8/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.0.0/Start-AzureVNetGatewayDiagnostics.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Start-AzureVNetGatewayDiagnostics

## SYNOPSIS
Starts gateway diagnostics for a VPN gateway.

## SYNTAX

```
Start-AzureVNetGatewayDiagnostics [-VNetName] <String> [-CaptureDurationInSeconds] <Int32>
 [[-ContainerName] <String>] [-StorageContext] <AzureStorageContext> [-Profile <AzureSMProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Start-AzureVNetGatewayDiagnostics** cmdlet starts a new gateway diagnostics session for a virtual private network (VPN) gateway.
Only one gateway diagnostics session can run at a time.
If you run this cmdlet while a gateway diagnostics session is running, this cmdlet returns an error.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -VNetName
Specifies the virtual network that contains a virtual network gateway for which this cmdlet runs diagnostics.

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

### -CaptureDurationInSeconds
Specifies the capture duration in seconds.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ContainerName
Specifies the name of an azure_2 container.
This cmdlet stores results in the container that this parameter specifies.

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

### -StorageContext
Specifies an azure_2 storage context.
This cmdlet stores results by using the storage context that this parameter specifies.

```yaml
Type: AzureStorageContext
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: False
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

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureVNetGatewayDiagnostics](.\Get-AzureVNetGatewayDiagnostics.md)

[Stop-AzureVNetGatewayDiagnostics](.\Stop-AzureVNetGatewayDiagnostics.md)

