---
external help file: Microsoft.Online.Administration.Automation.PSModule.dll-Help.xml
online version:
schema: 2.0.0
ms.assetid: A41324CE-63FC-4802-8589-344C52732E49
updated_at: 11/9/2016 6:37 PM
ms.date: 11/9/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/MSOnline/v1/Set-MsolCompanySettings.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/MSOnline/v1/Set-MsolCompanySettings.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/7986fb4880d0ee292c289166871e4b25df1ad4b8/Azure%20AD%20Cmdlets/MSOnline/v1/Set-MsolCompanySettings.md
ms.topic: reference
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: carolz
open_to_public_contributors: true
ms.service: active-directory
---

# Set-MsolCompanySettings

## SYNOPSIS
Sets company-level configuration settings.

## SYNTAX

```
Set-MsolCompanySettings [-SelfServePasswordResetEnabled <Boolean>]
 [-UsersPermissionToCreateGroupsEnabled <Boolean>] [-UsersPermissionToCreateLOBAppsEnabled <Boolean>]
 [-UsersPermissionToReadOtherUsersEnabled <Boolean>] [-UsersPermissionToUserConsentToAppEnabled <Boolean>]
 [-DefaultUsageLocation <String>] [-AllowAdHocSubscriptions <Boolean>] [-AllowEmailVerifiedUsers <Boolean>]
 [-TenantId <Guid>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-MsolCompanySettings** cmdlet is used to set company-level configuration settings.
Use [Get-MsolCompanyInformation](./Get-MsolCompanyInformation.md) to read the current values of these settings.

## EXAMPLES

### Example 1: Turns on the self-serve password reset feature
```
PS C:\> Set-MsolCompanySettings -SelfServePasswordResetEnabled $True
```

This command turns on the self-serve password reset feature for all users in the company.

## PARAMETERS

### -SelfServePasswordResetEnabled
Indicates whether to allow the use of the self-service password reset feature.
This setting is applied company-wide.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UsersPermissionToCreateGroupsEnabled
Indicates whether to allow users to create groups.
This setting is applied company-wide.
Set to $False to disable users' ability to create groups.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -AllowAdHocSubscriptions
Indicates whether to allow users to sign up for email based subscriptions.
This setting is applied company-wide.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -AllowEmailVerifiedUsers
Indicates whether users can join the tenant by email validation.
To join, the user must have an email address in a domain which matches one of the verified domains in the tenant.
This setting is applied company-wide for all domains in the tenant.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UsersPermissionToCreateLOBAppsEnabled
Indicates whether to allow users to create new applications.
This setting is applied company-wide.
Set to False to disable users' ability to create new applications for their organization.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UsersPermissionToReadOtherUsersEnabled
Indicates whether to allow users to view the profile info of other users in their company.
This setting is applied company-wide.
Set to $False to disable users' ability to use the Azure AD module for Windows PowerShell to access user information for their organization.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UsersPermissionToUserConsentToAppEnabled
Indicates whether to allow users to consent to apps that require access to their cloud user data, such as directory user profile or Office 365 mail and OneDrive for business.
This setting is applied company-wide.
Set to $False to disable users' ability to grant consent to applications.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DefaultUsageLocation
When assigning licenses to Microsoft products this value will be applied to the User.UsageLocation attribute if none is present.
If the default value is $Null then the location value for the tenant is used.

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

### -TenantId
Specifies the unique ID of the tenant on which to perform the operation.
The default value is the tenant of the current user.
This parameter applies only to partner users.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
[Get-MsolCompanyInformation](xref:MSOnline/v1/Get-MsolCompanyInformation.md)
