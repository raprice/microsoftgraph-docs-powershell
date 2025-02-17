---
external help file: Microsoft.Graph.Compliance-help.xml
Module Name: Microsoft.Graph.Compliance
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.compliance/add-mgcomplianceediscoverycasecustodianhold
schema: 2.0.0
---

# Add-MgComplianceEdiscoveryCaseCustodianHold

## SYNOPSIS
Invoke action applyHold

## SYNTAX

### ApplyExpanded (Default)
```
Add-MgComplianceEdiscoveryCaseCustodianHold -CaseId <String> [-AdditionalProperties <Hashtable>]
 [-Ids <String[]>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Apply1
```
Add-MgComplianceEdiscoveryCaseCustodianHold -CaseId <String>
 -BodyParameter <IPathsWwm7HsComplianceEdiscoveryCasesCaseIdCustodiansMicrosoftGraphEdiscoveryApplyholdPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Apply
```
Add-MgComplianceEdiscoveryCaseCustodianHold -CaseId <String> -CustodianId <String> [-PassThru] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### ApplyViaIdentityExpanded
```
Add-MgComplianceEdiscoveryCaseCustodianHold -InputObject <IComplianceIdentity>
 [-AdditionalProperties <Hashtable>] [-Ids <String[]>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ApplyViaIdentity1
```
Add-MgComplianceEdiscoveryCaseCustodianHold -InputObject <IComplianceIdentity>
 -BodyParameter <IPathsWwm7HsComplianceEdiscoveryCasesCaseIdCustodiansMicrosoftGraphEdiscoveryApplyholdPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ApplyViaIdentity
```
Add-MgComplianceEdiscoveryCaseCustodianHold -InputObject <IComplianceIdentity> [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Invoke action applyHold

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: ApplyExpanded, ApplyViaIdentityExpanded
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
Type: IPathsWwm7HsComplianceEdiscoveryCasesCaseIdCustodiansMicrosoftGraphEdiscoveryApplyholdPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Apply1, ApplyViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CaseId
key: id of case

```yaml
Type: String
Parameter Sets: ApplyExpanded, Apply1, Apply
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CustodianId
key: id of custodian

```yaml
Type: String
Parameter Sets: Apply
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Ids
.

```yaml
Type: String[]
Parameter Sets: ApplyExpanded, ApplyViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, please use Get-Help -Online and see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IComplianceIdentity
Parameter Sets: ApplyViaIdentityExpanded, ApplyViaIdentity1, ApplyViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

### Microsoft.Graph.PowerShell.Models.IComplianceIdentity
### Microsoft.Graph.PowerShell.Models.IPathsWwm7HsComplianceEdiscoveryCasesCaseIdCustodiansMicrosoftGraphEdiscoveryApplyholdPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IPathsWwm7HsComplianceEdiscoveryCasesCaseIdCustodiansMicrosoftGraphEdiscoveryApplyholdPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Ids <String[]>]`: 

INPUTOBJECT `<IComplianceIdentity>`: Identity Parameter
  - `[CaseId <String>]`: key: id of case
  - `[CaseOperationId <String>]`: key: id of caseOperation
  - `[CustodianId <String>]`: key: id of custodian
  - `[DataSourceId <String>]`: key: id of dataSource
  - `[LegalHoldId <String>]`: key: id of legalHold
  - `[NoncustodialDataSourceId <String>]`: key: id of noncustodialDataSource
  - `[ReviewSetId <String>]`: key: id of reviewSet
  - `[ReviewSetQueryId <String>]`: key: id of reviewSetQuery
  - `[SiteSourceId <String>]`: key: id of siteSource
  - `[SourceCollectionId <String>]`: key: id of sourceCollection
  - `[TagId <String>]`: key: id of tag
  - `[TagId1 <String>]`: key: id of tag
  - `[UnifiedGroupSourceId <String>]`: key: id of unifiedGroupSource
  - `[UserSourceId <String>]`: key: id of userSource

## RELATED LINKS
