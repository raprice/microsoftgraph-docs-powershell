---
external help file: Microsoft.Graph.CloudCommunications-help.xml
Module Name: Microsoft.Graph.CloudCommunications
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.cloudcommunications/update-mguseronlinemeetingattendancereportattendancerecord
schema: 2.0.0
---

# Update-MgUserOnlineMeetingAttendanceReportAttendanceRecord

## SYNOPSIS
Update the navigation property attendanceRecords in users

## SYNTAX

### UpdateExpanded1 (Default)
```
Update-MgUserOnlineMeetingAttendanceReportAttendanceRecord -AttendanceRecordId <String>
 -OnlineMeetingId <String> -UserId <String> [-AdditionalProperties <Hashtable>]
 [-AttendanceIntervals <IMicrosoftGraphAttendanceInterval[]>] [-EmailAddress <String>] [-Id <String>]
 [-Identity <IMicrosoftGraphIdentity>] [-RegistrantId <String>] [-Role <String>]
 [-TotalAttendanceInSeconds <Int32>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateExpanded
```
Update-MgUserOnlineMeetingAttendanceReportAttendanceRecord -AttendanceRecordId <String>
 -MeetingAttendanceReportId <String> -OnlineMeetingId <String> -UserId <String>
 [-AdditionalProperties <Hashtable>] [-AttendanceIntervals <IMicrosoftGraphAttendanceInterval[]>]
 [-EmailAddress <String>] [-Id <String>] [-Identity <IMicrosoftGraphIdentity>] [-RegistrantId <String>]
 [-Role <String>] [-TotalAttendanceInSeconds <Int32>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update1
```
Update-MgUserOnlineMeetingAttendanceReportAttendanceRecord -AttendanceRecordId <String>
 -OnlineMeetingId <String> -UserId <String> -BodyParameter <IMicrosoftGraphAttendanceRecord1> [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgUserOnlineMeetingAttendanceReportAttendanceRecord -AttendanceRecordId <String>
 -MeetingAttendanceReportId <String> -OnlineMeetingId <String> -UserId <String>
 -BodyParameter <IMicrosoftGraphAttendanceRecord1> [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded1
```
Update-MgUserOnlineMeetingAttendanceReportAttendanceRecord -InputObject <ICloudCommunicationsIdentity>
 [-AdditionalProperties <Hashtable>] [-AttendanceIntervals <IMicrosoftGraphAttendanceInterval[]>]
 [-EmailAddress <String>] [-Id <String>] [-Identity <IMicrosoftGraphIdentity>] [-RegistrantId <String>]
 [-Role <String>] [-TotalAttendanceInSeconds <Int32>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgUserOnlineMeetingAttendanceReportAttendanceRecord -InputObject <ICloudCommunicationsIdentity>
 [-AdditionalProperties <Hashtable>] [-AttendanceIntervals <IMicrosoftGraphAttendanceInterval[]>]
 [-EmailAddress <String>] [-Id <String>] [-Identity <IMicrosoftGraphIdentity>] [-RegistrantId <String>]
 [-Role <String>] [-TotalAttendanceInSeconds <Int32>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity1
```
Update-MgUserOnlineMeetingAttendanceReportAttendanceRecord -InputObject <ICloudCommunicationsIdentity>
 -BodyParameter <IMicrosoftGraphAttendanceRecord1> [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgUserOnlineMeetingAttendanceReportAttendanceRecord -InputObject <ICloudCommunicationsIdentity>
 -BodyParameter <IMicrosoftGraphAttendanceRecord1> [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property attendanceRecords in users

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded1, UpdateExpanded, UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AttendanceIntervals
List of time periods between joining and leaving a meeting.
To construct, please use Get-Help -Online and see NOTES section for ATTENDANCEINTERVALS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAttendanceInterval[]
Parameter Sets: UpdateExpanded1, UpdateExpanded, UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AttendanceRecordId
key: id of attendanceRecord

```yaml
Type: String
Parameter Sets: UpdateExpanded1, UpdateExpanded, Update1, Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
attendanceRecord
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAttendanceRecord1
Parameter Sets: Update1, Update, UpdateViaIdentity1, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -EmailAddress
Email address of the user associated with this atttendance record.

```yaml
Type: String
Parameter Sets: UpdateExpanded1, UpdateExpanded, UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded1, UpdateExpanded, UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Identity
identity
To construct, please use Get-Help -Online and see NOTES section for IDENTITY properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentity
Parameter Sets: UpdateExpanded1, UpdateExpanded, UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded, UpdateViaIdentity1, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MeetingAttendanceReportId
key: id of meetingAttendanceReport

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

### -OnlineMeetingId
key: id of onlineMeeting

```yaml
Type: String
Parameter Sets: UpdateExpanded1, UpdateExpanded, Update1, Update
Aliases:

Required: True
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

### -RegistrantId
Unique identifier of a meetingRegistrant.
Presents when the participant has registered for the meeting.

```yaml
Type: String
Parameter Sets: UpdateExpanded1, UpdateExpanded, UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Role
Role of the attendee.
Possible values are: None, Attendee, Presenter, and Organizer.

```yaml
Type: String
Parameter Sets: UpdateExpanded1, UpdateExpanded, UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TotalAttendanceInSeconds
Total duration of the attendances in seconds.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded1, UpdateExpanded, UpdateViaIdentityExpanded1, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded1, UpdateExpanded, Update1, Update
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
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAttendanceRecord1
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


ATTENDANCEINTERVALS <IMicrosoftGraphAttendanceInterval\[]>: List of time periods between joining and leaving a meeting.
  - `[DurationInSeconds <Int32?>]`: Duration of the meeting interval in seconds; that is, the difference between joinDateTime and leaveDateTime.
  - `[JoinDateTime <DateTime?>]`: The time the attendee joined in UTC.
  - `[LeaveDateTime <DateTime?>]`: The time the attendee left in UTC.

BODYPARAMETER `<IMicrosoftGraphAttendanceRecord1>`: attendanceRecord
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[AttendanceIntervals <IMicrosoftGraphAttendanceInterval[]>]`: List of time periods between joining and leaving a meeting.
    - `[DurationInSeconds <Int32?>]`: Duration of the meeting interval in seconds; that is, the difference between joinDateTime and leaveDateTime.
    - `[JoinDateTime <DateTime?>]`: The time the attendee joined in UTC.
    - `[LeaveDateTime <DateTime?>]`: The time the attendee left in UTC.
  - `[EmailAddress <String>]`: Email address of the user associated with this atttendance record.
  - `[Identity <IMicrosoftGraphIdentity>]`: identity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
    - `[Id <String>]`: Unique identifier for the identity.
  - `[RegistrantId <String>]`: Unique identifier of a meetingRegistrant. Presents when the participant has registered for the meeting.
  - `[Role <String>]`: Role of the attendee. Possible values are: None, Attendee, Presenter, and Organizer.
  - `[TotalAttendanceInSeconds <Int32?>]`: Total duration of the attendances in seconds.

IDENTITY `<IMicrosoftGraphIdentity>`: identity
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
  - `[Id <String>]`: Unique identifier for the identity.

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
