---
external help file: Microsoft.Graph.Teams-help.xml
Module Name: Microsoft.Graph.Teams
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.teams/set-mgteamschedule
schema: 2.0.0
---

# Set-MgTeamSchedule

## SYNOPSIS
Update the navigation property schedule in teams

## SYNTAX

### SetExpanded1 (Default)
```
Set-MgTeamSchedule -TeamId <String> [-AdditionalProperties <Hashtable>] [-Enabled] [-Id <String>]
 [-OfferShiftRequests <IMicrosoftGraphOfferShiftRequest1[]>] [-OfferShiftRequestsEnabled]
 [-OpenShiftChangeRequests <IMicrosoftGraphOpenShiftChangeRequest1[]>]
 [-OpenShifts <IMicrosoftGraphOpenShift1[]>] [-OpenShiftsEnabled] [-ProvisionStatus <String>]
 [-SchedulingGroups <IMicrosoftGraphSchedulingGroup1[]>] [-Shifts <IMicrosoftGraphShift1[]>]
 [-SwapShiftsChangeRequests <IMicrosoftGraphSwapShiftsChangeRequest1[]>] [-SwapShiftsRequestsEnabled]
 [-TimeCards <IMicrosoftGraphTimeCard[]>] [-TimeClockEnabled]
 [-TimeClockSettings <IMicrosoftGraphTimeClockSettings>] [-TimeOffReasons <IMicrosoftGraphTimeOffReason1[]>]
 [-TimeOffRequests <IMicrosoftGraphTimeOffRequest1[]>] [-TimeOffRequestsEnabled] [-TimeZone <String>]
 [-TimesOff <IMicrosoftGraphTimeOff1[]>] [-WorkforceIntegrationIds <String[]>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Set1
```
Set-MgTeamSchedule -TeamId <String> -BodyParameter <IMicrosoftGraphSchedule1> [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### SetViaIdentityExpanded1
```
Set-MgTeamSchedule -InputObject <ITeamsIdentity> [-AdditionalProperties <Hashtable>] [-Enabled] [-Id <String>]
 [-OfferShiftRequests <IMicrosoftGraphOfferShiftRequest1[]>] [-OfferShiftRequestsEnabled]
 [-OpenShiftChangeRequests <IMicrosoftGraphOpenShiftChangeRequest1[]>]
 [-OpenShifts <IMicrosoftGraphOpenShift1[]>] [-OpenShiftsEnabled] [-ProvisionStatus <String>]
 [-SchedulingGroups <IMicrosoftGraphSchedulingGroup1[]>] [-Shifts <IMicrosoftGraphShift1[]>]
 [-SwapShiftsChangeRequests <IMicrosoftGraphSwapShiftsChangeRequest1[]>] [-SwapShiftsRequestsEnabled]
 [-TimeCards <IMicrosoftGraphTimeCard[]>] [-TimeClockEnabled]
 [-TimeClockSettings <IMicrosoftGraphTimeClockSettings>] [-TimeOffReasons <IMicrosoftGraphTimeOffReason1[]>]
 [-TimeOffRequests <IMicrosoftGraphTimeOffRequest1[]>] [-TimeOffRequestsEnabled] [-TimeZone <String>]
 [-TimesOff <IMicrosoftGraphTimeOff1[]>] [-WorkforceIntegrationIds <String[]>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### SetViaIdentity1
```
Set-MgTeamSchedule -InputObject <ITeamsIdentity> -BodyParameter <IMicrosoftGraphSchedule1> [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property schedule in teams

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
schedule
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphSchedule1
Parameter Sets: Set1, SetViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Enabled
Indicates whether the schedule is enabled for the team.
Required.

```yaml
Type: SwitchParameter
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
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
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
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
Type: ITeamsIdentity
Parameter Sets: SetViaIdentityExpanded1, SetViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -OfferShiftRequests
.
To construct, please use Get-Help -Online and see NOTES section for OFFERSHIFTREQUESTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphOfferShiftRequest1[]
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OfferShiftRequestsEnabled
Indicates whether offer shift requests are enabled for the schedule.

```yaml
Type: SwitchParameter
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OpenShiftChangeRequests
.
To construct, please use Get-Help -Online and see NOTES section for OPENSHIFTCHANGEREQUESTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphOpenShiftChangeRequest1[]
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OpenShifts
.
To construct, please use Get-Help -Online and see NOTES section for OPENSHIFTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphOpenShift1[]
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OpenShiftsEnabled
Indicates whether open shifts are enabled for the schedule.

```yaml
Type: SwitchParameter
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
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

### -ProvisionStatus
operationStatus

```yaml
Type: String
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SchedulingGroups
The logical grouping of users in the schedule (usually by role).
To construct, please use Get-Help -Online and see NOTES section for SCHEDULINGGROUPS properties and create a hash table.

```yaml
Type: IMicrosoftGraphSchedulingGroup1[]
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Shifts
The shifts in the schedule.
To construct, please use Get-Help -Online and see NOTES section for SHIFTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphShift1[]
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SwapShiftsChangeRequests
.
To construct, please use Get-Help -Online and see NOTES section for SWAPSHIFTSCHANGEREQUESTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphSwapShiftsChangeRequest1[]
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SwapShiftsRequestsEnabled
Indicates whether swap shifts requests are enabled for the schedule.

```yaml
Type: SwitchParameter
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TeamId
key: id of team

```yaml
Type: String
Parameter Sets: SetExpanded1, Set1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeCards
.
To construct, please use Get-Help -Online and see NOTES section for TIMECARDS properties and create a hash table.

```yaml
Type: IMicrosoftGraphTimeCard[]
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeClockEnabled
Indicates whether time clock is enabled for the schedule.

```yaml
Type: SwitchParameter
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeClockSettings
timeClockSettings
To construct, please use Get-Help -Online and see NOTES section for TIMECLOCKSETTINGS properties and create a hash table.

```yaml
Type: IMicrosoftGraphTimeClockSettings
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeOffReasons
The set of reasons for a time off in the schedule.
To construct, please use Get-Help -Online and see NOTES section for TIMEOFFREASONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphTimeOffReason1[]
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeOffRequests
.
To construct, please use Get-Help -Online and see NOTES section for TIMEOFFREQUESTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphTimeOffRequest1[]
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeOffRequestsEnabled
Indicates whether time off requests are enabled for the schedule.

```yaml
Type: SwitchParameter
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimesOff
The instances of times off in the schedule.
To construct, please use Get-Help -Online and see NOTES section for TIMESOFF properties and create a hash table.

```yaml
Type: IMicrosoftGraphTimeOff1[]
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeZone
Indicates the time zone of the schedule team using tz database format.
Required.

```yaml
Type: String
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WorkforceIntegrationIds
.

```yaml
Type: String[]
Parameter Sets: SetExpanded1, SetViaIdentityExpanded1
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphSchedule1
### Microsoft.Graph.PowerShell.Models.ITeamsIdentity
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IMicrosoftGraphSchedule1>`: schedule
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[Enabled <Boolean?>]`: Indicates whether the schedule is enabled for the team. Required.
  - `[OfferShiftRequests <IMicrosoftGraphOfferShiftRequest1[]>]`: 
    - `[AssignedTo <String>]`: scheduleChangeRequestActor
    - `[ManagerActionMessage <String>]`: 
    - `[SenderMessage <String>]`: 
    - `[State <String>]`: scheduleChangeState
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Application <IMicrosoftGraphIdentity>]`: identity
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
        - `[Id <String>]`: Unique identifier for the identity.
      - `[Device <IMicrosoftGraphIdentity>]`: identity
      - `[User <IMicrosoftGraphIdentity>]`: identity
    - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[RecipientActionMessage <String>]`: Custom message sent by recipient of the offer shift request.
    - `[RecipientUserId <String>]`: User id of the recipient of the offer shift request.
    - `[SenderShiftId <String>]`: User id of the sender of the offer shift request.
  - `[OfferShiftRequestsEnabled <Boolean?>]`: Indicates whether offer shift requests are enabled for the schedule.
  - `[OpenShiftChangeRequests <IMicrosoftGraphOpenShiftChangeRequest1[]>]`: 
    - `[AssignedTo <String>]`: scheduleChangeRequestActor
    - `[ManagerActionMessage <String>]`: 
    - `[SenderMessage <String>]`: 
    - `[State <String>]`: scheduleChangeState
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[OpenShiftId <String>]`: ID for the open shift.
  - `[OpenShifts <IMicrosoftGraphOpenShift1[]>]`: 
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[DraftOpenShift <IMicrosoftGraphOpenShiftItem>]`: openShiftItem
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Activities <IMicrosoftGraphShiftActivity[]>]`: An incremental part of a shift which can cover details of when and where an employee is during their shift. For example, an assignment or a scheduled break or lunch. Required.
        - `[Code <String>]`: Customer defined code for the shiftActivity. Required.
        - `[DisplayName <String>]`: The name of the shiftActivity. Required.
        - `[EndDateTime <DateTime?>]`: The end date and time for the shiftActivity. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z. Required.
        - `[IsPaid <Boolean?>]`: Indicates whether the microsoft.graph.user should be paid for the activity during their shift. Required.
        - `[StartDateTime <DateTime?>]`: The start date and time for the shiftActivity. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z. Required.
        - `[Theme <String>]`: scheduleEntityTheme
      - `[DisplayName <String>]`: The shift label of the shiftItem.
      - `[Notes <String>]`: The shift notes for the shiftItem.
      - `[EndDateTime <DateTime?>]`: 
      - `[StartDateTime <DateTime?>]`: 
      - `[Theme <String>]`: scheduleEntityTheme
      - `[OpenSlotCount <Int32?>]`: Count of the number of slots for the given open shift.
    - `[IsStagedForDeletion <Boolean?>]`: 
    - `[SchedulingGroupId <String>]`: ID for the scheduling group that the open shift belongs to.
    - `[SharedOpenShift <IMicrosoftGraphOpenShiftItem>]`: openShiftItem
  - `[OpenShiftsEnabled <Boolean?>]`: Indicates whether open shifts are enabled for the schedule.
  - `[ProvisionStatus <String>]`: operationStatus
  - `[SchedulingGroups <IMicrosoftGraphSchedulingGroup1[]>]`: The logical grouping of users in the schedule (usually by role).
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[DisplayName <String>]`: The display name for the schedulingGroup. Required.
    - `[UserIds <String[]>]`: The list of user IDs that are a member of the schedulingGroup. Required.
  - `[Shifts <IMicrosoftGraphShift1[]>]`: The shifts in the schedule.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[DraftShift <IMicrosoftGraphShiftItem>]`: shiftItem
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[EndDateTime <DateTime?>]`: 
      - `[StartDateTime <DateTime?>]`: 
      - `[Theme <String>]`: scheduleEntityTheme
      - `[Activities <IMicrosoftGraphShiftActivity[]>]`: An incremental part of a shift which can cover details of when and where an employee is during their shift. For example, an assignment or a scheduled break or lunch. Required.
      - `[DisplayName <String>]`: The shift label of the shiftItem.
      - `[Notes <String>]`: The shift notes for the shiftItem.
    - `[IsStagedForDeletion <Boolean?>]`: 
    - `[SchedulingGroupId <String>]`: ID of the scheduling group the shift is part of. Required.
    - `[SharedShift <IMicrosoftGraphShiftItem>]`: shiftItem
    - `[UserId <String>]`: ID of the user assigned to the shift. Required.
  - `[SwapShiftsChangeRequests <IMicrosoftGraphSwapShiftsChangeRequest1[]>]`: 
    - `[RecipientActionMessage <String>]`: Custom message sent by recipient of the offer shift request.
    - `[RecipientUserId <String>]`: User id of the recipient of the offer shift request.
    - `[SenderShiftId <String>]`: User id of the sender of the offer shift request.
    - `[AssignedTo <String>]`: scheduleChangeRequestActor
    - `[ManagerActionMessage <String>]`: 
    - `[SenderMessage <String>]`: 
    - `[State <String>]`: scheduleChangeState
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[RecipientShiftId <String>]`: Shift ID for the recipient user with whom the request is to swap.
  - `[SwapShiftsRequestsEnabled <Boolean?>]`: Indicates whether swap shifts requests are enabled for the schedule.
  - `[TimeCards <IMicrosoftGraphTimeCard[]>]`: 
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[Breaks <IMicrosoftGraphTimeCardBreak[]>]`: The list of breaks associated with the timeCard.
      - `[BreakId <String>]`: ID of the timeCardBreak.
      - `[End <IMicrosoftGraphTimeCardEvent>]`: timeCardEvent
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[AtApprovedLocation <Boolean?>]`: Indicates whether the entry was recorded at the approved location.
        - `[DateTime <DateTime?>]`: The time the entry is recorded.
        - `[Notes <IMicrosoftGraphItemBody>]`: itemBody
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Content <String>]`: The content of the item.
          - `[ContentType <String>]`: bodyType
      - `[Notes <IMicrosoftGraphItemBody>]`: itemBody
      - `[Start <IMicrosoftGraphTimeCardEvent>]`: timeCardEvent
    - `[ClockInEvent <IMicrosoftGraphTimeCardEvent>]`: timeCardEvent
    - `[ClockOutEvent <IMicrosoftGraphTimeCardEvent>]`: timeCardEvent
    - `[ConfirmedBy <String>]`: confirmedBy
    - `[Notes <IMicrosoftGraphItemBody>]`: itemBody
    - `[OriginalEntry <IMicrosoftGraphTimeCardEntry>]`: timeCardEntry
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Breaks <IMicrosoftGraphTimeCardBreak[]>]`: The list of breaks associated with the timeCard.
      - `[ClockInEvent <IMicrosoftGraphTimeCardEvent>]`: timeCardEvent
      - `[ClockOutEvent <IMicrosoftGraphTimeCardEvent>]`: timeCardEvent
    - `[State <String>]`: timeCardState
    - `[UserId <String>]`: User ID to which  the timeCard belongs.
  - `[TimeClockEnabled <Boolean?>]`: Indicates whether time clock is enabled for the schedule.
  - `[TimeClockSettings <IMicrosoftGraphTimeClockSettings>]`: timeClockSettings
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ApprovedLocation <IMicrosoftGraphGeoCoordinates>]`: geoCoordinates
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Altitude <Double?>]`: Optional. The altitude (height), in feet,  above sea level for the item. Read-only.
      - `[Latitude <Double?>]`: Optional. The latitude, in decimal, for the item. Read-only.
      - `[Longitude <Double?>]`: Optional. The longitude, in decimal, for the item. Read-only.
  - `[TimeOffReasons <IMicrosoftGraphTimeOffReason1[]>]`: The set of reasons for a time off in the schedule.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[DisplayName <String>]`: The name of the timeOffReason. Required.
    - `[IconType <String>]`: timeOffReasonIconType
    - `[IsActive <Boolean?>]`: Indicates whether the timeOffReason can be used when creating new entities or updating existing ones. Required.
  - `[TimeOffRequests <IMicrosoftGraphTimeOffRequest1[]>]`: 
    - `[AssignedTo <String>]`: scheduleChangeRequestActor
    - `[ManagerActionMessage <String>]`: 
    - `[SenderMessage <String>]`: 
    - `[State <String>]`: scheduleChangeState
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[EndDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[StartDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[TimeOffReasonId <String>]`: The reason for the time off.
  - `[TimeOffRequestsEnabled <Boolean?>]`: Indicates whether time off requests are enabled for the schedule.
  - `[TimeZone <String>]`: Indicates the time zone of the schedule team using tz database format. Required.
  - `[TimesOff <IMicrosoftGraphTimeOff1[]>]`: The instances of times off in the schedule.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[DraftTimeOff <IMicrosoftGraphTimeOffItem>]`: timeOffItem
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[EndDateTime <DateTime?>]`: 
      - `[StartDateTime <DateTime?>]`: 
      - `[Theme <String>]`: scheduleEntityTheme
      - `[TimeOffReasonId <String>]`: ID of the timeOffReason for this timeOffItem. Required.
    - `[IsStagedForDeletion <Boolean?>]`: 
    - `[SharedTimeOff <IMicrosoftGraphTimeOffItem>]`: timeOffItem
    - `[UserId <String>]`: ID of the user assigned to the timeOff. Required.
  - `[WorkforceIntegrationIds <String[]>]`: 

INPUTOBJECT `<ITeamsIdentity>`: Identity Parameter
  - `[AssociatedTeamInfoId <String>]`: key: id of associatedTeamInfo
  - `[ChannelId <String>]`: key: id of channel
  - `[ChatId <String>]`: key: id of chat
  - `[ChatMessageHostedContentId <String>]`: key: id of chatMessageHostedContent
  - `[ChatMessageId <String>]`: key: id of chatMessage
  - `[ChatMessageId1 <String>]`: key: id of chatMessage
  - `[ConversationMemberId <String>]`: key: id of conversationMember
  - `[DeletedTeamId <String>]`: key: id of deletedTeam
  - `[GroupId <String>]`: key: id of group
  - `[OfferShiftRequestId <String>]`: key: id of offerShiftRequest
  - `[OpenShiftChangeRequestId <String>]`: key: id of openShiftChangeRequest
  - `[OpenShiftId <String>]`: key: id of openShift
  - `[PinnedChatMessageInfoId <String>]`: key: id of pinnedChatMessageInfo
  - `[ResourceSpecificPermissionGrantId <String>]`: key: id of resourceSpecificPermissionGrant
  - `[SchedulingGroupId <String>]`: key: id of schedulingGroup
  - `[SharedWithChannelTeamInfoId <String>]`: key: id of sharedWithChannelTeamInfo
  - `[ShiftId <String>]`: key: id of shift
  - `[SwapShiftsChangeRequestId <String>]`: key: id of swapShiftsChangeRequest
  - `[TeamId <String>]`: key: id of team
  - `[TeamTemplateDefinitionId <String>]`: key: id of teamTemplateDefinition
  - `[TeamTemplateId <String>]`: key: id of teamTemplate
  - `[TeamsAppDefinitionId <String>]`: key: id of teamsAppDefinition
  - `[TeamsAppId <String>]`: key: id of teamsApp
  - `[TeamsAppInstallationId <String>]`: key: id of teamsAppInstallation
  - `[TeamsAsyncOperationId <String>]`: key: id of teamsAsyncOperation
  - `[TeamsTabId <String>]`: key: id of teamsTab
  - `[TeamworkDeviceId <String>]`: key: id of teamworkDevice
  - `[TeamworkDeviceOperationId <String>]`: key: id of teamworkDeviceOperation
  - `[TeamworkTagId <String>]`: key: id of teamworkTag
  - `[TeamworkTagMemberId <String>]`: key: id of teamworkTagMember
  - `[TimeCardId <String>]`: key: id of timeCard
  - `[TimeOffId <String>]`: key: id of timeOff
  - `[TimeOffReasonId <String>]`: key: id of timeOffReason
  - `[TimeOffRequestId <String>]`: key: id of timeOffRequest
  - `[UserId <String>]`: key: id of user
  - `[UserScopeTeamsAppInstallationId <String>]`: key: id of userScopeTeamsAppInstallation
  - `[WorkforceIntegrationId <String>]`: key: id of workforceIntegration

OFFERSHIFTREQUESTS <IMicrosoftGraphOfferShiftRequest1\[]>: .
  - `[AssignedTo <String>]`: scheduleChangeRequestActor
  - `[ManagerActionMessage <String>]`: 
  - `[SenderMessage <String>]`: 
  - `[State <String>]`: scheduleChangeState
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[RecipientActionMessage <String>]`: Custom message sent by recipient of the offer shift request.
  - `[RecipientUserId <String>]`: User id of the recipient of the offer shift request.
  - `[SenderShiftId <String>]`: User id of the sender of the offer shift request.

OPENSHIFTCHANGEREQUESTS <IMicrosoftGraphOpenShiftChangeRequest1\[]>: .
  - `[AssignedTo <String>]`: scheduleChangeRequestActor
  - `[ManagerActionMessage <String>]`: 
  - `[SenderMessage <String>]`: 
  - `[State <String>]`: scheduleChangeState
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[OpenShiftId <String>]`: ID for the open shift.

OPENSHIFTS <IMicrosoftGraphOpenShift1\[]>: .
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[DraftOpenShift <IMicrosoftGraphOpenShiftItem>]`: openShiftItem
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Activities <IMicrosoftGraphShiftActivity[]>]`: An incremental part of a shift which can cover details of when and where an employee is during their shift. For example, an assignment or a scheduled break or lunch. Required.
      - `[Code <String>]`: Customer defined code for the shiftActivity. Required.
      - `[DisplayName <String>]`: The name of the shiftActivity. Required.
      - `[EndDateTime <DateTime?>]`: The end date and time for the shiftActivity. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z. Required.
      - `[IsPaid <Boolean?>]`: Indicates whether the microsoft.graph.user should be paid for the activity during their shift. Required.
      - `[StartDateTime <DateTime?>]`: The start date and time for the shiftActivity. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z. Required.
      - `[Theme <String>]`: scheduleEntityTheme
    - `[DisplayName <String>]`: The shift label of the shiftItem.
    - `[Notes <String>]`: The shift notes for the shiftItem.
    - `[EndDateTime <DateTime?>]`: 
    - `[StartDateTime <DateTime?>]`: 
    - `[Theme <String>]`: scheduleEntityTheme
    - `[OpenSlotCount <Int32?>]`: Count of the number of slots for the given open shift.
  - `[IsStagedForDeletion <Boolean?>]`: 
  - `[SchedulingGroupId <String>]`: ID for the scheduling group that the open shift belongs to.
  - `[SharedOpenShift <IMicrosoftGraphOpenShiftItem>]`: openShiftItem

SCHEDULINGGROUPS <IMicrosoftGraphSchedulingGroup1\[]>: The logical grouping of users in the schedule (usually by role).
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[DisplayName <String>]`: The display name for the schedulingGroup. Required.
  - `[UserIds <String[]>]`: The list of user IDs that are a member of the schedulingGroup. Required.

SHIFTS <IMicrosoftGraphShift1\[]>: The shifts in the schedule.
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[DraftShift <IMicrosoftGraphShiftItem>]`: shiftItem
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[EndDateTime <DateTime?>]`: 
    - `[StartDateTime <DateTime?>]`: 
    - `[Theme <String>]`: scheduleEntityTheme
    - `[Activities <IMicrosoftGraphShiftActivity[]>]`: An incremental part of a shift which can cover details of when and where an employee is during their shift. For example, an assignment or a scheduled break or lunch. Required.
      - `[Code <String>]`: Customer defined code for the shiftActivity. Required.
      - `[DisplayName <String>]`: The name of the shiftActivity. Required.
      - `[EndDateTime <DateTime?>]`: The end date and time for the shiftActivity. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z. Required.
      - `[IsPaid <Boolean?>]`: Indicates whether the microsoft.graph.user should be paid for the activity during their shift. Required.
      - `[StartDateTime <DateTime?>]`: The start date and time for the shiftActivity. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z. Required.
      - `[Theme <String>]`: scheduleEntityTheme
    - `[DisplayName <String>]`: The shift label of the shiftItem.
    - `[Notes <String>]`: The shift notes for the shiftItem.
  - `[IsStagedForDeletion <Boolean?>]`: 
  - `[SchedulingGroupId <String>]`: ID of the scheduling group the shift is part of. Required.
  - `[SharedShift <IMicrosoftGraphShiftItem>]`: shiftItem
  - `[UserId <String>]`: ID of the user assigned to the shift. Required.

SWAPSHIFTSCHANGEREQUESTS <IMicrosoftGraphSwapShiftsChangeRequest1\[]>: .
  - `[RecipientActionMessage <String>]`: Custom message sent by recipient of the offer shift request.
  - `[RecipientUserId <String>]`: User id of the recipient of the offer shift request.
  - `[SenderShiftId <String>]`: User id of the sender of the offer shift request.
  - `[AssignedTo <String>]`: scheduleChangeRequestActor
  - `[ManagerActionMessage <String>]`: 
  - `[SenderMessage <String>]`: 
  - `[State <String>]`: scheduleChangeState
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[RecipientShiftId <String>]`: Shift ID for the recipient user with whom the request is to swap.

TIMECARDS <IMicrosoftGraphTimeCard\[]>: .
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[Breaks <IMicrosoftGraphTimeCardBreak[]>]`: The list of breaks associated with the timeCard.
    - `[BreakId <String>]`: ID of the timeCardBreak.
    - `[End <IMicrosoftGraphTimeCardEvent>]`: timeCardEvent
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[AtApprovedLocation <Boolean?>]`: Indicates whether the entry was recorded at the approved location.
      - `[DateTime <DateTime?>]`: The time the entry is recorded.
      - `[Notes <IMicrosoftGraphItemBody>]`: itemBody
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Content <String>]`: The content of the item.
        - `[ContentType <String>]`: bodyType
    - `[Notes <IMicrosoftGraphItemBody>]`: itemBody
    - `[Start <IMicrosoftGraphTimeCardEvent>]`: timeCardEvent
  - `[ClockInEvent <IMicrosoftGraphTimeCardEvent>]`: timeCardEvent
  - `[ClockOutEvent <IMicrosoftGraphTimeCardEvent>]`: timeCardEvent
  - `[ConfirmedBy <String>]`: confirmedBy
  - `[Notes <IMicrosoftGraphItemBody>]`: itemBody
  - `[OriginalEntry <IMicrosoftGraphTimeCardEntry>]`: timeCardEntry
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Breaks <IMicrosoftGraphTimeCardBreak[]>]`: The list of breaks associated with the timeCard.
    - `[ClockInEvent <IMicrosoftGraphTimeCardEvent>]`: timeCardEvent
    - `[ClockOutEvent <IMicrosoftGraphTimeCardEvent>]`: timeCardEvent
  - `[State <String>]`: timeCardState
  - `[UserId <String>]`: User ID to which  the timeCard belongs.

TIMECLOCKSETTINGS `<IMicrosoftGraphTimeClockSettings>`: timeClockSettings
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ApprovedLocation <IMicrosoftGraphGeoCoordinates>]`: geoCoordinates
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Altitude <Double?>]`: Optional. The altitude (height), in feet,  above sea level for the item. Read-only.
    - `[Latitude <Double?>]`: Optional. The latitude, in decimal, for the item. Read-only.
    - `[Longitude <Double?>]`: Optional. The longitude, in decimal, for the item. Read-only.

TIMEOFFREASONS <IMicrosoftGraphTimeOffReason1\[]>: The set of reasons for a time off in the schedule.
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[DisplayName <String>]`: The name of the timeOffReason. Required.
  - `[IconType <String>]`: timeOffReasonIconType
  - `[IsActive <Boolean?>]`: Indicates whether the timeOffReason can be used when creating new entities or updating existing ones. Required.

TIMEOFFREQUESTS <IMicrosoftGraphTimeOffRequest1\[]>: .
  - `[AssignedTo <String>]`: scheduleChangeRequestActor
  - `[ManagerActionMessage <String>]`: 
  - `[SenderMessage <String>]`: 
  - `[State <String>]`: scheduleChangeState
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[EndDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[StartDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[TimeOffReasonId <String>]`: The reason for the time off.

TIMESOFF <IMicrosoftGraphTimeOff1\[]>: The instances of times off in the schedule.
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[DraftTimeOff <IMicrosoftGraphTimeOffItem>]`: timeOffItem
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[EndDateTime <DateTime?>]`: 
    - `[StartDateTime <DateTime?>]`: 
    - `[Theme <String>]`: scheduleEntityTheme
    - `[TimeOffReasonId <String>]`: ID of the timeOffReason for this timeOffItem. Required.
  - `[IsStagedForDeletion <Boolean?>]`: 
  - `[SharedTimeOff <IMicrosoftGraphTimeOffItem>]`: timeOffItem
  - `[UserId <String>]`: ID of the user assigned to the timeOff. Required.

## RELATED LINKS

## RELATED LINKS
