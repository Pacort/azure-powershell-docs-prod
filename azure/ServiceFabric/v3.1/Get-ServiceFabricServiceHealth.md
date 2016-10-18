---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 10/18/2016 3:14 PM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/v3.1/Get-ServiceFabricServiceHealth.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/93811e1b392b99b3b32acb51bf4afbefcc6a139c/Service-Fabric-cmdlets/ServiceFabric/v3.1/Get-ServiceFabricServiceHealth.md
ms.topic: reference
ms.prod: powershell
ms.service: service-fabric
ms.technology: Azure Powershell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-ServiceFabricServiceHealth

## SYNOPSIS
{{Fill in the Synopsis}}

## SYNTAX

```
Get-ServiceFabricServiceHealth [-ServiceName] <Uri> [-ConsiderWarningAsError <Boolean>]
 [-MaxPercentUnhealthyPartitionsPerService <Byte>] [-MaxPercentUnhealthyReplicasPerPartition <Byte>]
 [-EventsHealthStateFilter <Int64>] [-EventsFilter <HealthStateFilter>] [-PartitionsHealthStateFilter <Int64>]
 [-PartitionsFilter <HealthStateFilter>] [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
{{Fill in the Description}}

## EXAMPLES

### Example 1
```
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -ConsiderWarningAsError
{{Fill ConsiderWarningAsError Description}}

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EventsFilter
{{Fill EventsFilter Description}}

```yaml
Type: HealthStateFilter
Parameter Sets: (All)
Aliases: 
Accepted values: Default, None, Ok, Warning, Error, All

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EventsHealthStateFilter
{{Fill EventsHealthStateFilter Description}}

```yaml
Type: Int64
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MaxPercentUnhealthyPartitionsPerService
{{Fill MaxPercentUnhealthyPartitionsPerService Description}}

```yaml
Type: Byte
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MaxPercentUnhealthyReplicasPerPartition
{{Fill MaxPercentUnhealthyReplicasPerPartition Description}}

```yaml
Type: Byte
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PartitionsFilter
{{Fill PartitionsFilter Description}}

```yaml
Type: HealthStateFilter
Parameter Sets: (All)
Aliases: 
Accepted values: Default, None, Ok, Warning, Error, All

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PartitionsHealthStateFilter
{{Fill PartitionsHealthStateFilter Description}}

```yaml
Type: Int64
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServiceName
{{Fill ServiceName Description}}

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TimeoutSec
{{Fill TimeoutSec Description}}

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Uri

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS
