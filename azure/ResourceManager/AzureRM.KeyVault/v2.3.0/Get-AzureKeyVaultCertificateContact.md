---
external help file: Microsoft.Azure.Commands.KeyVault.dll-Help.xml
ms.assetid: 996FA5F2-AFAE-4424-AFDB-2DEEAB5143D1
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.3.0/Get-AzureKeyVaultCertificateContact.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.3.0/Get-AzureKeyVaultCertificateContact.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureKeyVaultCertificateContact

## SYNOPSIS
Gets contacts that are registered for certificate notifications for a key vault.

## SYNTAX

```
Get-AzureKeyVaultCertificateContact [-VaultName] <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureKeyVaultCertificateContact** cmdlet gets contacts that are registered for certificate notifications for a key vault in Azure Key Vault.

## EXAMPLES

### Example 1: Get all certificate contacts
```
PS C:\>$Contacts = Get-AzureKeyVaultCertificateContact -VaultName "Contoso"
```

This command gets all of the contacts for the certificate objects in the Contoso key vault, and then stores them in the $Contacts variable.

## PARAMETERS

### -VaultName
Specifies the name of the key vault.

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

### List<Microsoft.Azure.Commands.KeyVault.Models.KeyVaultCertificateContact>

## NOTES

## RELATED LINKS

[Add-AzureKeyVaultCertificateContact](xref:ResourceManager/AzureRM.KeyVault/v2.3.0/Add-AzureKeyVaultCertificateContact.md)

[Remove-AzureKeyVaultCertificateContact](xref:ResourceManager/AzureRM.KeyVault/v2.3.0/Remove-AzureKeyVaultCertificateContact.md)

