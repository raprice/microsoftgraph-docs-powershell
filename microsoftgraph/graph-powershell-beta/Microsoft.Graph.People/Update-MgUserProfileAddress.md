---
external help file: Microsoft.Graph.People-help.xml
Module Name: Microsoft.Graph.People
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.people/update-mguserprofileaddress
schema: 2.0.0
---

# Update-MgUserProfileAddress

## SYNOPSIS
Update the navigation property addresses in users

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgUserProfileAddress -ItemAddressId <String> -UserId <String> [-AdditionalProperties <Hashtable>]
 [-AllowedAudiences <String>] [-CreatedBy <IMicrosoftGraphIdentitySet>] [-CreatedDateTime <DateTime>]
 [-Detail <IMicrosoftGraphPhysicalAddress1>] [-DisplayName <String>]
 [-GeoCoordinates <IMicrosoftGraphGeoCoordinates>] [-Id <String>] [-Inference <IMicrosoftGraphInferenceData>]
 [-IsSearchable] [-LastModifiedBy <IMicrosoftGraphIdentitySet>] [-LastModifiedDateTime <DateTime>]
 [-Source <IMicrosoftGraphPersonDataSources>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgUserProfileAddress -ItemAddressId <String> -UserId <String>
 -BodyParameter <IMicrosoftGraphItemAddress> [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgUserProfileAddress -InputObject <IPeopleIdentity> [-AdditionalProperties <Hashtable>]
 [-AllowedAudiences <String>] [-CreatedBy <IMicrosoftGraphIdentitySet>] [-CreatedDateTime <DateTime>]
 [-Detail <IMicrosoftGraphPhysicalAddress1>] [-DisplayName <String>]
 [-GeoCoordinates <IMicrosoftGraphGeoCoordinates>] [-Id <String>] [-Inference <IMicrosoftGraphInferenceData>]
 [-IsSearchable] [-LastModifiedBy <IMicrosoftGraphIdentitySet>] [-LastModifiedDateTime <DateTime>]
 [-Source <IMicrosoftGraphPersonDataSources>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgUserProfileAddress -InputObject <IPeopleIdentity> -BodyParameter <IMicrosoftGraphItemAddress>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property addresses in users

## EXAMPLES

### Example 1: Using the Update-MgUserProfileAddress Cmdlet
```powershell
Import-Module Microsoft.Graph.People
$params = @{
	AllowedAudiences = "me"
	DisplayName = "Secret Hideout"
}
Update-MgUserProfileAddress -UserId $userId -ItemAddressId $itemAddressId -BodyParameter $params
```

This example shows how to use the Update-MgUserProfileAddress Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowedAudiences
allowedAudiences

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
itemAddress
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphItemAddress
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CreatedBy
identitySet
To construct, please use Get-Help -Online and see NOTES section for CREATEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentitySet
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreatedDateTime
Provides the dateTimeOffset for when the entity was created.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Detail
physicalAddress
To construct, please use Get-Help -Online and see NOTES section for DETAIL properties and create a hash table.

```yaml
Type: IMicrosoftGraphPhysicalAddress1
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
Friendly name the user has assigned to this address.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GeoCoordinates
geoCoordinates
To construct, please use Get-Help -Online and see NOTES section for GEOCOORDINATES properties and create a hash table.

```yaml
Type: IMicrosoftGraphGeoCoordinates
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
The unique idenfier for an entity.
Read-only.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Inference
inferenceData
To construct, please use Get-Help -Online and see NOTES section for INFERENCE properties and create a hash table.

```yaml
Type: IMicrosoftGraphInferenceData
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Type: IPeopleIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsSearchable
.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ItemAddressId
key: id of itemAddress

```yaml
Type: String
Parameter Sets: UpdateExpanded, Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedBy
identitySet
To construct, please use Get-Help -Online and see NOTES section for LASTMODIFIEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentitySet
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedDateTime
Provides the dateTimeOffset for when the entity was created.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### -Source
personDataSources
To construct, please use Get-Help -Online and see NOTES section for SOURCE properties and create a hash table.

```yaml
Type: IMicrosoftGraphPersonDataSources
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserId
key: id of user

```yaml
Type: String
Parameter Sets: UpdateExpanded, Update
Aliases:

Required: True
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphItemAddress
### Microsoft.Graph.PowerShell.Models.IPeopleIdentity
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IMicrosoftGraphItemAddress>`: itemAddress
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AllowedAudiences <String>]`: allowedAudiences
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity. This property is read-only.
      - `[Id <String>]`: The identifier of the identity. This property is read-only.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[CreatedDateTime <DateTime?>]`: Provides the dateTimeOffset for when the entity was created.
  - `[Inference <IMicrosoftGraphInferenceData>]`: inferenceData
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ConfidenceScore <Double?>]`: Confidence score reflecting the accuracy of the data inferred about the user.
    - `[UserHasVerifiedAccuracy <Boolean?>]`: Records if the user has confirmed this inference as being True or False.
  - `[IsSearchable <Boolean?>]`: 
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[LastModifiedDateTime <DateTime?>]`: Provides the dateTimeOffset for when the entity was created.
  - `[Source <IMicrosoftGraphPersonDataSources>]`: personDataSources
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Type <String[]>]`: 
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[Detail <IMicrosoftGraphPhysicalAddress1>]`: physicalAddress
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[City <String>]`: The city.
    - `[CountryOrRegion <String>]`: The country or region. It's a free-format string value, for example, 'United States'.
    - `[PostOfficeBox <String>]`: The post office box number.
    - `[PostalCode <String>]`: The postal code.
    - `[State <String>]`: The state.
    - `[Street <String>]`: The street.
    - `[Type <String>]`: physicalAddressType
  - `[DisplayName <String>]`: Friendly name the user has assigned to this address.
  - `[GeoCoordinates <IMicrosoftGraphGeoCoordinates>]`: geoCoordinates
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Altitude <Double?>]`: Optional. The altitude (height), in feet,  above sea level for the item. Read-only.
    - `[Latitude <Double?>]`: Optional. The latitude, in decimal, for the item. Writable on OneDrive Personal.
    - `[Longitude <Double?>]`: Optional. The longitude, in decimal, for the item. Writable on OneDrive Personal.

CREATEDBY `<IMicrosoftGraphIdentitySet>`: identitySet
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Application <IMicrosoftGraphIdentity>]`: identity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity. This property is read-only.
    - `[Id <String>]`: The identifier of the identity. This property is read-only.
  - `[Device <IMicrosoftGraphIdentity>]`: identity
  - `[User <IMicrosoftGraphIdentity>]`: identity

DETAIL `<IMicrosoftGraphPhysicalAddress1>`: physicalAddress
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[City <String>]`: The city.
  - `[CountryOrRegion <String>]`: The country or region. It's a free-format string value, for example, 'United States'.
  - `[PostOfficeBox <String>]`: The post office box number.
  - `[PostalCode <String>]`: The postal code.
  - `[State <String>]`: The state.
  - `[Street <String>]`: The street.
  - `[Type <String>]`: physicalAddressType

GEOCOORDINATES `<IMicrosoftGraphGeoCoordinates>`: geoCoordinates
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Altitude <Double?>]`: Optional. The altitude (height), in feet,  above sea level for the item. Read-only.
  - `[Latitude <Double?>]`: Optional. The latitude, in decimal, for the item. Writable on OneDrive Personal.
  - `[Longitude <Double?>]`: Optional. The longitude, in decimal, for the item. Writable on OneDrive Personal.

INFERENCE `<IMicrosoftGraphInferenceData>`: inferenceData
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ConfidenceScore <Double?>]`: Confidence score reflecting the accuracy of the data inferred about the user.
  - `[UserHasVerifiedAccuracy <Boolean?>]`: Records if the user has confirmed this inference as being True or False.

INPUTOBJECT `<IPeopleIdentity>`: Identity Parameter
  - `[ActivityStatisticsId <String>]`: key: id of activityStatistics
  - `[EducationalActivityId <String>]`: key: id of educationalActivity
  - `[ItemAddressId <String>]`: key: id of itemAddress
  - `[ItemEmailId <String>]`: key: id of itemEmail
  - `[ItemPatentId <String>]`: key: id of itemPatent
  - `[ItemPhoneId <String>]`: key: id of itemPhone
  - `[ItemPublicationId <String>]`: key: id of itemPublication
  - `[LanguageProficiencyId <String>]`: key: id of languageProficiency
  - `[PersonAnnotationId <String>]`: key: id of personAnnotation
  - `[PersonAnnualEventId <String>]`: key: id of personAnnualEvent
  - `[PersonAwardId <String>]`: key: id of personAward
  - `[PersonCertificationId <String>]`: key: id of personCertification
  - `[PersonId <String>]`: key: id of person
  - `[PersonInterestId <String>]`: key: id of personInterest
  - `[PersonNameId <String>]`: key: id of personName
  - `[PersonWebsiteId <String>]`: key: id of personWebsite
  - `[ProjectParticipationId <String>]`: key: id of projectParticipation
  - `[SharedInsightId <String>]`: key: id of sharedInsight
  - `[SkillProficiencyId <String>]`: key: id of skillProficiency
  - `[TrendingId <String>]`: key: id of trending
  - `[UsedInsightId <String>]`: key: id of usedInsight
  - `[UserAccountInformationId <String>]`: key: id of userAccountInformation
  - `[UserId <String>]`: key: id of user
  - `[WebAccountId <String>]`: key: id of webAccount
  - `[WorkPositionId <String>]`: key: id of workPosition

LASTMODIFIEDBY `<IMicrosoftGraphIdentitySet>`: identitySet
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Application <IMicrosoftGraphIdentity>]`: identity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity. This property is read-only.
    - `[Id <String>]`: The identifier of the identity. This property is read-only.
  - `[Device <IMicrosoftGraphIdentity>]`: identity
  - `[User <IMicrosoftGraphIdentity>]`: identity

SOURCE `<IMicrosoftGraphPersonDataSources>`: personDataSources
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Type <String[]>]`: 

## RELATED LINKS
