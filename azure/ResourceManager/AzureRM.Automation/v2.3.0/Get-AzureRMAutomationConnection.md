---
external help file: Microsoft.Azure.Commands.ResourceManager.Automation.dll-Help.xml
ms.assetid: 68F56D1C-23A9-4CB5-8FE8-C3A1E7C2AC1A
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v2.3.0/Get-AzureRMAutomationConnection.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v2.3.0/Get-AzureRMAutomationConnection.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmAutomationConnection

## SYNOPSIS
Gets an Automation connection.

## SYNTAX

### ByAll (Default)
```
Get-AzureRmAutomationConnection [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [<CommonParameters>]
```

### ByConnectionName
```
Get-AzureRmAutomationConnection [-Name] <String> [-ResourceGroupName] <String>
 [-AutomationAccountName] <String> [<CommonParameters>]
```

### ByConnectionTypeName
```
Get-AzureRmAutomationConnection [-ConnectionTypeName] <String> [-ResourceGroupName] <String>
 [-AutomationAccountName] <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmAutomationConnection** cmdlet gets one or more Azure Automation connections.
By default, this cmdlet retrieves all connections.
Specify the name of a connection to get a specific connection.
Specify the connection type name to get all connections of a specific type.

## EXAMPLES

### Example 1: Get all connections
```
PS C:\>Get-AzureRmAutomationConnection -ResourceGroupName "ResourceGroup01" -AutomationAccountName "Contoso17"
```

This command gets metadata for all connections in the Automation account named Contoso17.

### Example 2: Get all connections of a type
```
PS C:\>Get-AzureRmAutomationConnection -ResourceGroupName "ResourceGroup01" -AutomationAccountName "Contoso17" -ConnectionTypeName "SqlServer"
```

This command gets metadata for connections in the Automation account named Contoso17.
This command gets connections of the type SqlServer.

### Example 3: Get a connection
```
PS C:\>Get-AzureRmAutomationConnection -ResourceGroupName "ResourceGroup01" -AutomationAccountName "Contoso17" -Name "ContosoConnection"
```

This command gets metadata for the connection named ContosoConnection.

## PARAMETERS

### -AutomationAccountName
Specifies the name of the Automation account for which this cmdlet gets connections.

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

### -ConnectionTypeName
Specifies the name of a connection type for which this cmdlet retrieves connections.

```yaml
Type: String
Parameter Sets: ByConnectionTypeName
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of a connection that this cmdlet retrieves.

```yaml
Type: String
Parameter Sets: ByConnectionName
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of a resource group for which this cmdlet gets connections.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.Commands.Automation.Model.Connection

## NOTES

## RELATED LINKS

[New-AzureRmAutomationConnection](xref:ResourceManager/AzureRM.Automation/v2.3.0/New-AzureRMAutomationConnection.md)

[Remove-AzureRmAutomationConnection](xref:ResourceManager/AzureRM.Automation/v2.3.0/Remove-AzureRMAutomationConnection.md)

