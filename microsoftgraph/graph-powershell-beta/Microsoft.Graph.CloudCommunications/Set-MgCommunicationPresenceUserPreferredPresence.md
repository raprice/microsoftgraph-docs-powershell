---
external help file: Microsoft.Graph.CloudCommunications-help.xml
Module Name: Microsoft.Graph.CloudCommunications
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.cloudcommunications/set-mgcommunicationpresenceuserpreferredpresence
schema: 2.0.0
---

# Set-MgCommunicationPresenceUserPreferredPresence

## SYNOPSIS
Set the preferred availability and activity status for a user.
If the preferred presence of a user is set, the user's presence is the preferred presence.
Preferred presence takes effect only when there is at least one presence session of the user.
Otherwise, the user's presence stays as Offline.
A presence session can be created as a result of a successful setPresence operation, or if the user is signed in on a Teams client.
Read more about presence sessions and their time-out and expiration.

## SYNTAX

### SetExpanded (Default)
```
Set-MgCommunicationPresenceUserPreferredPresence -PresenceId <String> [-Activity <String>]
 [-AdditionalProperties <Hashtable>] [-Availability <String>] [-ExpirationDuration <TimeSpan>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Set
```
Set-MgCommunicationPresenceUserPreferredPresence -PresenceId <String>
 -BodyParameter <IPaths16OmbuoCommunicationsPresencesPresenceIdMicrosoftGraphSetuserpreferredpresencePostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SetViaIdentityExpanded
```
Set-MgCommunicationPresenceUserPreferredPresence -InputObject <ICloudCommunicationsIdentity>
 [-Activity <String>] [-AdditionalProperties <Hashtable>] [-Availability <String>]
 [-ExpirationDuration <TimeSpan>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SetViaIdentity
```
Set-MgCommunicationPresenceUserPreferredPresence -InputObject <ICloudCommunicationsIdentity>
 -BodyParameter <IPaths16OmbuoCommunicationsPresencesPresenceIdMicrosoftGraphSetuserpreferredpresencePostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Set the preferred availability and activity status for a user.
If the preferred presence of a user is set, the user's presence is the preferred presence.
Preferred presence takes effect only when there is at least one presence session of the user.
Otherwise, the user's presence stays as Offline.
A presence session can be created as a result of a successful setPresence operation, or if the user is signed in on a Teams client.
Read more about presence sessions and their time-out and expiration.

## EXAMPLES

## PARAMETERS

### -Activity
.

```yaml
Type: String
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Availability
.

```yaml
Type: String
Parameter Sets: SetExpanded, SetViaIdentityExpanded
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
Type: IPaths16OmbuoCommunicationsPresencesPresenceIdMicrosoftGraphSetuserpreferredpresencePostRequestbodyContentApplicationJsonSchema
Parameter Sets: Set, SetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ExpirationDuration
.

```yaml
Type: TimeSpan
Parameter Sets: SetExpanded, SetViaIdentityExpanded
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
Type: ICloudCommunicationsIdentity
Parameter Sets: SetViaIdentityExpanded, SetViaIdentity
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

### -PresenceId
key: id of presence

```yaml
Type: String
Parameter Sets: SetExpanded, Set
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

### Microsoft.Graph.PowerShell.Models.ICloudCommunicationsIdentity
### Microsoft.Graph.PowerShell.Models.IPaths16OmbuoCommunicationsPresencesPresenceIdMicrosoftGraphSetuserpreferredpresencePostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IPaths16OmbuoCommunicationsPresencesPresenceIdMicrosoftGraphSetuserpreferredpresencePostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Activity <String>]`: 
  - `[Availability <String>]`: 
  - `[ExpirationDuration <TimeSpan?>]`: 

INPUTOBJECT `<ICloudCommunicationsIdentity>`: Identity Parameter
  - `[AttendanceRecordId <String>]`: key: id of attendanceRecord
  - `[AudioRoutingGroupId <String>]`: key: id of audioRoutingGroup
  - `[CallId <String>]`: key: id of call
  - `[CallRecordId <String>]`: key: id of callRecord
  - `[CallTranscriptId <String>]`: key: id of callTranscript
  - `[CommsOperationId <String>]`: key: id of commsOperation
  - `[ContentSharingSessionId <String>]`: key: id of contentSharingSession
  - `[MeetingAttendanceReportId <String>]`: key: id of meetingAttendanceReport
  - `[MeetingRegistrationQuestionId <String>]`: key: id of meetingRegistrationQuestion
  - `[OnlineMeetingId <String>]`: key: id of onlineMeeting
  - `[ParticipantId <String>]`: key: id of participant
  - `[PresenceId <String>]`: key: id of presence
  - `[SessionId <String>]`: key: id of session
  - `[UserId <String>]`: key: id of user

## RELATED LINKS
