---
external help file: Microsoft.Graph.PersonalContacts-help.xml
Module Name: Microsoft.Graph.PersonalContacts
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.personalcontacts/new-mgusercontactfolderchildfolder
schema: 2.0.0
ms.prod: "outlook"
---

# New-MgUserContactFolderChildFolder

## SYNOPSIS
Create a new contactFolder as a child of a specified folder.
You can also create a new contactFolder under the user's default contact folder.

## SYNTAX

### CreateExpanded1 (Default)
```
New-MgUserContactFolderChildFolder -ContactFolderId <String> -UserId <String>
 [-AdditionalProperties <Hashtable>] [-ChildFolders <IMicrosoftGraphContactFolder1[]>]
 [-Contacts <IMicrosoftGraphContact1[]>] [-DisplayName <String>] [-Id <String>]
 [-MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty[]>] [-ParentFolderId <String>]
 [-SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty[]>]
 [-WellKnownName <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create1
```
New-MgUserContactFolderChildFolder -ContactFolderId <String> -UserId <String>
 -BodyParameter <IMicrosoftGraphContactFolder1> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded1
```
New-MgUserContactFolderChildFolder -InputObject <IPersonalContactsIdentity> [-AdditionalProperties <Hashtable>]
 [-ChildFolders <IMicrosoftGraphContactFolder1[]>] [-Contacts <IMicrosoftGraphContact1[]>]
 [-DisplayName <String>] [-Id <String>]
 [-MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty[]>] [-ParentFolderId <String>]
 [-SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty[]>]
 [-WellKnownName <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity1
```
New-MgUserContactFolderChildFolder -InputObject <IPersonalContactsIdentity>
 -BodyParameter <IMicrosoftGraphContactFolder1> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new contactFolder as a child of a specified folder.
You can also create a new contactFolder under the user's default contact folder.

## EXAMPLES

### Example 1: Using the New-MgUserContactFolderChildFolder Cmdlet
```powershell
Import-Module Microsoft.Graph.PersonalContacts
$params = @{
	DisplayName = "Family"
}
# A UPN can also be used as -UserId.
New-MgUserContactFolderChildFolder -UserId $userId -ContactFolderId $contactFolderId -BodyParameter $params
```

This example shows how to use the New-MgUserContactFolderChildFolder Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
contactFolder
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphContactFolder1
Parameter Sets: Create1, CreateViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ChildFolders
The collection of child folders in the folder.
Navigation property.
Read-only.
Nullable.
To construct, please use Get-Help -Online and see NOTES section for CHILDFOLDERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphContactFolder1[]
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ContactFolderId
key: id of contactFolder

```yaml
Type: String
Parameter Sets: CreateExpanded1, Create1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Contacts
The contacts in the folder.
Navigation property.
Read-only.
Nullable.
To construct, please use Get-Help -Online and see NOTES section for CONTACTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphContact1[]
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
The folder's display name.

```yaml
Type: String
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
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
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
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
Type: IPersonalContactsIdentity
Parameter Sets: CreateViaIdentityExpanded1, CreateViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MultiValueExtendedProperties
The collection of multi-value extended properties defined for the contactFolder.
Read-only.
Nullable.
To construct, please use Get-Help -Online and see NOTES section for MULTIVALUEEXTENDEDPROPERTIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphMultiValueLegacyExtendedProperty[]
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ParentFolderId
The ID of the folder's parent folder.

