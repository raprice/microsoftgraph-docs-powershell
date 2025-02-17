---
external help file: Microsoft.Graph.Groups-help.xml
Module Name: Microsoft.Graph.Groups
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.groups/set-mggrouplicense
schema: 2.0.0
---

# Set-MgGroupLicense

## SYNOPSIS
Add or remove licenses on the group.
Licenses assigned to the group will be assigned to all users in the group.
To learn more about group-based licensing, see What is group-based licensing in Azure Active Directory.
To get the subscriptions available in the directory, perform a GET subscribedSkus request.

## SYNTAX

### AssignExpanded1 (Default)
```
Set-MgGroupLicense -GroupId <String> [-AddLicenses <IMicrosoftGraphAssignedLicense[]>]
 [-AdditionalProperties <Hashtable>] [-RemoveLicenses <String[]>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Assign1
```
Set-MgGroupLicense -GroupId <String>
 -BodyParameter <IPaths6Fg5LiGroupsGroupIdMicrosoftGraphAssignlicensePostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### AssignViaIdentityExpanded1
```
Set-MgGroupLicense -InputObject <IGroupsIdentity> [-AddLicenses <IMicrosoftGraphAssignedLicense[]>]
 [-AdditionalProperties <Hashtable>] [-RemoveLicenses <String[]>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### AssignViaIdentity1
```
Set-MgGroupLicense -InputObject <IGroupsIdentity>
 -BodyParameter <IPaths6Fg5LiGroupsGroupIdMicrosoftGraphAssignlicensePostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Add or remove licenses on the group.
Licenses assigned to the group will be assigned to all users in the group.
To learn more about group-based licensing, see What is group-based licensing in Azure Active Directory.
To get the subscriptions available in the directory, perform a GET subscribedSkus request.

## EXAMPLES

### Example 1: Using the Set-MgGroupLicense Cmdlet
```powershell
Import-Module Microsoft.Graph.Groups
$params = @{
	AddLicenses = @(
		@{
			DisabledPlans = @(
				"113feb6c-3fe4-4440-bddc-54d774bf0318"
				"14ab5db5-e6c4-4b20-b4bc-13e36fd2227f"
			)
			SkuId = "b05e124f-c7cc-45a0-a6aa-8cf78c946968"
		}
		@{
			DisabledPlans = @(
				"a413a9ff-720c-4822-98ef-2f37c2a21f4c"
			)
			SkuId = "c7df2760-2c81-4ef7-b578-5b5392b571df"
		}
	)
	RemoveLicenses = @(
	)
}
Set-MgGroupLicense -GroupId $groupId -BodyParameter $params
```

This example shows how to use the Set-MgGroupLicense Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

### Example 2: Using the Set-MgGroupLicense Cmdlet
```powershell
Import-Module Microsoft.Graph.Groups
$params = @{
	AddLicenses = @(
	)
	RemoveLicenses = @(
		"c7df2760-2c81-4ef7-b578-5b5392b571df"
		"b05e124f-c7cc-45a0-a6aa-8cf78c946968"
	)
}
Set-MgGroupLicense -GroupId $groupId -BodyParameter $params
```

This example shows how to use the Set-MgGroupLicense Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: AssignExpanded1, AssignViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AddLicenses
.
To construct, please use Get-Help -Online and see NOTES section for ADDLICENSES properties and create a hash table.

```yaml
Type: IMicrosoftGraphAssignedLicense[]
Parameter Sets: AssignExpanded1, AssignViaIdentityExpanded1
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
Type: IPaths6Fg5LiGroupsGroupIdMicrosoftGraphAssignlicensePostRequestbodyContentApplicationJsonSchema
Parameter Sets: Assign1, AssignViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -GroupId
key: id of group

```yaml
Type: String
Parameter Sets: AssignExpanded1, Assign1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, please use Get-Help -Online and see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IGroupsIdentity
Parameter Sets: AssignViaIdentityExpanded1, AssignViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -RemoveLicenses
.

