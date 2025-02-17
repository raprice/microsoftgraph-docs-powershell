---
external help file: Microsoft.Graph.Identity.DirectoryManagement-help.xml
Module Name: Microsoft.Graph.Identity.DirectoryManagement
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.identity.directorymanagement/get-mgdirectorydeleteditemavailableextensionproperty
schema: 2.0.0
---

# Get-MgDirectoryDeletedItemAvailableExtensionProperty

## SYNOPSIS
Return all directory extension definitions that have been registered in a directory, including through multi-tenant apps.
The following entities support extension properties:\n+ user\n+ group\n+ administrativeUnit\n+ application\n+ device\n+ organization

## SYNTAX

### GetExpanded (Default)
```
Get-MgDirectoryDeletedItemAvailableExtensionProperty [-AdditionalProperties <Hashtable>]
 [-IsSyncedFromOnPremises] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Get
```
Get-MgDirectoryDeletedItemAvailableExtensionProperty
 -BodyParameter <IPaths1803LqaDirectoryDeleteditemsMicrosoftGraphGetavailableextensionpropertiesPostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Return all directory extension definitions that have been registered in a directory, including through multi-tenant apps.
The following entities support extension properties:\n+ user\n+ group\n+ administrativeUnit\n+ application\n+ device\n+ organization

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: GetExpanded
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
Type: IPaths1803LqaDirectoryDeleteditemsMicrosoftGraphGetavailableextensionpropertiesPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsSyncedFromOnPremises
.

```yaml
Type: SwitchParameter
Parameter Sets: GetExpanded
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

### Microsoft.Graph.PowerShell.Models.IPaths1803LqaDirectoryDeleteditemsMicrosoftGraphGetavailableextensionpropertiesPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphExtensionProperty
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IPaths1803LqaDirectoryDeleteditemsMicrosoftGraphGetavailableextensionpropertiesPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[IsSyncedFromOnPremises <Boolean?>]`: 

## RELATED LINKS