```yaml
Type: String
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SingleValueExtendedProperties
The collection of single-value extended properties defined for the contactFolder.
Read-only.
Nullable.
To construct, please use Get-Help -Online and see NOTES section for SINGLEVALUEEXTENDEDPROPERTIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphSingleValueLegacyExtendedProperty[]
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
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
Parameter Sets: CreateExpanded1, Create1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WellKnownName
The name of the folder if the folder is a recognized folder.
Currently contacts is the only recognized contacts folder.

```yaml
Type: String
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphContactFolder1
### Microsoft.Graph.PowerShell.Models.IPersonalContactsIdentity
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphContactFolder1
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IMicrosoftGraphContactFolder1>`: contactFolder
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[ChildFolders <IMicrosoftGraphContactFolder1[]>]`: The collection of child folders in the folder. Navigation property. Read-only. Nullable.
  - `[Contacts <IMicrosoftGraphContact1[]>]`: The contacts in the folder. Navigation property. Read-only. Nullable.
    - `[Categories <String[]>]`: The categories associated with the item
    - `[ChangeKey <String>]`: Identifies the version of the item. Every time the item is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.
    - `[CreatedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[LastModifiedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[AssistantName <String>]`: The name of the contact's assistant.
    - `[Birthday <DateTime?>]`: The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[Children <String[]>]`: The names of the contact's children.
    - `[CompanyName <String>]`: The name of the contact's company.
    - `[Department <String>]`: The contact's department.
    - `[DisplayName <String>]`: The contact's display name. You can specify the display name in a create or update operation. Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified. To preserve a pre-existing value, always include it as displayName in an update operation.
    - `[EmailAddresses <IMicrosoftGraphTypedEmailAddress[]>]`: The contact's email addresses.
      - `[Address <String>]`: The email address of the person or entity.
      - `[Name <String>]`: The display name of the person or entity.
      - `[OtherLabel <String>]`: To specify a custom type of email address, set type to other, and assign otherLabel to a custom string. For example, you may use a specific email address for your volunteer activities. Set type to other, and set otherLabel to a custom string such as Volunteer work.
      - `[Type <String>]`: emailType
    - `[Extensions <IMicrosoftGraphExtension[]>]`: The collection of open extensions defined for the contact. Nullable.
      - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[FileAs <String>]`: The name the contact is filed under.
    - `[Flag <IMicrosoftGraphFollowupFlag>]`: followupFlag
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[CompletedDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}). For example, '2019-04-16T09:00:00'.
        - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'. See below for possible values.
      - `[DueDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
      - `[FlagStatus <String>]`: followupFlagStatus
      - `[StartDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
    - `[Gender <String>]`: The contact's gender.
    - `[Generation <String>]`: The contact's generation.
    - `[GivenName <String>]`: The contact's given name.
    - `[ImAddresses <String[]>]`: 
    - `[Initials <String>]`: 
    - `[IsFavorite <Boolean?>]`: 
    - `[JobTitle <String>]`: 
    - `[Manager <String>]`: 
    - `[MiddleName <String>]`: 
    - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty[]>]`: The collection of multi-value extended properties defined for the contact. Read-only. Nullable.
      - `[Id <String>]`: The unique idenfier for an entity. Read-only.
      - `[Value <String[]>]`: A collection of property values.
    - `[NickName <String>]`: 
    - `[OfficeLocation <String>]`: 
    - `[ParentFolderId <String>]`: 
    - `[PersonalNotes <String>]`: 
    - `[Phones <IMicrosoftGraphPhone[]>]`: 
      - `[Number <String>]`: The phone number.
      - `[Type <String>]`: phoneType
    - `[Photo <IMicrosoftGraphProfilePhoto>]`: profilePhoto
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique idenfier for an entity. Read-only.
      - `[Height <Int32?>]`: The height of the photo. Read-only.
      - `[Width <Int32?>]`: The width of the photo. Read-only.
    - `[PostalAddresses <IMicrosoftGraphPhysicalAddress1[]>]`: 
      - `[City <String>]`: The city.
      - `[CountryOrRegion <String>]`: The country or region. It's a free-format string value, for example, 'United States'.
      - `[PostOfficeBox <String>]`: The post office box number.
      - `[PostalCode <String>]`: The postal code.
      - `[State <String>]`: The state.
      - `[Street <String>]`: The street.
      - `[Type <String>]`: physicalAddressType
    - `[Profession <String>]`: 
    - `[SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty[]>]`: The collection of single-value extended properties defined for the contact. Read-only. Nullable.
      - `[Id <String>]`: The unique idenfier for an entity. Read-only.
      - `[Value <String>]`: A property value.
    - `[SpouseName <String>]`: 
    - `[Surname <String>]`: 
    - `[Title <String>]`: 
    - `[Websites <IMicrosoftGraphWebsite[]>]`: 
      - `[Address <String>]`: The URL of the website.
      - `[DisplayName <String>]`: The display name of the web site.
      - `[Type <String>]`: websiteType
    - `[WeddingAnniversary <DateTime?>]`: 
    - `[YomiCompanyName <String>]`: 
    - `[YomiGivenName <String>]`: 
    - `[YomiSurname <String>]`: 
  - `[DisplayName <String>]`: The folder's display name.
  - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty[]>]`: The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.
  - `[ParentFolderId <String>]`: The ID of the folder's parent folder.
  - `[SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty[]>]`: The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.
  - `[WellKnownName <String>]`: The name of the folder if the folder is a recognized folder. Currently contacts is the only recognized contacts folder.

