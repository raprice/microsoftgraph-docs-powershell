---
external help file: Microsoft.Graph.Search-help.xml
Module Name: Microsoft.Graph.Search
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.search/update-mgexternalconnectionitem
schema: 2.0.0
---

# Update-MgExternalConnectionItem

## SYNOPSIS
Update the navigation property items in external

## SYNTAX

### UpdateExpanded1 (Default)
```
Update-MgExternalConnectionItem -ExternalConnectionId <String> -ExternalItemId <String>
 [-Acl <IMicrosoftGraphExternalConnectorsAcl1[]>] [-AdditionalProperties <Hashtable>]
 [-Content <IMicrosoftGraphExternalConnectorsExternalItemContent>] [-Id <String>] [-Properties <Hashtable>]
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update1
```
Update-MgExternalConnectionItem -ExternalConnectionId <String> -ExternalItemId <String>
 -BodyParameter <IMicrosoftGraphExternalConnectorsExternalItem1> [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### UpdateViaIdentityExpanded1
```
Update-MgExternalConnectionItem -InputObject <ISearchIdentity> [-Acl <IMicrosoftGraphExternalConnectorsAcl1[]>]
 [-AdditionalProperties <Hashtable>] [-Content <IMicrosoftGraphExternalConnectorsExternalItemContent>]
 [-Id <String>] [-Properties <Hashtable>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity1
```
Update-MgExternalConnectionItem -InputObject <ISearchIdentity>
 -BodyParameter <IMicrosoftGraphExternalConnectorsExternalItem1> [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property items in external

## EXAMPLES

### Example 1: Using the Update-MgExternalConnectionItem Cmdlet
```powershell
Import-Module Microsoft.Graph.Search
$params = @{
	Acl = @(
		@{
			Type = "everyone"
			Value = "67a141d8-cf4e-4528-ba07-bed21bfacd2d"
			AccessType = "grant"
		}
	)
}
Update-MgExternalConnectionItem -ExternalConnectionId $externalConnectionId -ExternalItemId $externalItemId -BodyParameter $params
```

This example shows how to use the Update-MgExternalConnectionItem Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -Acl
An array of access control entries.
Each entry specifies the access granted to a user or group.
Required.
To construct, please use Get-Help -Online and see NOTES section for ACL properties and create a hash table.

```yaml
Type: IMicrosoftGraphExternalConnectorsAcl1[]
Parameter Sets: UpdateExpanded1, UpdateViaIdentityExpanded1
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
Parameter Sets: UpdateExpanded1, UpdateViaIdentityExpanded1
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
Type: IMicrosoftGraphExternalConnectorsExternalItem1
Parameter Sets: Update1, UpdateViaIdentity1
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
Parameter Sets: UpdateExpanded1, UpdateViaIdentityExpanded1
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
Parameter Sets: UpdateExpanded1, Update1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExternalItemId
key: id of externalItem

```yaml
Type: String
Parameter Sets: UpdateExpanded1, Update1
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
Parameter Sets: UpdateExpanded1, UpdateViaIdentityExpanded1
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
Parameter Sets: UpdateViaIdentityExpanded1, UpdateViaIdentity1
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

### -Properties
properties

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded1, UpdateViaIdentityExpanded1
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphExternalConnectorsExternalItem1
### Microsoft.Graph.PowerShell.Models.ISearchIdentity
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


ACL <IMicrosoftGraphExternalConnectorsAcl1\[]>: An array of access control entries. Each entry specifies the access granted to a user or group. Required.
  - `[AccessType <String>]`: accessType
  - `[Type <String>]`: aclType
  - `[Value <String>]`: The unique identifer of the identity. In case of Azure Active Directory identities, value is set to the object identifier of the user, group or tenant for types user, group and everyone (and everyoneExceptGuests) respectively. In case of external groups value is set to the ID of the externalGroup

BODYPARAMETER `<IMicrosoftGraphExternalConnectorsExternalItem1>`: externalItem
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[Acl <IMicrosoftGraphExternalConnectorsAcl1[]>]`: An array of access control entries. Each entry specifies the access granted to a user or group. Required.
    - `[AccessType <String>]`: accessType
    - `[Type <String>]`: aclType
    - `[Value <String>]`: The unique identifer of the identity. In case of Azure Active Directory identities, value is set to the object identifier of the user, group or tenant for types user, group and everyone (and everyoneExceptGuests) respectively. In case of external groups value is set to the ID of the externalGroup
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
