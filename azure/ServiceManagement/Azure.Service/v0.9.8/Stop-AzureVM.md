---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: D9EADB83-9A6B-4E1A-A429-2FCA8FC31152
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v0.9.8/Stop-AzureVM.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v0.9.8/Stop-AzureVM.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v0.9.8/Stop-AzureVM.md
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

# Stop-AzureVM

## SYNOPSIS
Shuts down an Azure virtual machine.

## SYNTAX

### ByName (Default)
```
Stop-AzureVM [-Name] <String[]> [-StayProvisioned] [-Force] [-ServiceName] <String> [-Profile <AzureProfile>]
 [-PipelineVariable <String>] [<CommonParameters>]
```

### Input
```
Stop-AzureVM -VM <IPersistentVM[]> [-StayProvisioned] [-Force] [-ServiceName] <String>
 [-Profile <AzureProfile>] [-PipelineVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Stop-AzureVM** cmdlet shuts down a virtual machine.

## EXAMPLES

### Example 1: Shut down a virtual machine
```
PS C:\>Stop-AzureVM -ServiceName "ContosoService01" -Name "MyVM"
```

This command shuts down a virtual machine that the specified service contains.

### Example 2: Shut down a virtual machine by using a virtual machine object
```
PS C:\>Get-AzureVM -ServiceName "ContosoService01" -Name "MyVM" | Stop-AzureVM
```

This command shuts down a virtual machine that the specified service contains, by using the virtual machine object that **Get-AzureVM** returns.

### Example 3: Shut down a VM and keep the VM provisioned
```
PS C:\>Stop-AzureVM -ServiceName "ContosoService01" -Name "MyVM" -StayProvisioned
```

This command shuts down a virtual machine that the specified service contains, and keeps it provisioned.

### Example 4: Shut down a VM and allow deallocation of the last VM in the deployment
```
PS C:\>Stop-AzureVM -ServiceName "ContosoService01" -Name "MyVM" -Force
```

This command shuts down a virtual machine that the specified service contains and allows deallocation of the last virtual machine in the deployment.

### Example 5: Shut down multiple VMs
```
PS C:\>Stop-AzureVM -ServiceName "PSTestService" -Name "*" -Force
```

This command shuts down multiple virtual machines that the specified service contains.

## PARAMETERS

### -Name
Specifies the name of the virtual machine to shut down.

Use the wildcard character to stop multiple virtual machines asynchronously.
With a wildcard character, this cmdlet calls the Shutdown Roleshttp://msdn.microsoft.com/en-us/library/azure/dn469421.aspx operation (http://msdn.microsoft.com/en-us/library/azure/dn469421.aspx), instead of the Shutdown Rolehttp://msdn.microsoft.com/en-us/library/azure/jj157195.aspx operation (http://msdn.microsoft.com/en-us/library/azure/jj157195.aspx).

```yaml
Type: String[]
Parameter Sets: ByName
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -StayProvisioned
Specifies that this cmdlet keeps the virtual machine provisioned.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Specifies whether to allow the deallocation of the last virtual machine in a deployment.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServiceName
Specifies the name of the Azure service that contains the virtual machine to shut down.

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

### -VM
Specifies a virtual machine object that identifies the virtual machine to shut down.

```yaml
Type: IPersistentVM[]
Parameter Sets: Input
Aliases: InputObject

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PipelineVariable
Not Specified

```yaml
Type: String
Parameter Sets: (All)
Aliases: pv

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
Type: AzureProfile
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

[Get-AzureVM](xref:ServiceManagement/Azure.Service/v0.9.8/Get-AzureVM.md)

[New-AzureVM](xref:ServiceManagement/Azure.Service/v0.9.8/New-AzureVM.md)

[Restart-AzureVM](xref:ServiceManagement/Azure.Service/v0.9.8/Restart-AzureVM.md)

[Start-AzureVM](xref:ServiceManagement/Azure.Service/v0.9.8/Start-AzureVM.md)


