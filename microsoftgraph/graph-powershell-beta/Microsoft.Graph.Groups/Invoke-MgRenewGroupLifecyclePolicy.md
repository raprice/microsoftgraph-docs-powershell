---
external help file: Microsoft.Graph.Groups-help.xml
Module Name: Microsoft.Graph.Groups
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.groups/invoke-mgrenewgrouplifecyclepolicy
schema: 2.0.0
---

# Invoke-MgRenewGroupLifecyclePolicy

## SYNOPSIS
Renew a group's expiration.
When a group is renewed, the group expiration is extended by the number of days defined in the policy.

## SYNTAX

### RenewExpanded (Default)
```
Invoke-MgRenewGroupLifecyclePolicy [-AdditionalProperties <Hashtable>] [-GroupId <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Renew
```
Invoke-MgRenewGroupLifecyclePolicy
 -BodyParameter <IPaths8F8L4QGrouplifecyclepoliciesMicrosoftGraphRenewgroupPostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Renew a group's expiration.
When a group is renewed, the group expiration is extended by the number of days defined in the policy.

## EXAMPLES

### Example 1: Using the Invoke-MgRenewGroupLifecyclePolicy Cmdlet
```powershell
Import-Module Microsoft.Graph.Groups
$params = @{
	GroupId = "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
Invoke-MgRenewGroupLifecyclePolicy -BodyParameter $params
```

This example shows how to use the Invoke-MgRenewGroupLifecyclePolicy Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: RenewExpanded
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
Type: IPaths8F8L4QGrouplifecyclepoliciesMicrosoftGraphRenewgroupPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Renew
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -GroupId
.

```yaml
Type: String
Parameter Sets: RenewExpanded
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

### Microsoft.Graph.PowerShell.Models.IPaths8F8L4QGrouplifecyclepoliciesMicrosoftGraphRenewgroupPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IPaths8F8L4QGrouplifecyclepoliciesMicrosoftGraphRenewgroupPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[GroupId <String>]`: 

## RELATED LINKS
