---
external help file: Microsoft.Graph.People-help.xml
Module Name: Microsoft.Graph.People
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.people/new-mguserprofileeducationalactivity
schema: 2.0.0
---

# New-MgUserProfileEducationalActivity

## SYNOPSIS
Create a new educationalActivity in a user's profile.

## SYNTAX

### CreateExpanded (Default)
```
New-MgUserProfileEducationalActivity -UserId <String> [-AdditionalProperties <Hashtable>]
 [-AllowedAudiences <String>] [-CompletionMonthYear <DateTime>] [-CreatedBy <IMicrosoftGraphIdentitySet>]
 [-CreatedDateTime <DateTime>] [-EndMonthYear <DateTime>] [-Id <String>]
 [-Inference <IMicrosoftGraphInferenceData>] [-Institution <IMicrosoftGraphInstitutionData>] [-IsSearchable]
 [-LastModifiedBy <IMicrosoftGraphIdentitySet>] [-LastModifiedDateTime <DateTime>]
 [-Program <IMicrosoftGraphEducationalActivityDetail>] [-Source <IMicrosoftGraphPersonDataSources>]
 [-StartMonthYear <DateTime>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgUserProfileEducationalActivity -UserId <String> -BodyParameter <IMicrosoftGraphEducationalActivity>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgUserProfileEducationalActivity -InputObject <IPeopleIdentity> [-AdditionalProperties <Hashtable>]
 [-AllowedAudiences <String>] [-CompletionMonthYear <DateTime>] [-CreatedBy <IMicrosoftGraphIdentitySet>]
 [-CreatedDateTime <DateTime>] [-EndMonthYear <DateTime>] [-Id <String>]
 [-Inference <IMicrosoftGraphInferenceData>] [-Institution <IMicrosoftGraphInstitutionData>] [-IsSearchable]
 [-LastModifiedBy <IMicrosoftGraphIdentitySet>] [-LastModifiedDateTime <DateTime>]
 [-Program <IMicrosoftGraphEducationalActivityDetail>] [-Source <IMicrosoftGraphPersonDataSources>]
 [-StartMonthYear <DateTime>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgUserProfileEducationalActivity -InputObject <IPeopleIdentity>
 -BodyParameter <IMicrosoftGraphEducationalActivity> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new educationalActivity in a user's profile.

## EXAMPLES

### Example 1: Using the New-MgUserProfileEducationalActivity Cmdlet
```powershell
Import-Module Microsoft.Graph.People
$params = @{
	CompletionMonthYear = "Date"
	EndMonthYear = "Date"
	Institution = @{
		Description = $null
		DisplayName = "Colorado State University"
		Location = @{
			Type = "business"
			PostOfficeBox = $null
			Street = "12000 E Prospect Rd"
			City = "Fort Collins"
			State = "Colorado"
			CountryOrRegion = "USA"
			PostalCode = "80525"
		}
		WebUrl = "https://www.colostate.edu"
	}
	Program = @{
		Abbreviation = "MBA"
		Activities = $null
		Awards = $null
		Description = "Master of Business Administration with a major in Entreprenuership and Finance."
		DisplayName = "Master of Business Administration"
		FieldsOfStudy = $null
		Grade = "3.9"
		Notes = $null
		WebUrl = "https://biz.colostate.edu"
	}
	StartMonthYear = "Date"
}
# A UPN can also be used as -UserId.
New-MgUserProfileEducationalActivity -UserId $userId -BodyParameter $params
```

This example shows how to use the New-MgUserProfileEducationalActivity Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
educationalActivity
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphEducationalActivity
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CompletionMonthYear
The month and year the user graduated or completed the activity.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreatedBy
identitySet
To construct, please use Get-Help -Online and see NOTES section for CREATEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentitySet
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EndMonthYear
The month and year the user completed the educational activity referenced.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Institution
institutionData
To construct, please use Get-Help -Online and see NOTES section for INSTITUTION properties and create a hash table.

```yaml
Type: IMicrosoftGraphInstitutionData
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsSearchable
.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Program
educationalActivityDetail
To construct, please use Get-Help -Online and see NOTES section for PROGRAM properties and create a hash table.

