---
external help file: Microsoft.Graph.CloudCommunications-help.xml
Module Name: Microsoft.Graph.CloudCommunications
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.cloudcommunications/new-mgcommunicationcall
schema: 2.0.0
ms.prod: cloud-communications
---

# New-MgCommunicationCall

## SYNOPSIS
Create call enables your bot to create a new outgoing peer-to-peer or group call, or join an existing meeting.
You will need to register the calling bot and go through the list of permissions needed as mentioned below.

## SYNTAX

### CreateExpanded (Default)
```
New-MgCommunicationCall [-AdditionalProperties <Hashtable>]
 [-AudioRoutingGroups <IMicrosoftGraphAudioRoutingGroup[]>] [-CallChainId <String>]
 [-CallOptions <IMicrosoftGraphCallOptions>] [-CallRoutes <IMicrosoftGraphCallRoute[]>] [-CallbackUri <String>]
 [-ChatInfo <IMicrosoftGraphChatInfo>] [-ContentSharingSessions <IMicrosoftGraphContentSharingSession[]>]
 [-Direction <String>] [-Id <String>] [-IncomingContext <IMicrosoftGraphIncomingContext>]
 [-MediaConfig <Hashtable>] [-MediaState <IMicrosoftGraphCallMediaState>] [-MeetingInfo <Hashtable>]
 [-MyParticipantId <String>] [-Operations <IMicrosoftGraphCommsOperation[]>]
 [-Participants <IMicrosoftGraphParticipant[]>] [-RequestedModalities <String[]>]
 [-ResultInfo <IMicrosoftGraphResultInfo>] [-Source <IMicrosoftGraphParticipantInfo>] [-State <String>]
 [-Subject <String>] [-Targets <IMicrosoftGraphInvitationParticipantInfo[]>] [-TenantId <String>]
 [-ToneInfo <IMicrosoftGraphToneInfo>] [-Transcription <IMicrosoftGraphCallTranscriptionInfo>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgCommunicationCall -BodyParameter <IMicrosoftGraphCall> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create call enables your bot to create a new outgoing peer-to-peer or group call, or join an existing meeting.
You will need to register the calling bot and go through the list of permissions needed as mentioned below.

## EXAMPLES

### Example 1: Using the New-MgCommunicationCall Cmdlet
```powershell
Import-Module Microsoft.Graph.CloudCommunications
$params = @{
	"@odata.type" = "#microsoft.graph.call"
	CallbackUri = "https://bot.contoso.com/callback"
	Source = @{
		"@odata.type" = "#microsoft.graph.participantInfo"
		Identity = @{
			"@odata.type" = "#microsoft.graph.identitySet"
			Application = @{
				"@odata.type" = "#microsoft.graph.identity"
				DisplayName = "Calling Bot"
				Id = "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
			}
		}
		Region = $null
		LanguageId = $null
	}
	Targets = @(
		@{
			"@odata.type" = "#microsoft.graph.invitationParticipantInfo"
			Identity = @{
				"@odata.type" = "#microsoft.graph.identitySet"
				User = @{
					"@odata.type" = "#microsoft.graph.identity"
					DisplayName = "John"
					Id = "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
				}
			}
		}
	)
	RequestedModalities = @(
		"audio"
	)
	MediaConfig = @{
		"@odata.type" = "#microsoft.graph.appHostedMediaConfig"
		Blob = "<Media Session Configuration>"
	}
}
New-MgCommunicationCall -BodyParameter $params
```

This example shows how to use the New-MgCommunicationCall Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

### Example 2: Using the New-MgCommunicationCall Cmdlet
```powershell
Import-Module Microsoft.Graph.CloudCommunications
$params = @{
	"@odata.type" = "#microsoft.graph.call"
	CallbackUri = "https://bot.contoso.com/callback"
	Targets = @(
		@{
			"@odata.type" = "#microsoft.graph.invitationParticipantInfo"
			Identity = @{
				"@odata.type" = "#microsoft.graph.identitySet"
				User = @{
					"@odata.type" = "#microsoft.graph.identity"
					DisplayName = "John"
					Id = "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
				}
			}
		}
	)
	RequestedModalities = @(
		"audio"
	)
	MediaConfig = @{
		"@odata.type" = "#microsoft.graph.serviceHostedMediaConfig"
	}
}
New-MgCommunicationCall -BodyParameter $params
```

This example shows how to use the New-MgCommunicationCall Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

### Example 3: Using the New-MgCommunicationCall Cmdlet
```powershell
Import-Module Microsoft.Graph.CloudCommunications
$params = @{
	"@odata.type" = "#microsoft.graph.call"
	CallbackUri = "https://bot.contoso.com/callback"
	Source = @{
		"@odata.type" = "#microsoft.graph.participantInfo"
		Identity = @{
			"@odata.type" = "#microsoft.graph.identitySet"
			ApplicationInstance = @{
				"@odata.type" = "#microsoft.graph.identity"
				DisplayName = "Calling Bot"
				Id = "3d913abb-aec0-4964-8fa6-3c6850c4f278"
			}
		}
		CountryCode = $null
		EndpointType = $null
		Region = $null
		LanguageId = $null
	}
	Targets = @(
		@{
			"@odata.type" = "#microsoft.graph.invitationParticipantInfo"
			Identity = @{
				"@odata.type" = "#microsoft.graph.identitySet"
				Phone = @{
					"@odata.type" = "#microsoft.graph.identity"
					Id = "+12345678901"
				}
			}
		}
	)
	RequestedModalities = @(
		"audio"
	)
	MediaConfig = @{
		"@odata.type" = "#microsoft.graph.serviceHostedMediaConfig"
	}
	TenantId = "aa67bd4c-8475-432d-bd41-39f255720e0a"
}
New-MgCommunicationCall -BodyParameter $params
```

This example shows how to use the New-MgCommunicationCall Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

### Example 4: Using the New-MgCommunicationCall Cmdlet
```powershell
Import-Module Microsoft.Graph.CloudCommunications
$params = @{
	"@odata.type" = "#microsoft.graph.call"
	CallbackUri = "https://bot.contoso.com/callback"
	Source = @{
		"@odata.type" = "#microsoft.graph.participantInfo"
		Identity = @{
			"@odata.type" = "#microsoft.graph.identitySet"
			ApplicationInstance = @{
				"@odata.type" = "#microsoft.graph.identity"
				DisplayName = "Calling Bot"
				Id = "3d913abb-aec0-4964-8fa6-3c6850c4f278"
			}
		}
		CountryCode = $null
		EndpointType = $null
		Region = $null
		LanguageId = $null
	}
	Targets = @(
		@{
			"@odata.type" = "#microsoft.graph.invitationParticipantInfo"
			Identity = @{
				"@odata.type" = "#microsoft.graph.identitySet"
				Phone = @{
					"@odata.type" = "#microsoft.graph.identity"
					Id = "+12345678901"
				}
			}
		}
	)
	RequestedModalities = @(
		"audio"
	)
	MediaConfig = @{
		"@odata.type" = "#microsoft.graph.appHostedMediaConfig"
		Blob = "<Media Session Configuration>"
	}
	TenantId = "aa67bd4c-8475-432d-bd41-39f255720e0a"
}
New-MgCommunicationCall -BodyParameter $params
```

This example shows how to use the New-MgCommunicationCall Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AudioRoutingGroups
.
To construct, please use Get-Help -Online and see NOTES section for AUDIOROUTINGGROUPS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAudioRoutingGroup[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
call
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphCall
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CallbackUri
The callback URL on which callbacks will be delivered.
Must be https.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CallChainId
A unique identifier for all the participant calls in a conference or a unique identifier for two participant calls in a P2P call.
This needs to be copied over from Microsoft.Graph.Call.CallChainId.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CallOptions
callOptions
To construct, please use Get-Help -Online and see NOTES section for CALLOPTIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphCallOptions
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CallRoutes
The routing information on how the call was retargeted.
Read-only.
To construct, please use Get-Help -Online and see NOTES section for CALLROUTES properties and create a hash table.

```yaml
Type: IMicrosoftGraphCallRoute[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ChatInfo
chatInfo
To construct, please use Get-Help -Online and see NOTES section for CHATINFO properties and create a hash table.

```yaml
Type: IMicrosoftGraphChatInfo
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ContentSharingSessions
.
To construct, please use Get-Help -Online and see NOTES section for CONTENTSHARINGSESSIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphContentSharingSession[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Direction
callDirection

```yaml
Type: String
Parameter Sets: CreateExpanded
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
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IncomingContext
incomingContext
To construct, please use Get-Help -Online and see NOTES section for INCOMINGCONTEXT properties and create a hash table.

```yaml
Type: IMicrosoftGraphIncomingContext
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MediaConfig
mediaConfig

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MediaState
callMediaState
To construct, please use Get-Help -Online and see NOTES section for MEDIASTATE properties and create a hash table.

```yaml
Type: IMicrosoftGraphCallMediaState
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MeetingInfo
meetingInfo

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MyParticipantId
.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Operations
.
To construct, please use Get-Help -Online and see NOTES section for OPERATIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphCommsOperation[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Participants
.
To construct, please use Get-Help -Online and see NOTES section for PARTICIPANTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphParticipant[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RequestedModalities
The list of requested modalities.
Possible values are: unknown, audio, video, videoBasedScreenSharing, data.

```yaml
Type: String[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResultInfo
resultInfo
To construct, please use Get-Help -Online and see NOTES section for RESULTINFO properties and create a hash table.

```yaml
Type: IMicrosoftGraphResultInfo
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Source
participantInfo
To construct, please use Get-Help -Online and see NOTES section for SOURCE properties and create a hash table.

```yaml
Type: IMicrosoftGraphParticipantInfo
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -State
.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Subject
The subject of the conversation.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Targets
The targets of the call.
Required information for creating peer to peer call.
To construct, please use Get-Help -Online and see NOTES section for TARGETS properties and create a hash table.

```yaml
Type: IMicrosoftGraphInvitationParticipantInfo[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TenantId
.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ToneInfo
toneInfo
To construct, please use Get-Help -Online and see NOTES section for TONEINFO properties and create a hash table.

```yaml
Type: IMicrosoftGraphToneInfo
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Transcription
callTranscriptionInfo
To construct, please use Get-Help -Online and see NOTES section for TRANSCRIPTION properties and create a hash table.

```yaml
Type: IMicrosoftGraphCallTranscriptionInfo
Parameter Sets: CreateExpanded
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphCall
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphCall
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


AUDIOROUTINGGROUPS <IMicrosoftGraphAudioRoutingGroup\[]>: .
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[Receivers <String[]>]`: 
  - `[RoutingMode <String>]`: 
  - `[Sources <String[]>]`: 

BODYPARAMETER `<IMicrosoftGraphCall>`: call
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[AudioRoutingGroups <IMicrosoftGraphAudioRoutingGroup[]>]`: 
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[Receivers <String[]>]`: 
    - `[RoutingMode <String>]`: 
    - `[Sources <String[]>]`: 
  - `[CallChainId <String>]`: A unique identifier for all the participant calls in a conference or a unique identifier for two participant calls in a P2P call.  This needs to be copied over from Microsoft.Graph.Call.CallChainId.
  - `[CallOptions <IMicrosoftGraphCallOptions>]`: callOptions
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[HideBotAfterEscalation <Boolean?>]`: Indicates whether to hide the app after the call is escalated.
    - `[IsContentSharingNotificationEnabled <Boolean?>]`: Indicates whether content sharing notifications should be enabled for the call.
  - `[CallRoutes <IMicrosoftGraphCallRoute[]>]`: The routing information on how the call was retargeted. Read-only.
    - `[Final <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Application <IMicrosoftGraphIdentity>]`: identity
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
        - `[Id <String>]`: Unique identifier for the identity.
      - `[Device <IMicrosoftGraphIdentity>]`: identity
      - `[User <IMicrosoftGraphIdentity>]`: identity
    - `[Original <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[RoutingType <String>]`: routingType
  - `[CallbackUri <String>]`: The callback URL on which callbacks will be delivered. Must be https.
  - `[ChatInfo <IMicrosoftGraphChatInfo>]`: chatInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[MessageId <String>]`: The unique identifier of a message in a Microsoft Teams channel.
    - `[ReplyChainMessageId <String>]`: The ID of the reply message.
    - `[ThreadId <String>]`: The unique identifier for a thread in Microsoft Teams.
  - `[ContentSharingSessions <IMicrosoftGraphContentSharingSession[]>]`: 
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[Direction <String>]`: callDirection
  - `[IncomingContext <IMicrosoftGraphIncomingContext>]`: incomingContext
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ObservedParticipantId <String>]`: The ID of the participant that is under observation. Read-only.
    - `[OnBehalfOf <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[SourceParticipantId <String>]`: The ID of the participant that triggered the incoming call. Read-only.
    - `[Transferor <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[MediaConfig <IMicrosoftGraphMediaConfig>]`: mediaConfig
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[MediaState <IMicrosoftGraphCallMediaState>]`: callMediaState
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Audio <String>]`: mediaState
  - `[MeetingInfo <IMicrosoftGraphMeetingInfo>]`: meetingInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[MyParticipantId <String>]`: 
  - `[Operations <IMicrosoftGraphCommsOperation[]>]`: 
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[ClientContext <String>]`: Unique Client Context string. Max limit is 256 chars.
    - `[ResultInfo <IMicrosoftGraphResultInfo>]`: resultInfo
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Code <Int32?>]`: The result code.
      - `[Message <String>]`: The message.
      - `[Subcode <Int32?>]`: The result sub-code.
    - `[Status <String>]`: operationStatus
  - `[Participants <IMicrosoftGraphParticipant[]>]`: 
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[Info <IMicrosoftGraphParticipantInfo>]`: participantInfo
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[CountryCode <String>]`: The ISO 3166-1 Alpha-2 country code of the participant's best estimated physical location at the start of the call. Read-only.
      - `[EndpointType <String>]`: endpointType
      - `[Identity <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[LanguageId <String>]`: The language culture string. Read-only.
      - `[ParticipantId <String>]`: The participant ID of the participant. Read-only.
      - `[Region <String>]`: The home region of the participant. This can be a country, a continent, or a larger geographic region. This does not change based on the participant's current physical location. Read-only.
    - `[IsInLobby <Boolean?>]`: true if the participant is in lobby.
    - `[IsMuted <Boolean?>]`: true if the participant is muted (client or server muted).
    - `[MediaStreams <IMicrosoftGraphMediaStream[]>]`: The list of media streams.
      - `[Direction <String>]`: mediaDirection
      - `[Label <String>]`: The media stream label.
      - `[MediaType <String>]`: 
      - `[ServerMuted <Boolean?>]`: If the media is muted by the server.
      - `[SourceId <String>]`: The source ID.
    - `[Metadata <String>]`: A blob of data provided by the participant in the roster.
    - `[RecordingInfo <IMicrosoftGraphRecordingInfo>]`: recordingInfo
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Initiator <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[RecordingStatus <String>]`: recordingStatus
  - `[RequestedModalities <String[]>]`: The list of requested modalities. Possible values are: unknown, audio, video, videoBasedScreenSharing, data.
  - `[ResultInfo <IMicrosoftGraphResultInfo>]`: resultInfo
  - `[Source <IMicrosoftGraphParticipantInfo>]`: participantInfo
  - `[State <String>]`: 
  - `[Subject <String>]`: The subject of the conversation.
  - `[Targets <IMicrosoftGraphInvitationParticipantInfo[]>]`: The targets of the call. Required information for creating peer to peer call.
    - `[Hidden <Boolean?>]`: Optional. Whether to hide the participant from the roster.
    - `[Identity <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[ParticipantId <String>]`: Optional. The ID of the target participant.
    - `[RemoveFromDefaultAudioRoutingGroup <Boolean?>]`: Optional. Whether to remove them from the main mixer.
    - `[ReplacesCallId <String>]`: Optional. The call which the target identity is currently a part of. For peer-to-peer case, the call will be dropped once the participant is added successfully.
  - `[TenantId <String>]`: 
  - `[ToneInfo <IMicrosoftGraphToneInfo>]`: toneInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[SequenceId <Int64?>]`: An incremental identifier used for ordering DTMF events.
    - `[Tone <String>]`: tone
  - `[Transcription <IMicrosoftGraphCallTranscriptionInfo>]`: callTranscriptionInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[LastModifiedDateTime <DateTime?>]`: The state modified time in UTC.
    - `[State <String>]`: callTranscriptionState

CALLOPTIONS `<IMicrosoftGraphCallOptions>`: callOptions
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[HideBotAfterEscalation <Boolean?>]`: Indicates whether to hide the app after the call is escalated.
  - `[IsContentSharingNotificationEnabled <Boolean?>]`: Indicates whether content sharing notifications should be enabled for the call.

CALLROUTES <IMicrosoftGraphCallRoute\[]>: The routing information on how the call was retargeted. Read-only.
  - `[Final <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[Original <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[RoutingType <String>]`: routingType

CHATINFO `<IMicrosoftGraphChatInfo>`: chatInfo
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[MessageId <String>]`: The unique identifier of a message in a Microsoft Teams channel.
  - `[ReplyChainMessageId <String>]`: The ID of the reply message.
  - `[ThreadId <String>]`: The unique identifier for a thread in Microsoft Teams.

CONTENTSHARINGSESSIONS <IMicrosoftGraphContentSharingSession\[]>: .
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.

INCOMINGCONTEXT `<IMicrosoftGraphIncomingContext>`: incomingContext
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ObservedParticipantId <String>]`: The ID of the participant that is under observation. Read-only.
  - `[OnBehalfOf <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[SourceParticipantId <String>]`: The ID of the participant that triggered the incoming call. Read-only.
  - `[Transferor <IMicrosoftGraphIdentitySet>]`: identitySet

MEDIASTATE `<IMicrosoftGraphCallMediaState>`: callMediaState
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Audio <String>]`: mediaState

OPERATIONS <IMicrosoftGraphCommsOperation\[]>: .
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[ClientContext <String>]`: Unique Client Context string. Max limit is 256 chars.
  - `[ResultInfo <IMicrosoftGraphResultInfo>]`: resultInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Code <Int32?>]`: The result code.
    - `[Message <String>]`: The message.
    - `[Subcode <Int32?>]`: The result sub-code.
  - `[Status <String>]`: operationStatus

PARTICIPANTS <IMicrosoftGraphParticipant\[]>: .
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[Info <IMicrosoftGraphParticipantInfo>]`: participantInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[CountryCode <String>]`: The ISO 3166-1 Alpha-2 country code of the participant's best estimated physical location at the start of the call. Read-only.
    - `[EndpointType <String>]`: endpointType
    - `[Identity <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Application <IMicrosoftGraphIdentity>]`: identity
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
        - `[Id <String>]`: Unique identifier for the identity.
      - `[Device <IMicrosoftGraphIdentity>]`: identity
      - `[User <IMicrosoftGraphIdentity>]`: identity
    - `[LanguageId <String>]`: The language culture string. Read-only.
    - `[ParticipantId <String>]`: The participant ID of the participant. Read-only.
    - `[Region <String>]`: The home region of the participant. This can be a country, a continent, or a larger geographic region. This does not change based on the participant's current physical location. Read-only.
  - `[IsInLobby <Boolean?>]`: true if the participant is in lobby.
  - `[IsMuted <Boolean?>]`: true if the participant is muted (client or server muted).
  - `[MediaStreams <IMicrosoftGraphMediaStream[]>]`: The list of media streams.
    - `[Direction <String>]`: mediaDirection
    - `[Label <String>]`: The media stream label.
    - `[MediaType <String>]`: 
    - `[ServerMuted <Boolean?>]`: If the media is muted by the server.
    - `[SourceId <String>]`: The source ID.
  - `[Metadata <String>]`: A blob of data provided by the participant in the roster.
  - `[RecordingInfo <IMicrosoftGraphRecordingInfo>]`: recordingInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Initiator <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[RecordingStatus <String>]`: recordingStatus

RESULTINFO `<IMicrosoftGraphResultInfo>`: resultInfo
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Code <Int32?>]`: The result code.
  - `[Message <String>]`: The message.
  - `[Subcode <Int32?>]`: The result sub-code.

SOURCE `<IMicrosoftGraphParticipantInfo>`: participantInfo
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[CountryCode <String>]`: The ISO 3166-1 Alpha-2 country code of the participant's best estimated physical location at the start of the call. Read-only.
  - `[EndpointType <String>]`: endpointType
  - `[Identity <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[LanguageId <String>]`: The language culture string. Read-only.
  - `[ParticipantId <String>]`: The participant ID of the participant. Read-only.
  - `[Region <String>]`: The home region of the participant. This can be a country, a continent, or a larger geographic region. This does not change based on the participant's current physical location. Read-only.

TARGETS <IMicrosoftGraphInvitationParticipantInfo\[]>: The targets of the call. Required information for creating peer to peer call.
  - `[Hidden <Boolean?>]`: Optional. Whether to hide the participant from the roster.
  - `[Identity <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity. Note that this might not always be available or up to date. For example, if a user changes their display name, the API might show the new value in a future response, but the items associated with the user won't show up as having changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[ParticipantId <String>]`: Optional. The ID of the target participant.
  - `[RemoveFromDefaultAudioRoutingGroup <Boolean?>]`: Optional. Whether to remove them from the main mixer.
  - `[ReplacesCallId <String>]`: Optional. The call which the target identity is currently a part of. For peer-to-peer case, the call will be dropped once the participant is added successfully.

TONEINFO `<IMicrosoftGraphToneInfo>`: toneInfo
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[SequenceId <Int64?>]`: An incremental identifier used for ordering DTMF events.
  - `[Tone <String>]`: tone

TRANSCRIPTION `<IMicrosoftGraphCallTranscriptionInfo>`: callTranscriptionInfo
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[LastModifiedDateTime <DateTime?>]`: The state modified time in UTC.
  - `[State <String>]`: callTranscriptionState

## RELATED LINKS

## RELATED LINKS
