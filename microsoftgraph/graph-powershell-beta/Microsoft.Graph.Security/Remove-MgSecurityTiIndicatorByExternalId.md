---
external help file: Microsoft.Graph.Security-help.xml
Module Name: Microsoft.Graph.Security
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.security/remove-mgsecuritytiindicatorbyexternalid
schema: 2.0.0
---

# Remove-MgSecurityTiIndicatorByExternalId

## SYNOPSIS
Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests, when the request contains external IDs instead of IDs.

## SYNTAX

### DeleteExpanded (Default)
```
Remove-MgSecurityTiIndicatorByExternalId [-AdditionalProperties <Hashtable>] [-Value <String[]>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Delete
```
Remove-MgSecurityTiIndicatorByExternalId
 -BodyParameter <IPaths1Jddi17SecurityTiindicatorsMicrosoftGraphDeletetiindicatorsbyexternalidPostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests, when the request contains external IDs instead of IDs.

## EXAMPLES

### Example 1: Using the Remove-MgSecurityTiIndicatorByExternalId Cmdlet
```powershell
Import-Module Microsoft.Graph.Security
$params = @{
	Value = @(
		"externalId-value1"
		"externalId-value2"
	)
}
Remove-MgSecurityTiIndicatorByExternalId -BodyParameter $params
```

This example shows how to use the Remove-MgSecurityTiIndicatorByExternalId Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: DeleteExpanded
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
Type: IPaths1Jddi17SecurityTiindicatorsMicrosoftGraphDeletetiindicatorsbyexternalidPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Delete
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Value
.

```yaml
Type: String[]
Parameter Sets: DeleteExpanded
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

### Microsoft.Graph.PowerShell.Models.IPaths1Jddi17SecurityTiindicatorsMicrosoftGraphDeletetiindicatorsbyexternalidPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphResultInfo
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IPaths1Jddi17SecurityTiindicatorsMicrosoftGraphDeletetiindicatorsbyexternalidPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Value <String[]>]`: 

## RELATED LINKS
