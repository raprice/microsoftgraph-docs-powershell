---
external help file: Microsoft.Graph.DeviceManagement.Actions-help.xml
Module Name: Microsoft.Graph.DeviceManagement.Actions
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.devicemanagement.actions/approve-mgdevicemanagementandroidmanagedstoreaccountenterprisesettingapp
schema: 2.0.0
---

# Approve-MgDeviceManagementAndroidManagedStoreAccountEnterpriseSettingApp

## SYNOPSIS
Invoke action approveApps

## SYNTAX

### ApproveExpanded (Default)
```
Approve-MgDeviceManagementAndroidManagedStoreAccountEnterpriseSettingApp [-AdditionalProperties <Hashtable>]
 [-ApproveAllPermissions] [-PackageIds <String[]>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Approve
```
Approve-MgDeviceManagementAndroidManagedStoreAccountEnterpriseSettingApp
 -BodyParameter <IPathsQ0Me7IDevicemanagementAndroidmanagedstoreaccountenterprisesettingsMicrosoftGraphApproveappsPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Invoke action approveApps

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: ApproveExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApproveAllPermissions
.

```yaml
Type: SwitchParameter
Parameter Sets: ApproveExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
.
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPathsQ0Me7IDevicemanagementAndroidmanagedstoreaccountenterprisesettingsMicrosoftGraphApproveappsPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Approve
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PackageIds
.

```yaml
Type: String[]
Parameter Sets: ApproveExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Returns true when the command succeeds

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

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
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
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IPathsQ0Me7IDevicemanagementAndroidmanagedstoreaccountenterprisesettingsMicrosoftGraphApproveappsPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IPathsQ0Me7IDevicemanagementAndroidmanagedstoreaccountenterprisesettingsMicrosoftGraphApproveappsPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ApproveAllPermissions <Boolean?>]`: 
  - `[PackageIds <String[]>]`: 

## RELATED LINKS
