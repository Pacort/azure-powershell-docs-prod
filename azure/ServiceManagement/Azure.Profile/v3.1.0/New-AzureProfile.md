---
external help file: Microsoft.WindowsAzure.Commands.Profile.dll-Help.xml
ms.assetid: D3D0E796-B485-4920-9AF9-9DC690736593
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Profile/v3.1.0/New-AzureProfile.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ServiceManagement/Azure.Profile/v3.1.0/New-AzureProfile.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureProfile

## SYNOPSIS

## SYNTAX

### Token
```
New-AzureProfile [-Environment <AzureEnvironment>] [-SubscriptionId] <String> [-StorageAccount <String>]
 [-AccessToken] <String> [-AccountId] <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

### Credentials
```
New-AzureProfile [-Environment <AzureEnvironment>] [-SubscriptionId] <String> [-StorageAccount <String>]
 [-Credential] <PSCredential> [[-Tenant] <String>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

### Empty
```
New-AzureProfile [-Environment <AzureEnvironment>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

### Certificate
```
New-AzureProfile [-Environment <AzureEnvironment>] [-SubscriptionId] <String> [-StorageAccount <String>]
 [-Certificate] <X509Certificate2> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

### ServicePrincipal
```
New-AzureProfile [-Environment <AzureEnvironment>] [-SubscriptionId] <String> [-StorageAccount <String>]
 [-Credential] <PSCredential> [-Tenant] <String> [-ServicePrincipal] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

### File
```
New-AzureProfile [-Path] <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

### PropertyBag
```
New-AzureProfile [-Properties] <Hashtable> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### 1:
```
PS C:\>
```

## PARAMETERS

### -Environment
```yaml
Type: AzureEnvironment
Parameter Sets: Token, Credentials, Empty, Certificate, ServicePrincipal
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubscriptionId
```yaml
Type: String
Parameter Sets: Token, Credentials, Certificate, ServicePrincipal
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StorageAccount
```yaml
Type: String
Parameter Sets: Token, Credentials, Certificate, ServicePrincipal
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AccessToken
```yaml
Type: String
Parameter Sets: Token
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AccountId
```yaml
Type: String
Parameter Sets: Token
Aliases: 

Required: True
Position: 1
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

### -Credential
```yaml
Type: PSCredential
Parameter Sets: Credentials, ServicePrincipal
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Tenant
```yaml
Type: String
Parameter Sets: Credentials
Aliases: TenantId

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: ServicePrincipal
Aliases: TenantId

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Certificate
```yaml
Type: X509Certificate2
Parameter Sets: Certificate
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ServicePrincipal
```yaml
Type: SwitchParameter
Parameter Sets: ServicePrincipal
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Path
```yaml
Type: String
Parameter Sets: File
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Properties
```yaml
Type: Hashtable
Parameter Sets: PropertyBag
Aliases: 

Required: True
Position: 0
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
