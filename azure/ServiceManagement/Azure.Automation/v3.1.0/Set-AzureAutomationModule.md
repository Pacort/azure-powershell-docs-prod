---
external help file: Microsoft.Azure.Commands.Automation.dll-Help.xml
ms.assetid: 24ACC1F1-F78A-4ECD-A996-31EC153F911C
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v3.1.0/Set-AzureAutomationModule.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v3.1.0/Set-AzureAutomationModule.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureAutomationModule

## SYNOPSIS
Updates a module in Automation.

## SYNTAX

```
Set-AzureAutomationModule [-Name] <String> [-Tags <IDictionary>] [-ContentLinkUri <Uri>]
 [-ContentLinkVersion <String>] [-AutomationAccountName] <String> [-Profile <AzureSMProfile>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureAutomationModule** cmdlet imports a new version of a module or changes the configuration of the module in Azure Automation.

## EXAMPLES

### Example 1: Update a module
```
PS C:\> Set-AzureAutomationModule  Â¢ ¢â€šÂ¬"AutomationAccountName "Contoso17"  Â¢ ¢â€šÂ¬"Name "ContosoModule"  Â¢ ¢â€šÂ¬"ContentLinkUri ".\ContosoModule.zip"  Â¢ ¢â€šÂ¬"ContentLinkVersion "1.1"
```

This command imports an updated version of an existing module named ContosoModule into the Azure Automation account named Contoso17.

## PARAMETERS

### -Name
Specifies the name of the module.

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

### -Tags
Specifies tags for the module.

```yaml
Type: IDictionary
Parameter Sets: (All)
Aliases: Tag

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ContentLinkUri
Specifies the path to the module file.

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ContentLinkVersion
Specifies the version of the module.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -AutomationAccountName
Specifies the name of the Automation account with the module.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.Commands.Automation.Model.Module

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureAutomationModule](xref:ServiceManagement/Azure.Automation/v3.1.0/Get-AzureAutomationModule.md)

[New-AzureAutomationModule](xref:ServiceManagement/Azure.Automation/v3.1.0/New-AzureAutomationModule.md)

[Remove-AzureAutomationModule](xref:ServiceManagement/Azure.Automation/v3.1.0/Remove-AzureAutomationModule.md)

