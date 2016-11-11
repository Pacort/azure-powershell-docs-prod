---
external help file: Microsoft.WindowsAzure.Commands.SqlDatabase.dll-Help.xml
ms.assetid: 54BA99EE-1B0E-4E28-98D2-E6FDB452E013
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.SQLDatabase/v3.1.0/New-AzureSqlDatabaseServerFirewallRule.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ServiceManagement/Azure.SQLDatabase/v3.1.0/New-AzureSqlDatabaseServerFirewallRule.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureSqlDatabaseServerFirewallRule

## SYNOPSIS
Creates a firewall rule in Azure SQL Database Server.

## SYNTAX

### IpRange (Default)
```
New-AzureSqlDatabaseServerFirewallRule [-ServerName] <String> -RuleName <String> -StartIpAddress <String>
 -EndIpAddress <String> [-Force] [-Profile <AzureSMProfile>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### AllowAllAzureServices
```
New-AzureSqlDatabaseServerFirewallRule [-ServerName] <String> [-RuleName <String>] [-AllowAllAzureServices]
 [-Force] [-Profile <AzureSMProfile>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureSqlDatabaseServerFirewallRule** cmdlet creates a firewall rule in the specified instance of Azure SQL Database Server in the current subscription.

Use the *StartIpAddress* and *EndIpAddress* parameters to specify a range of IP addresses that this rule allows to connect to the Azure SQL Database server.

Specify the *AllowAllAzureServices* parameter to create a rule that allows Azure connections to the server.
The rule has starting and ending IP address values of 0.0.0.0.
If you do not specify a firewall rule name, this cmdlet assigns the default name AllowAllAzureServices.

## EXAMPLES

### Example 1: Create a firewall rule
```
PS C:\>New-AzureSqlDatabaseServerFirewallRule -ServerName "lpqd0zbr8y" -RuleName "FirewallRule24" -StartIpAddress 10.1.1.1 -EndIpAddress 10.1.1.2
```

This command creates a firewall rule FirewallRule24 on the Azure SQL Database server named lpqd0zbr8y.
The command specifies an IP address range.

### Example 2: Create a rule that allows all Azure services
```
PS C:\>New-AzureSqlDatabaseServerFirewallRule -ServerName "lpqd0zbr8y" -AllowAllAzureServices -RuleName "AzureConnections"
```

This command creates a firewall rule named AzureConnections on the server named lpqd0zbr8y that allows Azure connections.

### Example 3: Create a rule that allows all Azure services that uses the default name Create a rule that allows all Azure services that uses the default name
```
PS C:\>New-AzureSqlDatabaseServerFirewallRule -ServerName "lpqd0zbr8y" -AllowAllAzureServices
```

This command creates a firewall rule on the specified server named lpqd0zbr8y that allows Azure connections.
The command assigns the default rule name AllowAllAzureServices.

## PARAMETERS

### -ServerName
Specifies the name of a server.
This cmdlet creates a firewall rule on the server that this cmdlet specifies.
Specify the server name, not the fully qualified DNS name.

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

### -RuleName
Specifies the name of the new firewall rule.

```yaml
Type: String
Parameter Sets: IpRange
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: AllowAllAzureServices
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartIpAddress
Specifies the start value of the IP address range for the firewall rule.

```yaml
Type: String
Parameter Sets: IpRange
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EndIpAddress
Specifies the end value of the IP address range for this rule.

```yaml
Type: String
Parameter Sets: IpRange
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Forces the command to run without asking for user confirmation.

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

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.Shows what would happen if the cmdlet runs.
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

### -Confirm
Prompts you for confirmation before running the cmdlet.Prompts you for confirmation before running the cmdlet.

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

### -AllowAllAzureServices
Indicates that this firewall rule enables all Azure IP addresses to access the server.

```yaml
Type: SwitchParameter
Parameter Sets: AllowAllAzureServices
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.WindowsAzure.Commands.SqlDatabase.Model.SqlDatabaseServerFirewallRuleContext

## NOTES

## RELATED LINKS

[Azure SQL Database](https://azure.microsoft.com/en-us/services/sql-database/)

[Create Firewall Rule](https://msdn.microsoft.com/en-us/library/azure/dn505712.aspx)

[Operations for Azure SQL Databases](https://msdn.microsoft.com/en-us/library/azure/dn505719.aspx)

[Get-AzureSqlDatabaseServerFirewallRule](xref:ServiceManagement/Azure.SQLDatabase/v3.1.0/Get-AzureSqlDatabaseServerFirewallRule.md)

[Remove-AzureSqlDatabaseServerFirewallRule](xref:ServiceManagement/Azure.SQLDatabase/v3.1.0/Remove-AzureSqlDatabaseServerFirewallRule.md)

[Set-AzureSqlDatabaseServerFirewallRule](xref:ServiceManagement/Azure.SQLDatabase/v3.1.0/Set-AzureSqlDatabaseServerFirewallRule.md)

