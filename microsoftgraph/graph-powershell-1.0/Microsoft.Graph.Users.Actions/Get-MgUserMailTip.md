---
external help file: Microsoft.Graph.Users.Actions-help.xml
Module Name: Microsoft.Graph.Users.Actions
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.users.actions/get-mgusermailtip
schema: 2.0.0
---

# Get-MgUserMailTip

## SYNOPSIS
Get the MailTips of one or more recipients as available to the signed-in user.
Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to \nbe returned for more than one recipient at one time.
The requested MailTips are returned in a mailTips collection.

## SYNTAX

### GetExpanded1 (Default)
```
Get-MgUserMailTip -UserId <String> [-AdditionalProperties <Hashtable>] [-EmailAddresses <String[]>]
 [-MailTipsOptions <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Get1
```
Get-MgUserMailTip -UserId <String>
 -BodyParameter <IComponentsM2Vn8QRequestbodiesGetmailtipsrequestbodyContentApplicationJsonSchema> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### GetViaIdentityExpanded1
```
Get-MgUserMailTip -InputObject <IUsersActionsIdentity> [-AdditionalProperties <Hashtable>]
 [-EmailAddresses <String[]>] [-MailTipsOptions <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### GetViaIdentity1
```
Get-MgUserMailTip -InputObject <IUsersActionsIdentity>
 -BodyParameter <IComponentsM2Vn8QRequestbodiesGetmailtipsrequestbodyContentApplicationJsonSchema> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Get the MailTips of one or more recipients as available to the signed-in user.
Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to \nbe returned for more than one recipient at one time.
The requested MailTips are returned in a mailTips collection.

## EXAMPLES

### Example 1: Using the Get-MgUserMailTip Cmdlet
```powershell
Import-Module Microsoft.Graph.Users.Actions
$params = @{
	EmailAddresses = @(
		"danas@contoso.onmicrosoft.com"
		"fannyd@contoso.onmicrosoft.com"
	)
	MailTipsOptions = "automaticReplies, mailboxFullStatus"
}
# A UPN can also be used as -UserId.
Get-MgUserMailTip -UserId $userId -BodyParameter $params
```

This example shows how to use the Get-MgUserMailTip Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: GetExpanded1, GetViaIdentityExpanded1
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
Type: IComponentsM2Vn8QRequestbodiesGetmailtipsrequestbodyContentApplicationJsonSchema
Parameter Sets: Get1, GetViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -EmailAddresses
.

```yaml
Type: String[]
Parameter Sets: GetExpanded1, GetViaIdentityExpanded1
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
Type: IUsersActionsIdentity
Parameter Sets: GetViaIdentityExpanded1, GetViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MailTipsOptions
mailTipsType

```yaml
Type: String
Parameter Sets: GetExpanded1, GetViaIdentityExpanded1
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
Parameter Sets: GetExpanded1, Get1
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

### Microsoft.Graph.PowerShell.Models.IComponentsM2Vn8QRequestbodiesGetmailtipsrequestbodyContentApplicationJsonSchema
### Microsoft.Graph.PowerShell.Models.IUsersActionsIdentity
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphMailTips
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IComponentsM2Vn8QRequestbodiesGetmailtipsrequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[EmailAddresses <String[]>]`: 
  - `[MailTipsOptions <String>]`: mailTipsType

INPUTOBJECT `<IUsersActionsIdentity>`: Identity Parameter
  - `[AccessReviewInstanceId <String>]`: key: id of accessReviewInstance
  - `[AccessReviewStageId <String>]`: key: id of accessReviewStage
  - `[AppLogCollectionRequestId <String>]`: key: id of appLogCollectionRequest
  - `[AuthenticationMethodId <String>]`: key: id of authenticationMethod
  - `[CalendarId <String>]`: key: id of calendar
  - `[ChatId <String>]`: key: id of chat
  - `[ChatMessageId <String>]`: key: id of chatMessage
  - `[ChatMessageId1 <String>]`: key: id of chatMessage
  - `[CloudPcId <String>]`: key: id of cloudPC
  - `[ContentTypeId <String>]`: key: id of contentType
  - `[DeviceEnrollmentConfigurationId <String>]`: key: id of deviceEnrollmentConfiguration
  - `[DeviceId <String>]`: key: id of device
  - `[DeviceLogCollectionResponseId <String>]`: key: id of deviceLogCollectionResponse
  - `[DocumentSetVersionId <String>]`: key: id of documentSetVersion
  - `[DriveId <String>]`: key: id of drive
  - `[DriveItemId <String>]`: key: id of driveItem
  - `[DriveItemVersionId <String>]`: key: id of driveItemVersion
  - `[EventId <String>]`: key: id of event
  - `[EventId1 <String>]`: key: id of event
  - `[ListItemId <String>]`: key: id of listItem
  - `[ListItemVersionId <String>]`: key: id of listItemVersion
  - `[MailFolderId <String>]`: key: id of mailFolder
  - `[MailFolderId1 <String>]`: key: id of mailFolder
  - `[ManagedDeviceId <String>]`: key: id of managedDevice
  - `[MessageId <String>]`: key: id of message
  - `[MicrosoftAuthenticatorAuthenticationMethodId <String>]`: key: id of microsoftAuthenticatorAuthenticationMethod
  - `[MobileAppTroubleshootingEventId <String>]`: key: id of mobileAppTroubleshootingEvent
  - `[NotebookId <String>]`: key: id of notebook
  - `[OnenotePageId <String>]`: key: id of onenotePage
  - `[OnenoteSectionId <String>]`: key: id of onenoteSection
  - `[OutlookTaskFolderId <String>]`: key: id of outlookTaskFolder
  - `[OutlookTaskGroupId <String>]`: key: id of outlookTaskGroup
  - `[OutlookTaskId <String>]`: key: id of outlookTask
  - `[PasswordlessMicrosoftAuthenticatorAuthenticationMethodId <String>]`: key: id of passwordlessMicrosoftAuthenticatorAuthenticationMethod
  - `[PermissionId <String>]`: key: id of permission
  - `[PhoneAuthenticationMethodId <String>]`: key: id of phoneAuthenticationMethod
  - `[ResourceSpecificPermissionGrantId <String>]`: key: id of resourceSpecificPermissionGrant
  - `[SensitivityLabelId <String>]`: key: id of sensitivityLabel
  - `[SubscriptionId <String>]`: key: id of subscription
  - `[TeamsAppInstallationId <String>]`: key: id of teamsAppInstallation
  - `[TodoTaskId <String>]`: key: id of todoTask
  - `[TodoTaskListId <String>]`: key: id of todoTaskList
  - `[UserId <String>]`: key: id of user
  - `[WindowsHelloForBusinessAuthenticationMethodId <String>]`: key: id of windowsHelloForBusinessAuthenticationMethod

## RELATED LINKS