CHILDFOLDERS <IMicrosoftGraphContactFolder1\[]>: The collection of child folders in the folder. Navigation property. Read-only. Nullable.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[ChildFolders <IMicrosoftGraphContactFolder1[]>]`: The collection of child folders in the folder. Navigation property. Read-only. Nullable.
  - `[Contacts <IMicrosoftGraphContact1[]>]`: The contacts in the folder. Navigation property. Read-only. Nullable.
    - `[Categories <String[]>]`: The categories associated with the item
    - `[ChangeKey <String>]`: Identifies the version of the item. Every time the item is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.
    - `[CreatedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[LastModifiedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[AssistantName <String>]`: The name of the contact's assistant.
    - `[Birthday <DateTime?>]`: The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[Children <String[]>]`: The names of the contact's children.
    - `[CompanyName <String>]`: The name of the contact's company.
    - `[Department <String>]`: The contact's department.
    - `[DisplayName <String>]`: The contact's display name. You can specify the display name in a create or update operation. Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified. To preserve a pre-existing value, always include it as displayName in an update operation.
    - `[EmailAddresses <IMicrosoftGraphTypedEmailAddress[]>]`: The contact's email addresses.
      - `[Address <String>]`: The email address of the person or entity.
      - `[Name <String>]`: The display name of the person or entity.
      - `[OtherLabel <String>]`: To specify a custom type of email address, set type to other, and assign otherLabel to a custom string. For example, you may use a specific email address for your volunteer activities. Set type to other, and set otherLabel to a custom string such as Volunteer work.
      - `[Type <String>]`: emailType
    - `[Extensions <IMicrosoftGraphExtension[]>]`: The collection of open extensions defined for the contact. Nullable.
      - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[FileAs <String>]`: The name the contact is filed under.
    - `[Flag <IMicrosoftGraphFollowupFlag>]`: followupFlag
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[CompletedDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}). For example, '2019-04-16T09:00:00'.
        - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'. See below for possible values.
      - `[DueDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
      - `[FlagStatus <String>]`: followupFlagStatus
      - `[StartDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
    - `[Gender <String>]`: The contact's gender.
    - `[Generation <String>]`: The contact's generation.
    - `[GivenName <String>]`: The contact's given name.
    - `[ImAddresses <String[]>]`: 
    - `[Initials <String>]`: 
    - `[IsFavorite <Boolean?>]`: 
    - `[JobTitle <String>]`: 
    - `[Manager <String>]`: 
    - `[MiddleName <String>]`: 
    - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty[]>]`: The collection of multi-value extended properties defined for the contact. Read-only. Nullable.
      - `[Id <String>]`: The unique idenfier for an entity. Read-only.
      - `[Value <String[]>]`: A collection of property values.
    - `[NickName <String>]`: 
    - `[OfficeLocation <String>]`: 
    - `[ParentFolderId <String>]`: 
    - `[PersonalNotes <String>]`: 
    - `[Phones <IMicrosoftGraphPhone[]>]`: 
      - `[Number <String>]`: The phone number.
      - `[Type <String>]`: phoneType
    - `[Photo <IMicrosoftGraphProfilePhoto>]`: profilePhoto
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique idenfier for an entity. Read-only.
      - `[Height <Int32?>]`: The height of the photo. Read-only.
      - `[Width <Int32?>]`: The width of the photo. Read-only.
    - `[PostalAddresses <IMicrosoftGraphPhysicalAddress1[]>]`: 
      - `[City <String>]`: The city.
      - `[CountryOrRegion <String>]`: The country or region. It's a free-format string value, for example, 'United States'.
      - `[PostOfficeBox <String>]`: The post office box number.
      - `[PostalCode <String>]`: The postal code.
      - `[State <String>]`: The state.
      - `[Street <String>]`: The street.
      - `[Type <String>]`: physicalAddressType
    - `[Profession <String>]`: 
    - `[SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty[]>]`: The collection of single-value extended properties defined for the contact. Read-only. Nullable.
      - `[Id <String>]`: The unique idenfier for an entity. Read-only.
      - `[Value <String>]`: A property value.
    - `[SpouseName <String>]`: 
    - `[Surname <String>]`: 
    - `[Title <String>]`: 
    - `[Websites <IMicrosoftGraphWebsite[]>]`: 
      - `[Address <String>]`: The URL of the website.
      - `[DisplayName <String>]`: The display name of the web site.
      - `[Type <String>]`: websiteType
    - `[WeddingAnniversary <DateTime?>]`: 
    - `[YomiCompanyName <String>]`: 
    - `[YomiGivenName <String>]`: 
    - `[YomiSurname <String>]`: 
  - `[DisplayName <String>]`: The folder's display name.
  - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty[]>]`: The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.
  - `[ParentFolderId <String>]`: The ID of the folder's parent folder.
  - `[SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty[]>]`: The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.
  - `[WellKnownName <String>]`: The name of the folder if the folder is a recognized folder. Currently contacts is the only recognized contacts folder.

CONTACTS <IMicrosoftGraphContact1\[]>: The contacts in the folder. Navigation property. Read-only. Nullable.
  - `[Categories <String[]>]`: The categories associated with the item
  - `[ChangeKey <String>]`: Identifies the version of the item. Every time the item is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.
  - `[CreatedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[LastModifiedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[AssistantName <String>]`: The name of the contact's assistant.
  - `[Birthday <DateTime?>]`: The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[Children <String[]>]`: The names of the contact's children.
  - `[CompanyName <String>]`: The name of the contact's company.
  - `[Department <String>]`: The contact's department.
  - `[DisplayName <String>]`: The contact's display name. You can specify the display name in a create or update operation. Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified. To preserve a pre-existing value, always include it as displayName in an update operation.
  - `[EmailAddresses <IMicrosoftGraphTypedEmailAddress[]>]`: The contact's email addresses.
    - `[Address <String>]`: The email address of the person or entity.
    - `[Name <String>]`: The display name of the person or entity.
    - `[OtherLabel <String>]`: To specify a custom type of email address, set type to other, and assign otherLabel to a custom string. For example, you may use a specific email address for your volunteer activities. Set type to other, and set otherLabel to a custom string such as Volunteer work.
    - `[Type <String>]`: emailType
  - `[Extensions <IMicrosoftGraphExtension[]>]`: The collection of open extensions defined for the contact. Nullable.
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[FileAs <String>]`: The name the contact is filed under.
  - `[Flag <IMicrosoftGraphFollowupFlag>]`: followupFlag
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[CompletedDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}). For example, '2019-04-16T09:00:00'.
      - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'. See below for possible values.
    - `[DueDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
    - `[FlagStatus <String>]`: followupFlagStatus
    - `[StartDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
  - `[Gender <String>]`: The contact's gender.
  - `[Generation <String>]`: The contact's generation.
  - `[GivenName <String>]`: The contact's given name.
  - `[ImAddresses <String[]>]`: 
  - `[Initials <String>]`: 
  - `[IsFavorite <Boolean?>]`: 
  - `[JobTitle <String>]`: 
  - `[Manager <String>]`: 
  - `[MiddleName <String>]`: 
  - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty[]>]`: The collection of multi-value extended properties defined for the contact. Read-only. Nullable.
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[Value <String[]>]`: A collection of property values.
  - `[NickName <String>]`: 
  - `[OfficeLocation <String>]`: 
  - `[ParentFolderId <String>]`: 
  - `[PersonalNotes <String>]`: 
  - `[Phones <IMicrosoftGraphPhone[]>]`: 
    - `[Number <String>]`: The phone number.
    - `[Type <String>]`: phoneType
  - `[Photo <IMicrosoftGraphProfilePhoto>]`: profilePhoto
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[Height <Int32?>]`: The height of the photo. Read-only.
    - `[Width <Int32?>]`: The width of the photo. Read-only.
  - `[PostalAddresses <IMicrosoftGraphPhysicalAddress1[]>]`: 
    - `[City <String>]`: The city.
    - `[CountryOrRegion <String>]`: The country or region. It's a free-format string value, for example, 'United States'.
    - `[PostOfficeBox <String>]`: The post office box number.
    - `[PostalCode <String>]`: The postal code.
    - `[State <String>]`: The state.
    - `[Street <String>]`: The street.
    - `[Type <String>]`: physicalAddressType
  - `[Profession <String>]`: 
  - `[SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty[]>]`: The collection of single-value extended properties defined for the contact. Read-only. Nullable.
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[Value <String>]`: A property value.
  - `[SpouseName <String>]`: 
  - `[Surname <String>]`: 
  - `[Title <String>]`: 
  - `[Websites <IMicrosoftGraphWebsite[]>]`: 
    - `[Address <String>]`: The URL of the website.
    - `[DisplayName <String>]`: The display name of the web site.
    - `[Type <String>]`: websiteType
  - `[WeddingAnniversary <DateTime?>]`: 
  - `[YomiCompanyName <String>]`: 
  - `[YomiGivenName <String>]`: 
  - `[YomiSurname <String>]`: 

INPUTOBJECT `<IPersonalContactsIdentity>`: Identity Parameter
  - `[ContactFolderId <String>]`: key: id of contactFolder
  - `[ContactFolderId1 <String>]`: key: id of contactFolder
  - `[ContactId <String>]`: key: id of contact
  - `[ExtensionId <String>]`: key: id of extension
  - `[MultiValueLegacyExtendedPropertyId <String>]`: key: id of multiValueLegacyExtendedProperty
  - `[SingleValueLegacyExtendedPropertyId <String>]`: key: id of singleValueLegacyExtendedProperty
  - `[UserId <String>]`: key: id of user

MULTIVALUEEXTENDEDPROPERTIES <IMicrosoftGraphMultiValueLegacyExtendedProperty\[]>: The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[Value <String[]>]`: A collection of property values.

SINGLEVALUEEXTENDEDPROPERTIES <IMicrosoftGraphSingleValueLegacyExtendedProperty\[]>: The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[Value <String>]`: A property value.

## RELATED LINKS

## RELATED LINKS
