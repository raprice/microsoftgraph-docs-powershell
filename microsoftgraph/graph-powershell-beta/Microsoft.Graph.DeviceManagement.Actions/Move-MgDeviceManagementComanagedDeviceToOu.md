---
external help file: Microsoft.Graph.DeviceManagement.Actions-help.xml
Module Name: Microsoft.Graph.DeviceManagement.Actions
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.devicemanagement.actions/move-mgdevicemanagementcomanageddevicetoou
schema: 2.0.0
---

# Move-MgDeviceManagementComanagedDeviceToOu

## SYNOPSIS
Invoke action moveDevicesToOU

## SYNTAX

### MoveExpanded (Default)
```
Move-MgDeviceManagementComanagedDeviceToOu [-AdditionalProperties <Hashtable>] [-DeviceIds <String[]>]
 [-OrganizationalUnitPath <String>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Move
```
Move-MgDeviceManagementComanagedDeviceToOu
 -BodyParameter <IPathsU50RagDevicemanagementComanageddevicesMicrosoftGraphMovedevicestoouPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Invoke action moveDevicesToOU

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: MoveExpanded
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
Type: IPathsU50RagDevicemanagementComanageddevicesMicrosoftGraphMovedevicestoouPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Move
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DeviceIds
.

```yaml
Type: String[]
Parameter Sets: MoveExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OrganizationalUnitPath
.

```yaml
Type: String
Parameter Sets: MoveExpanded
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

### Microsoft.Graph.PowerShell.Models.IPathsU50RagDevicemanagementComanageddevicesMicrosoftGraphMovedevicestoouPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IPathsU50RagDevicemanagementComanageddevicesMicrosoftGraphMovedevicestoouPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DeviceIds <String[]>]`: 
  - `[OrganizationalUnitPath <String>]`: 

## RELATED LINKS