```yaml
Type: IMicrosoftGraphEducationalActivityDetail
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartMonthYear
The month and year the user commenced the activity referenced.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, Create
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphEducationalActivity
### Microsoft.Graph.PowerShell.Models.IPeopleIdentity
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphEducationalActivity
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IMicrosoftGraphEducationalActivity>`: educationalActivity
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
  - `[CompletionMonthYear <DateTime?>]`: The month and year the user graduated or completed the activity.
  - `[EndMonthYear <DateTime?>]`: The month and year the user completed the educational activity referenced.
  - `[Institution <IMicrosoftGraphInstitutionData>]`: institutionData
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Description <String>]`: Short description of the institution the user studied at.
    - `[DisplayName <String>]`: Name of the institution the user studied at.
    - `[Location <IMicrosoftGraphPhysicalAddress1>]`: physicalAddress
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[City <String>]`: The city.
      - `[CountryOrRegion <String>]`: The country or region. It's a free-format string value, for example, 'United States'.
      - `[PostOfficeBox <String>]`: The post office box number.
      - `[PostalCode <String>]`: The postal code.
      - `[State <String>]`: The state.
      - `[Street <String>]`: The street.
      - `[Type <String>]`: physicalAddressType
    - `[WebUrl <String>]`: Link to the institution or department homepage.
  - `[Program <IMicrosoftGraphEducationalActivityDetail>]`: educationalActivityDetail
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Abbreviation <String>]`: Shortened name of the degree or program (example: PhD, MBA)
    - `[Activities <String[]>]`: Extracurricular activities undertaken alongside the program.
    - `[Awards <String[]>]`: Any awards or honors associated with the program.
    - `[Description <String>]`: Short description of the program provided by the user.
    - `[DisplayName <String>]`: Long-form name of the program that the user has provided.
    - `[FieldsOfStudy <String[]>]`: Majors and minors associated with the program. (if applicable)
    - `[Grade <String>]`: The final grade, class, GPA or score.
    - `[Notes <String>]`: Additional notes the user has provided.
    - `[WebUrl <String>]`: Link to the degree or program page.
  - `[StartMonthYear <DateTime?>]`: The month and year the user commenced the activity referenced.

CREATEDBY `<IMicrosoftGraphIdentitySet>`: identitySet
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Application <IMicrosoftGraphIdentity>]`: identity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity. This property is read-only.
    - `[Id <String>]`: The identifier of the identity. This property is read-only.
  - `[Device <IMicrosoftGraphIdentity>]`: identity
  - `[User <IMicrosoftGraphIdentity>]`: identity

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

INSTITUTION `<IMicrosoftGraphInstitutionData>`: institutionData
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Description <String>]`: Short description of the institution the user studied at.
  - `[DisplayName <String>]`: Name of the institution the user studied at.
  - `[Location <IMicrosoftGraphPhysicalAddress1>]`: physicalAddress
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[City <String>]`: The city.
    - `[CountryOrRegion <String>]`: The country or region. It's a free-format string value, for example, 'United States'.
    - `[PostOfficeBox <String>]`: The post office box number.
    - `[PostalCode <String>]`: The postal code.
    - `[State <String>]`: The state.
    - `[Street <String>]`: The street.
    - `[Type <String>]`: physicalAddressType
  - `[WebUrl <String>]`: Link to the institution or department homepage.

LASTMODIFIEDBY `<IMicrosoftGraphIdentitySet>`: identitySet
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Application <IMicrosoftGraphIdentity>]`: identity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity. This property is read-only.
    - `[Id <String>]`: The identifier of the identity. This property is read-only.
  - `[Device <IMicrosoftGraphIdentity>]`: identity
  - `[User <IMicrosoftGraphIdentity>]`: identity

PROGRAM `<IMicrosoftGraphEducationalActivityDetail>`: educationalActivityDetail
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Abbreviation <String>]`: Shortened name of the degree or program (example: PhD, MBA)
  - `[Activities <String[]>]`: Extracurricular activities undertaken alongside the program.
  - `[Awards <String[]>]`: Any awards or honors associated with the program.
  - `[Description <String>]`: Short description of the program provided by the user.
  - `[DisplayName <String>]`: Long-form name of the program that the user has provided.
  - `[FieldsOfStudy <String[]>]`: Majors and minors associated with the program. (if applicable)
  - `[Grade <String>]`: The final grade, class, GPA or score.
  - `[Notes <String>]`: Additional notes the user has provided.
  - `[WebUrl <String>]`: Link to the degree or program page.

SOURCE `<IMicrosoftGraphPersonDataSources>`: personDataSources
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Type <String[]>]`: 

## RELATED LINKS
