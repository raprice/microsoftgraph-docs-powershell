---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.identity.signins/update-mginformationprotection
schema: 2.0.0
---

# Update-MgInformationProtection

## SYNOPSIS
Update informationProtection

## SYNTAX

### UpdateExpanded1 (Default)
```
Update-MgInformationProtection [-AdditionalProperties <Hashtable>] [-Bitlocker <IMicrosoftGraphBitlocker>]
 [-Id <String>] [-ThreatAssessmentRequests <IMicrosoftGraphThreatAssessmentRequest[]>] [-PassThru] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Update1
```
Update-MgInformationProtection -BodyParameter <IMicrosoftGraphInformationProtection1> [-PassThru] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update informationProtection

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Bitlocker
bitlocker
To construct, please use Get-Help -Online and see NOTES section for BITLOCKER properties and create a hash table.

```yaml
Type: IMicrosoftGraphBitlocker
Parameter Sets: UpdateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
informationProtection
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphInformationProtection1
Parameter Sets: Update1
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
Parameter Sets: UpdateExpanded1
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

### -ThreatAssessmentRequests
.
To construct, please use Get-Help -Online and see NOTES section for THREATASSESSMENTREQUESTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphThreatAssessmentRequest[]
Parameter Sets: UpdateExpanded1
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphInformationProtection1
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BITLOCKER `<IMicrosoftGraphBitlocker>`: bitlocker
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[RecoveryKeys <IMicrosoftGraphBitlockerRecoveryKey[]>]`: The recovery keys associated with the bitlocker entity.
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[CreatedDateTime <DateTime?>]`: The date and time when the key was originally backed up to Azure Active Directory. Not nullable.
    - `[DeviceId <String>]`: Identifier of the device the BitLocker key is originally backed up from. Supports $filter (eq).
    - `[Key <String>]`: The BitLocker recovery key. Returned only on $select. Not nullable.
    - `[VolumeType <String>]`: volumeType

BODYPARAMETER `<IMicrosoftGraphInformationProtection>`: informationProtection
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Bitlocker <IMicrosoftGraphBitlocker>]`: bitlocker
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[RecoveryKeys <IMicrosoftGraphBitlockerRecoveryKey[]>]`: The recovery keys associated with the bitlocker entity.
      - `[Id <String>]`: The unique idenfier for an entity. Read-only.
      - `[CreatedDateTime <DateTime?>]`: The date and time when the key was originally backed up to Azure Active Directory. Not nullable.
      - `[DeviceId <String>]`: Identifier of the device the BitLocker key is originally backed up from. Supports $filter (eq).
      - `[Key <String>]`: The BitLocker recovery key. Returned only on $select. Not nullable.
      - `[VolumeType <String>]`: volumeType
  - `[ThreatAssessmentRequests <IMicrosoftGraphThreatAssessmentRequest[]>]`: 
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[Category <String>]`: threatCategory
    - `[ContentType <String>]`: threatAssessmentContentType
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Application <IMicrosoftGraphIdentity>]`: identity
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
        - `[Id <String>]`: Unique identifier for the identity.
      - `[Device <IMicrosoftGraphIdentity>]`: identity
      - `[User <IMicrosoftGraphIdentity>]`: identity
    - `[CreatedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[ExpectedAssessment <String>]`: threatExpectedAssessment
    - `[RequestSource <String>]`: threatAssessmentRequestSource
    - `[Results <IMicrosoftGraphThreatAssessmentResult[]>]`: A collection of threat assessment results. Read-only. By default, a GET /threatAssessmentRequests/{id} does not return this property unless you apply $expand on it.
      - `[Id <String>]`: The unique idenfier for an entity. Read-only.
      - `[CreatedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
      - `[Message <String>]`: The result message for each threat assessment.
      - `[ResultType <String>]`: threatAssessmentResultType
    - `[Status <String>]`: threatAssessmentStatus

THREATASSESSMENTREQUESTS <IMicrosoftGraphThreatAssessmentRequest\[]>: .
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[Category <String>]`: threatCategory
  - `[ContentType <String>]`: threatAssessmentContentType
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[CreatedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[ExpectedAssessment <String>]`: threatExpectedAssessment
  - `[RequestSource <String>]`: threatAssessmentRequestSource
  - `[Results <IMicrosoftGraphThreatAssessmentResult[]>]`: A collection of threat assessment results. Read-only. By default, a GET /threatAssessmentRequests/{id} does not return this property unless you apply $expand on it.
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[CreatedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[Message <String>]`: The result message for each threat assessment.
    - `[ResultType <String>]`: threatAssessmentResultType
  - `[Status <String>]`: threatAssessmentStatus

## RELATED LINKS
