---
external help file: Microsoft.Graph.Reports-help.xml
Module Name: Microsoft.Graph.Reports
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.reports/get-mgreportattacksimulationusercoverage
schema: 2.0.0
---

# Get-MgReportAttackSimulationUserCoverage

## SYNOPSIS
Invoke function getAttackSimulationSimulationUserCoverage

## SYNTAX

```
Get-MgReportAttackSimulationUserCoverage [-Count] [-Filter <String>] [-Search <String>] [-Skip <Int32>]
 [-Top <Int32>] [<CommonParameters>]
```

## DESCRIPTION
Invoke function getAttackSimulationSimulationUserCoverage

## EXAMPLES

### Example 1: Using the Get-MgReportAttackSimulationUserCoverage Cmdlet
```powershell
Import-Module Microsoft.Graph.Reports
Get-MgReportAttackSimulationUserCoverage
```

This example shows how to use the Get-MgReportAttackSimulationUserCoverage Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -Count
Include count of items

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

### -Filter
Filter items by property values

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Search
Search items by search phrases

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Top
Show only the first n items

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: Limit

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Skip
Skip the first n items

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAttackSimulationUserCoverage
## NOTES

ALIASES

## RELATED LINKS
