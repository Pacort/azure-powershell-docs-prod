---
external help file: Microsoft.Azure.Commands.Sql.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: BBFA7BF9-47CE-4845-B266-0E8A9B7140E7
updated_at: 11/22/2016 8:52 PM
ms.date: 11/22/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Sql/v2.1.0/Get-AzureRmSqlDatabaseRestorePoints.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Sql/v2.1.0/Get-AzureRmSqlDatabaseRestorePoints.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0cedc8f73bc96cf5ac4c69144e17b3de601fd3cc/azureps-cmdlets-docs/ResourceManager/AzureRM.Sql/v2.1.0/Get-AzureRmSqlDatabaseRestorePoints.md
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

# Get-AzureRmSqlDatabaseRestorePoints

## SYNOPSIS
Retrieves the distinct restore points from which a SQL Data Warehouse can be restored.

## SYNTAX

```
Get-AzureRmSqlDatabaseRestorePoints [-ServerName] <String> [-DatabaseName] <String>
 [-ResourceGroupName] <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmSqlDatabaseRestorePoints** cmdlet retrieves the distinct restore points that an Azure SQL Data Warehouse can be restored from.
For an Azure SQL Database, the restore window is continuous.
This means that any point in time in the backup retention period of the database can be used as a restore point.

This cmdlet is also supported by the SQL Server Stretch Database service on Azure.

## EXAMPLES

### Example 1: Get all restore points
```
PS C:\>Get-AzureRmSqlDatabaseRestorePoints -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -DatabaseName "Database01"
ResourceGroupName        : resourcegroup01
ServerName               : server01
DatabaseName             : database01
Location                 : Central US
RestorePointType         : CONTINUOUS
RestorePointCreationDate : 
EarliestRestoreDate      : 8/12/2015 12:00:00 AM
```

This command returns all available restore points for the Azure SQL Database named Database01.

## PARAMETERS

### -ServerName
Specifies the name of the AzureSQL Server that hosts the database.

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

### -DatabaseName
Specifies the name of the SQL Database.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group to which the SQL Database is assigned.

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

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Azure SQL Database Cmdlets](xref:ResourceManager/AzureRM.Sql/v2.1.0/AzureRM.Sql.md)


