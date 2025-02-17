---
external help file: Microsoft.Graph.DeviceManagement.Administration-help.xml
Module Name: Microsoft.Graph.DeviceManagement.Administration
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.devicemanagement.administration/update-mgdevicemanagementvirtualendpointcrosscloudgovernmentorganizationmapping
schema: 2.0.0
---

# Update-MgDeviceManagementVirtualEndpointCrossCloudGovernmentOrganizationMapping

## SYNOPSIS
Update the navigation property crossCloudGovernmentOrganizationMapping in deviceManagement

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgDeviceManagementVirtualEndpointCrossCloudGovernmentOrganizationMapping
 [-AdditionalProperties <Hashtable>] [-Id <String>] [-OrganizationIdsInUsGovCloud <String[]>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgDeviceManagementVirtualEndpointCrossCloudGovernmentOrganizationMapping
 -BodyParameter <IMicrosoftGraphCloudPcCrossCloudGovernmentOrganizationMapping> [-PassThru] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property crossCloudGovernmentOrganizationMapping in deviceManagement

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
cloudPcCrossCloudGovernmentOrganizationMapping
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphCloudPcCrossCloudGovernmentOrganizationMapping
Parameter Sets: Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Id
The unique idenfier for an entity.
Read-only.

```yaml
Type: String
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OrganizationIdsInUsGovCloud
The tenant ID in the Azure Government cloud corresponding to the GCC tenant in the public cloud.
Currently, 1:1 mappings are supported, so this collection can only contain one tenant ID.

```yaml
Type: String[]
Parameter Sets: UpdateExpanded
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphCloudPcCrossCloudGovernmentOrganizationMapping
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IMicrosoftGraphCloudPcCrossCloudGovernmentOrganizationMapping>`: cloudPcCrossCloudGovernmentOrganizationMapping
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[OrganizationIdsInUsGovCloud <String[]>]`: The tenant ID in the Azure Government cloud corresponding to the GCC tenant in the public cloud. Currently, 1:1 mappings are supported, so this collection can only contain one tenant ID.

## RELATED LINKS
