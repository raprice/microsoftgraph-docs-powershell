---
external help file: Microsoft.Graph.DeviceManagement.Administration-help.xml
Module Name: Microsoft.Graph.DeviceManagement.Administration
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.devicemanagement.administration/new-mgdevicemanagementauditevent
schema: 2.0.0
---

# New-MgDeviceManagementAuditEvent

## SYNOPSIS
Create new navigation property to auditEvents for deviceManagement

## SYNTAX

### CreateExpanded1 (Default)
```
New-MgDeviceManagementAuditEvent [-Activity <String>] [-ActivityDateTime <DateTime>]
 [-ActivityOperationType <String>] [-ActivityResult <String>] [-ActivityType <String>]
 [-Actor <IMicrosoftGraphAuditActor1>] [-AdditionalProperties <Hashtable>] [-Category <String>]
 [-ComponentName <String>] [-CorrelationId <String>] [-DisplayName <String>] [-Id <String>]
 [-Resources <IMicrosoftGraphAuditResource1[]>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create1
```
New-MgDeviceManagementAuditEvent -BodyParameter <IMicrosoftGraphAuditEvent> [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to auditEvents for deviceManagement

## EXAMPLES

## PARAMETERS

### -Activity
Friendly name of the activity.

```yaml
Type: String
Parameter Sets: CreateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ActivityDateTime
The date time in UTC when the activity was performed.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ActivityOperationType
The HTTP operation type of the activity.

```yaml
Type: String
Parameter Sets: CreateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ActivityResult
The result of the activity.

```yaml
Type: String
Parameter Sets: CreateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ActivityType
The type of activity that was being performed.

```yaml
Type: String
Parameter Sets: CreateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Actor
A class containing the properties for Audit Actor.
To construct, please use Get-Help -Online and see NOTES section for ACTOR properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuditActor1
Parameter Sets: CreateExpanded1
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
Parameter Sets: CreateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
A class containing the properties for Audit Event.
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuditEvent
Parameter Sets: Create1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Category
Audit category.

```yaml
Type: String
Parameter Sets: CreateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ComponentName
Component name.

```yaml
Type: String
Parameter Sets: CreateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CorrelationId
The client request Id that is used to correlate activity within the system.

```yaml
Type: String
Parameter Sets: CreateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
Event display name.

```yaml
Type: String
Parameter Sets: CreateExpanded1
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
Parameter Sets: CreateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Resources
Resources being modified.
To construct, please use Get-Help -Online and see NOTES section for RESOURCES properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuditResource1[]
Parameter Sets: CreateExpanded1
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAuditEvent
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAuditEvent
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


ACTOR `<IMicrosoftGraphAuditActor1>`: A class containing the properties for Audit Actor.
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ApplicationDisplayName <String>]`: Name of the Application.
  - `[ApplicationId <String>]`: AAD Application Id.
  - `[AuditActorType <String>]`: Actor Type.
  - `[IPAddress <String>]`: IPAddress.
  - `[RemoteTenantId <String>]`: Remote Tenant Id
  - `[RemoteUserId <String>]`: Remote User Id
  - `[ServicePrincipalName <String>]`: Service Principal Name (SPN).
  - `[Type <String>]`: Actor Type.
  - `[UserId <String>]`: User Id.
  - `[UserPermissions <String[]>]`: List of user permissions when the audit was performed.
  - `[UserPrincipalName <String>]`: User Principal Name (UPN).
  - `[UserRoleScopeTags <IMicrosoftGraphRoleScopeTagInfo[]>]`: List of user scope tags when the audit was performed.
    - `[DisplayName <String>]`: Scope Tag Display name.
    - `[RoleScopeTagId <String>]`: Scope Tag Id.

BODYPARAMETER `<IMicrosoftGraphAuditEvent>`: A class containing the properties for Audit Event.
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[Activity <String>]`: Friendly name of the activity.
  - `[ActivityDateTime <DateTime?>]`: The date time in UTC when the activity was performed.
  - `[ActivityOperationType <String>]`: The HTTP operation type of the activity.
  - `[ActivityResult <String>]`: The result of the activity.
  - `[ActivityType <String>]`: The type of activity that was being performed.
  - `[Actor <IMicrosoftGraphAuditActor1>]`: A class containing the properties for Audit Actor.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ApplicationDisplayName <String>]`: Name of the Application.
    - `[ApplicationId <String>]`: AAD Application Id.
    - `[AuditActorType <String>]`: Actor Type.
    - `[IPAddress <String>]`: IPAddress.
    - `[RemoteTenantId <String>]`: Remote Tenant Id
    - `[RemoteUserId <String>]`: Remote User Id
    - `[ServicePrincipalName <String>]`: Service Principal Name (SPN).
    - `[Type <String>]`: Actor Type.
    - `[UserId <String>]`: User Id.
    - `[UserPermissions <String[]>]`: List of user permissions when the audit was performed.
    - `[UserPrincipalName <String>]`: User Principal Name (UPN).
    - `[UserRoleScopeTags <IMicrosoftGraphRoleScopeTagInfo[]>]`: List of user scope tags when the audit was performed.
      - `[DisplayName <String>]`: Scope Tag Display name.
      - `[RoleScopeTagId <String>]`: Scope Tag Id.
  - `[Category <String>]`: Audit category.
  - `[ComponentName <String>]`: Component name.
  - `[CorrelationId <String>]`: The client request Id that is used to correlate activity within the system.
  - `[DisplayName <String>]`: Event display name.
  - `[Resources <IMicrosoftGraphAuditResource1[]>]`: Resources being modified.
    - `[AuditResourceType <String>]`: Audit resource's type.
    - `[DisplayName <String>]`: Display name.
    - `[ModifiedProperties <IMicrosoftGraphAuditProperty[]>]`: List of modified properties.
      - `[DisplayName <String>]`: Display name.
      - `[NewValue <String>]`: New value.
      - `[OldValue <String>]`: Old value.
    - `[ResourceId <String>]`: Audit resource's Id.
    - `[Type <String>]`: Audit resource's type.

RESOURCES <IMicrosoftGraphAuditResource1\[]>: Resources being modified.
  - `[AuditResourceType <String>]`: Audit resource's type.
  - `[DisplayName <String>]`: Display name.
  - `[ModifiedProperties <IMicrosoftGraphAuditProperty[]>]`: List of modified properties.
    - `[DisplayName <String>]`: Display name.
    - `[NewValue <String>]`: New value.
    - `[OldValue <String>]`: Old value.
  - `[ResourceId <String>]`: Audit resource's Id.
  - `[Type <String>]`: Audit resource's type.

## RELATED LINKS
