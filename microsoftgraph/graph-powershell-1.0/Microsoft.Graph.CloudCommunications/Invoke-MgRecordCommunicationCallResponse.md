---
external help file: Microsoft.Graph.CloudCommunications-help.xml
Module Name: Microsoft.Graph.CloudCommunications
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.cloudcommunications/invoke-mgrecordcommunicationcallresponse
schema: 2.0.0
---

# Invoke-MgRecordCommunicationCallResponse

## SYNOPSIS
Records a short audio response from the caller.\nA bot can utilize this to capture a voice response from a caller after they are prompted for a response.
For further information on how to handle operations, please review commsOperation This action is not intended to record the entire call.
The maximum length of recording is 2 minutes.
The recording is not saved permanently by the Cloud Communications Platform and is discarded shortly after the call ends.
The bot must download the recording promptly after the recording operation finishes by using the recordingLocation value that's given in the completed notification.

## SYNTAX

### RecordExpanded (Default)
```
Invoke-MgRecordCommunicationCallResponse -CallId <String> [-AdditionalProperties <Hashtable>] [-BargeInAllowed]
 [-ClientContext <String>] [-InitialSilenceTimeoutInSeconds <Int32>] [-MaxRecordDurationInSeconds <Int32>]
 [-MaxSilenceTimeoutInSeconds <Int32>] [-PlayBeep] [-Prompts <IMicrosoftGraphPrompt[]>] [-StopTones <String[]>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Record
```
Invoke-MgRecordCommunicationCallResponse -CallId <String>
 -BodyParameter <IPaths14Wb7KqCommunicationsCallsCallIdMicrosoftGraphRecordresponsePostRequestbodyContentApplicationJsonSchema1>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### RecordViaIdentityExpanded
```
Invoke-MgRecordCommunicationCallResponse -InputObject <ICloudCommunicationsIdentity>
 [-AdditionalProperties <Hashtable>] [-BargeInAllowed] [-ClientContext <String>]
 [-InitialSilenceTimeoutInSeconds <Int32>] [-MaxRecordDurationInSeconds <Int32>]
 [-MaxSilenceTimeoutInSeconds <Int32>] [-PlayBeep] [-Prompts <IMicrosoftGraphPrompt[]>] [-StopTones <String[]>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### RecordViaIdentity
```
Invoke-MgRecordCommunicationCallResponse -InputObject <ICloudCommunicationsIdentity>
 -BodyParameter <IPaths14Wb7KqCommunicationsCallsCallIdMicrosoftGraphRecordresponsePostRequestbodyContentApplicationJsonSchema1>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Records a short audio response from the caller.\nA bot can utilize this to capture a voice response from a caller after they are prompted for a response.
For further information on how to handle operations, please review commsOperation This action is not intended to record the entire call.
The maximum length of recording is 2 minutes.
The recording is not saved permanently by the Cloud Communications Platform and is discarded shortly after the call ends.
The bot must download the recording promptly after the recording operation finishes by using the recordingLocation value that's given in the completed notification.

## EXAMPLES

### Example 1: Using the Invoke-MgRecordCommunicationCallResponse Cmdlet
```powershell
Import-Module Microsoft.Graph.CloudCommunications
$params = @{
	BargeInAllowed = $true
	ClientContext = "d45324c1-fcb5-430a-902c-f20af696537c"
	Prompts = @(
		@{
			"@odata.type" = "#microsoft.graph.mediaPrompt"
		}
	)
	MaxRecordDurationInSeconds = 10
	InitialSilenceTimeoutInSeconds = 5
	MaxSilenceTimeoutInSeconds = 2
	PlayBeep = $true
	StopTones = @(
		"#"
		"1"
		"*"
	)
}
Invoke-MgRecordCommunicationCallResponse -CallId $callId -BodyParameter $params
```

This example shows how to use the Invoke-MgRecordCommunicationCallResponse Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: RecordExpanded, RecordViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BargeInAllowed
.

```yaml
Type: SwitchParameter
Parameter Sets: RecordExpanded, RecordViaIdentityExpanded
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
Type: IPaths14Wb7KqCommunicationsCallsCallIdMicrosoftGraphRecordresponsePostRequestbodyContentApplicationJsonSchema1
Parameter Sets: Record, RecordViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CallId
key: id of call

```yaml
Type: String
Parameter Sets: RecordExpanded, Record
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ClientContext
.

```yaml
Type: String
Parameter Sets: RecordExpanded, RecordViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InitialSilenceTimeoutInSeconds
.

```yaml
Type: Int32
Parameter Sets: RecordExpanded, RecordViaIdentityExpanded
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
Parameter Sets: RecordViaIdentityExpanded, RecordViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MaxRecordDurationInSeconds
.

```yaml
Type: Int32
Parameter Sets: RecordExpanded, RecordViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MaxSilenceTimeoutInSeconds
.

```yaml
Type: Int32
Parameter Sets: RecordExpanded, RecordViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PlayBeep
.

```yaml
Type: SwitchParameter
Parameter Sets: RecordExpanded, RecordViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Prompts
.

```yaml
Type: IMicrosoftGraphPrompt[]
Parameter Sets: RecordExpanded, RecordViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StopTones
.

```yaml
Type: String[]
Parameter Sets: RecordExpanded, RecordViaIdentityExpanded
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

### Microsoft.Graph.PowerShell.Models.ICloudCommunicationsIdentity
### Microsoft.Graph.PowerShell.Models.IPaths14Wb7KqCommunicationsCallsCallIdMicrosoftGraphRecordresponsePostRequestbodyContentApplicationJsonSchema1
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphRecordOperation
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IPaths14Wb7KqCommunicationsCallsCallIdMicrosoftGraphRecordresponsePostRequestbodyContentApplicationJsonSchema1>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[BargeInAllowed <Boolean?>]`: 
  - `[ClientContext <String>]`: 
  - `[InitialSilenceTimeoutInSeconds <Int32?>]`: 
  - `[MaxRecordDurationInSeconds <Int32?>]`: 
  - `[MaxSilenceTimeoutInSeconds <Int32?>]`: 
  - `[PlayBeep <Boolean?>]`: 
  - `[Prompts <IMicrosoftGraphPrompt[]>]`: 
  - `[StopTones <String[]>]`: 

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
