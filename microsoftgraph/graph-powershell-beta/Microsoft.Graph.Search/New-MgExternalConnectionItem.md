---
external help file: Microsoft.Graph.Search-help.xml
Module Name: Microsoft.Graph.Search
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.search/new-mgexternalconnectionitem
schema: 2.0.0
---

# New-MgExternalConnectionItem

## SYNOPSIS
Create new navigation property to items for external

## SYNTAX

### CreateExpanded (Default)
```
New-MgExternalConnectionItem -ExternalConnectionId <String> [-Acl <IMicrosoftGraphExternalConnectorsAcl[]>]
 [-Activities <IMicrosoftGraphExternalConnectorsExternalActivity[]>] [-AdditionalProperties <Hashtable>]
 [-Content <IMicrosoftGraphExternalConnectorsExternalItemContent>] [-Id <String>] [-Properties <Hashtable>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgExternalConnectionItem -ExternalConnectionId <String>
 -BodyParameter <IMicrosoftGraphExternalConnectorsExternalItem> [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgExternalConnectionItem -InputObject <ISearchIdentity> [-Acl <IMicrosoftGraphExternalConnectorsAcl[]>]
 [-Activities <IMicrosoftGraphExternalConnectorsExternalActivity[]>] [-AdditionalProperties <Hashtable>]
 [-Content <IMicrosoftGraphExternalConnectorsExternalItemContent>] [-Id <String>] [-Properties <Hashtable>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgExternalConnectionItem -InputObject <ISearchIdentity>
 -BodyParameter <IMicrosoftGraphExternalConnectorsExternalItem> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to items for external

## EXAMPLES

## PARAMETERS

### -Acl
An array of access control entries.
Each entry specifies the access granted to a user or group.
Required.
To construct, please use Get-Help -Online and see NOTES section for ACL properties and create a hash table.

```yaml
Type: IMicrosoftGraphExternalConnectorsAcl[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Activities
Write-only property.
Returns results.
To construct, please use Get-Help -Online and see NOTES section for ACTIVITIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphExternalConnectorsExternalActivity[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
externalItem
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphExternalConnectorsExternalItem
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Content
externalItemContent
To construct, please use Get-Help -Online and see NOTES section for CONTENT properties and create a hash table.

```yaml
Type: IMicrosoftGraphExternalConnectorsExternalItemContent
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExternalConnectionId
key: id of externalConnection

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

### -InputObject
Identity Parameter
To construct, please use Get-Help -Online and see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: ISearchIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Properties
properties

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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphExternalConnectorsExternalItem
### Microsoft.Graph.PowerShell.Models.ISearchIdentity
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphExternalConnectorsExternalItem
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


ACL <IMicrosoftGraphExternalConnectorsAcl\[]>: An array of access control entries. Each entry specifies the access granted to a user or group. Required.
  - `[AccessType <String>]`: accessType
  - `[IdentitySource <String>]`: identitySourceType
  - `[Type <String>]`: aclType
  - `[Value <String>]`: The unique identifer of the identity. In case of Azure Active Directory identities, value is set to the object identifier of the user, group or tenant for types user, group and everyone (and everyoneExceptGuests) respectively. In case of external groups value is set to the ID of the externalGroup.

ACTIVITIES <IMicrosoftGraphExternalConnectorsExternalActivity\[]>: Write-only property. Returns results.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[PerformedBy <IMicrosoftGraphExternalConnectorsIdentity>]`: identity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[Type <String>]`: identityType
  - `[StartDateTime <DateTime?>]`: When the particular activity occurred.
  - `[Type <String>]`: externalActivityType

BODYPARAMETER `<IMicrosoftGraphExternalConnectorsExternalItem>`: externalItem
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[Acl <IMicrosoftGraphExternalConnectorsAcl[]>]`: An array of access control entries. Each entry specifies the access granted to a user or group. Required.
    - `[AccessType <String>]`: accessType
    - `[IdentitySource <String>]`: identitySourceType
    - `[Type <String>]`: aclType
    - `[Value <String>]`: The unique identifer of the identity. In case of Azure Active Directory identities, value is set to the object identifier of the user, group or tenant for types user, group and everyone (and everyoneExceptGuests) respectively. In case of external groups value is set to the ID of the externalGroup.
  - `[Activities <IMicrosoftGraphExternalConnectorsExternalActivity[]>]`: Write-only property. Returns results.
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[PerformedBy <IMicrosoftGraphExternalConnectorsIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique idenfier for an entity. Read-only.
      - `[Type <String>]`: identityType
    - `[StartDateTime <DateTime?>]`: When the particular activity occurred.
    - `[Type <String>]`: externalActivityType
  - `[Content <IMicrosoftGraphExternalConnectorsExternalItemContent>]`: externalItemContent
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Type <String>]`: externalItemContentType
    - `[Value <String>]`: The content for the externalItem. Required.
  - `[Properties <IMicrosoftGraphExternalConnectorsProperties>]`: properties
    - `[(Any) <Object>]`: This indicates any property can be added to this object.

CONTENT `<IMicrosoftGraphExternalConnectorsExternalItemContent>`: externalItemContent
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Type <String>]`: externalItemContentType
  - `[Value <String>]`: The content for the externalItem. Required.

INPUTOBJECT `<ISearchIdentity>`: Identity Parameter
  - `[AcronymId <String>]`: key: id of acronym
  - `[BookmarkId <String>]`: key: id of bookmark
  - `[ConnectionOperationId <String>]`: key: id of connectionOperation
  - `[ExternalActivityId <String>]`: key: id of externalActivity
  - `[ExternalConnectionId <String>]`: key: id of externalConnection
  - `[ExternalGroupId <String>]`: key: id of externalGroup
  - `[ExternalItemId <String>]`: key: id of externalItem
  - `[IdentityId <String>]`: key: id of identity
  - `[QnaId <String>]`: key: id of qna

## RELATED LINKS
