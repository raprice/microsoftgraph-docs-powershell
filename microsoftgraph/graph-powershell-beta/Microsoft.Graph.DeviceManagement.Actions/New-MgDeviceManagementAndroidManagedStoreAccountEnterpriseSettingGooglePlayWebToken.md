---
external help file: Microsoft.Graph.DeviceManagement.Actions-help.xml
Module Name: Microsoft.Graph.DeviceManagement.Actions
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.devicemanagement.actions/new-mgdevicemanagementandroidmanagedstoreaccountenterprisesettinggoogleplaywebtoken
schema: 2.0.0
---

# New-MgDeviceManagementAndroidManagedStoreAccountEnterpriseSettingGooglePlayWebToken

## SYNOPSIS
Generates a web token that is used in an embeddable component.

## SYNTAX

### CreateExpanded (Default)
```
New-MgDeviceManagementAndroidManagedStoreAccountEnterpriseSettingGooglePlayWebToken
 [-AdditionalProperties <Hashtable>] [-ParentUri <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgDeviceManagementAndroidManagedStoreAccountEnterpriseSettingGooglePlayWebToken
 -BodyParameter <IPathsIaia9DDevicemanagementAndroidmanagedstoreaccountenterprisesettingsMicrosoftGraphCreategoogleplaywebtokenPostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Generates a web token that is used in an embeddable component.

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded
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
Type: IPathsIaia9DDevicemanagementAndroidmanagedstoreaccountenterprisesettingsMicrosoftGraphCreategoogleplaywebtokenPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ParentUri
.

```yaml
Type: String
Parameter Sets: CreateExpanded
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

### Microsoft.Graph.PowerShell.Models.IPathsIaia9DDevicemanagementAndroidmanagedstoreaccountenterprisesettingsMicrosoftGraphCreategoogleplaywebtokenPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### System.String
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IPathsIaia9DDevicemanagementAndroidmanagedstoreaccountenterprisesettingsMicrosoftGraphCreategoogleplaywebtokenPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ParentUri <String>]`: 

## RELATED LINKS
