---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.identity.signins/get-mgidentitycontinuouaccessevaluationpolicy
schema: 2.0.0
---

# Get-MgIdentityContinuouAccessEvaluationPolicy

## SYNOPSIS
Read the properties and relationships of a continuousAccessEvaluationPolicy object.

## SYNTAX

```
Get-MgIdentityContinuouAccessEvaluationPolicy [-ExpandProperty <String[]>] [-Property <String[]>]
 [<CommonParameters>]
```

## DESCRIPTION
Read the properties and relationships of a continuousAccessEvaluationPolicy object.

## EXAMPLES

### Example 1: Using the Get-MgIdentityContinuouAccessEvaluationPolicy Cmdlet
```powershell
Import-Module Microsoft.Graph.Identity.SignIns
Get-MgIdentityContinuouAccessEvaluationPolicy
```

This example shows how to use the Get-MgIdentityContinuouAccessEvaluationPolicy Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -ExpandProperty
Expand related entities

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Expand

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Property
Select properties to be returned

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Select

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphContinuousAccessEvaluationPolicy
## NOTES

ALIASES

## RELATED LINKS