```yaml
Type: String[]
Parameter Sets: AssignExpanded1, AssignViaIdentityExpanded1
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

### Microsoft.Graph.PowerShell.Models.IGroupsIdentity
### Microsoft.Graph.PowerShell.Models.IPaths6Fg5LiGroupsGroupIdMicrosoftGraphAssignlicensePostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphGroup
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


ADDLICENSES <IMicrosoftGraphAssignedLicense\[]>: .
  - `[DisabledPlans <String[]>]`: A collection of the unique identifiers for plans that have been disabled.
  - `[SkuId <String>]`: The unique identifier for the SKU.

BODYPARAMETER `<IPaths6Fg5LiGroupsGroupIdMicrosoftGraphAssignlicensePostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AddLicenses <IMicrosoftGraphAssignedLicense[]>]`: 
    - `[DisabledPlans <String[]>]`: A collection of the unique identifiers for plans that have been disabled.
    - `[SkuId <String>]`: The unique identifier for the SKU.
  - `[RemoveLicenses <String[]>]`: 

INPUTOBJECT `<IGroupsIdentity>`: Identity Parameter
  - `[AttachmentId <String>]`: key: id of attachment
  - `[ContentTypeId <String>]`: key: id of contentType
  - `[ConversationId <String>]`: key: id of conversation
  - `[ConversationThreadId <String>]`: key: id of conversationThread
  - `[DirectoryObjectId <String>]`: key: id of directoryObject
  - `[DirectorySettingId <String>]`: key: id of directorySetting
  - `[DocumentSetVersionId <String>]`: key: id of documentSetVersion
  - `[DriveId <String>]`: key: id of drive
  - `[DriveItemId <String>]`: key: id of driveItem
  - `[DriveItemVersionId <String>]`: key: id of driveItemVersion
  - `[EndDateTime <String>]`: Usage: endDateTime='{endDateTime}'
  - `[EndpointId <String>]`: key: id of endpoint
  - `[EventId <String>]`: key: id of event
  - `[ExtensionId <String>]`: key: id of extension
  - `[GroupId <String>]`: key: id of group
  - `[GroupLifecyclePolicyId <String>]`: key: id of groupLifecyclePolicy
  - `[HorizontalSectionColumnId <String>]`: key: id of horizontalSectionColumn
  - `[HorizontalSectionId <String>]`: key: id of horizontalSection
  - `[IncludePersonalNotebooks <Boolean?>]`: Usage: includePersonalNotebooks={includePersonalNotebooks}
  - `[Interval <String>]`: Usage: interval='{interval}'
  - `[ListId <String>]`: key: id of list
  - `[ListId1 <String>]`: Usage: listId='{listId}'
  - `[ListItemId <String>]`: key: id of listItem
  - `[ListItemVersionId <String>]`: key: id of listItemVersion
  - `[MentionId <String>]`: key: id of mention
  - `[MultiValueLegacyExtendedPropertyId <String>]`: key: id of multiValueLegacyExtendedProperty
  - `[NotebookId <String>]`: key: id of notebook
  - `[OnenotePageId <String>]`: key: id of onenotePage
  - `[OnenoteSectionId <String>]`: key: id of onenoteSection
  - `[Path <String>]`: Usage: path='{path}'
  - `[PermissionId <String>]`: key: id of permission
  - `[PostId <String>]`: key: id of post
  - `[ProfilePhotoId <String>]`: key: id of profilePhoto
  - `[Q <String>]`: Usage: q='{q}'
  - `[ResourceSpecificPermissionGrantId <String>]`: key: id of resourceSpecificPermissionGrant
  - `[SingleValueLegacyExtendedPropertyId <String>]`: key: id of singleValueLegacyExtendedProperty
  - `[SiteId <String>]`: key: id of site
  - `[SitePageId <String>]`: key: id of sitePage
  - `[StartDateTime <String>]`: Usage: startDateTime='{startDateTime}'
  - `[SubscriptionId <String>]`: key: id of subscription
  - `[Token <String>]`: Usage: token='{token}'
  - `[User <String>]`: Usage: User='{User}'
  - `[UserId <String>]`: key: id of user
  - `[WebPartId <String>]`: key: id of webPart

## RELATED LINKS
