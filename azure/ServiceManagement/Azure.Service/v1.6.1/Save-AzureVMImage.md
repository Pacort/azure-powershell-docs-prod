---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 06D538B7-C3ED-4735-98C3-44958140E8DE
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/Save-AzureVMImage.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/Save-AzureVMImage.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/Save-AzureVMImage.md
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

# Save-AzureVMImage

## SYNOPSIS
Captures and saves the image of a stopped Azure virtual machine.

## SYNTAX

```
Save-AzureVMImage [-ServiceName] <String> [-Name] <String> [-ImageName] <String> [[-ImageLabel] <String>]
 [[-OSState] <String>] [-Profile <AzureSMProfile>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Save-AzureVMImage** cmdlet captures and saves the image of a stopped Azure virtual machine.
For Windows virtual machines, run the Sysprep tool to prepare the image before it is captured.
After the image is captured, the virtual machine is deleted.

## EXAMPLES

### Example 1: Save an existing virtual machine and then delete it from a deployment
```
PS C:\>Save-AzureVMImage -ServiceName "MyService" -Name "MyVM" -NewImageName "MyBaseImage" -NewImageLabel "MyBaseVM"
```

This command captures an existing virtual machine and deletes it from the deployment.

## PARAMETERS

### -ServiceName
Specifies the name of the Azure service.

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

### -Name
Specifies the name of the source virtual machine.

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

### -ImageName
Specifies the name of the virtual machine image.

```yaml
Type: String
Parameter Sets: (All)
Aliases: NewImageName

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ImageLabel
Specifies the label of the virtual machine image.

```yaml
Type: String
Parameter Sets: (All)
Aliases: NewImageLabel

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -OSState
Specifies the operation system state for the virtual machine image.
Use this parameter if you intend to capture a virtual machine image to Azure.

Valid values are:

- Generalized
- Specialized

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: True (ByPropertyName)
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

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AzureVMImage](xref:ServiceManagement/Azure.Service/v1.6.1/Add-AzureVMImage.md)

[Get-AzureVMImage](xref:ServiceManagement/Azure.Service/v1.6.1/Get-AzureVMImage.md)

[Remove-AzureVMImage](xref:ServiceManagement/Azure.Service/v1.6.1/Remove-AzureVMImage.md)

[Update-AzureVMImage](xref:ServiceManagement/Azure.Service/v1.6.1/Update-AzureVMImage.md)


