---
external help file: Microsoft.Graph.Applications-help.xml
Module Name: Microsoft.Graph.Applications
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.applications/update-mgserviceprincipalpasswordsinglesignoncredentials
schema: 2.0.0
---

# Update-MgServicePrincipalPasswordSingleSignOnCredentials

## SYNOPSIS
Update single sign-on credentials using a password for a user or group.

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgServicePrincipalPasswordSingleSignOnCredentials -ServicePrincipalId <String>
 [-AdditionalProperties <Hashtable>] [-Credentials <IMicrosoftGraphCredential[]>] [-Id <String>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgServicePrincipalPasswordSingleSignOnCredentials -ServicePrincipalId <String>
 -BodyParameter <IPaths1R4QqcnServiceprincipalsServiceprincipalIdMicrosoftGraphUpdatepasswordsinglesignoncredentialsPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgServicePrincipalPasswordSingleSignOnCredentials -InputObject <IApplicationsIdentity>
 [-AdditionalProperties <Hashtable>] [-Credentials <IMicrosoftGraphCredential[]>] [-Id <String>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgServicePrincipalPasswordSingleSignOnCredentials -InputObject <IApplicationsIdentity>
 -BodyParameter <IPaths1R4QqcnServiceprincipalsServiceprincipalIdMicrosoftGraphUpdatepasswordsinglesignoncredentialsPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update single sign-on credentials using a password for a user or group.

## EXAMPLES

### Example 1: Using the Update-MgServicePrincipalPasswordSingleSignOnCredentials Cmdlet
```powershell
Import-Module Microsoft.Graph.Applications
$params = @{
	Id = "5793aa3b-cca9-4794-679a240f8b58"
	Credentials = @(
		@{
			FieldId = "param_username"
			Value = "myusername"
			Type = "username"
		}
		@{
			FieldId = "param_password"
			Value = "pa$$w0rd"
			Type = "password"
		}
	)
}
Update-MgServicePrincipalPasswordSingleSignOnCredentials -ServicePrincipalId $servicePrincipalId -BodyParameter $params
```

This example shows how to use the Update-MgServicePrincipalPasswordSingleSignOnCredentials Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Type: IPaths1R4QqcnServiceprincipalsServiceprincipalIdMicrosoftGraphUpdatepasswordsinglesignoncredentialsPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Credentials
.
To construct, please use Get-Help -Online and see NOTES section for CREDENTIALS properties and create a hash table.

```yaml
Type: IMicrosoftGraphCredential[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
.

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Type: IApplicationsIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
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

### -ServicePrincipalId
key: id of servicePrincipal

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

### Microsoft.Graph.PowerShell.Models.IApplicationsIdentity
### Microsoft.Graph.PowerShell.Models.IPaths1R4QqcnServiceprincipalsServiceprincipalIdMicrosoftGraphUpdatepasswordsinglesignoncredentialsPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IPaths1R4QqcnServiceprincipalsServiceprincipalIdMicrosoftGraphUpdatepasswordsinglesignoncredentialsPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Credentials <IMicrosoftGraphCredential[]>]`: 
    - `[FieldId <String>]`: The name of the field for this credential. e.g, username or password or phoneNumber. This is defined by the application. Must match what is in the html field on singleSignOnSettings/password object.
    - `[Type <String>]`: The type for this credential. Valid values: username, password, or other.
    - `[Value <String>]`: The value for this credential. e.g, mysuperhiddenpassword. Note the value for passwords is write-only, the value can never be read back.
  - `[Id <String>]`: 

CREDENTIALS <IMicrosoftGraphCredential\[]>: .
  - `[FieldId <String>]`: The name of the field for this credential. e.g, username or password or phoneNumber. This is defined by the application. Must match what is in the html field on singleSignOnSettings/password object.
  - `[Type <String>]`: The type for this credential. Valid values: username, password, or other.
  - `[Value <String>]`: The value for this credential. e.g, mysuperhiddenpassword. Note the value for passwords is write-only, the value can never be read back.

INPUTOBJECT `<IApplicationsIdentity>`: Identity Parameter
  - `[AppManagementPolicyId <String>]`: key: id of appManagementPolicy
  - `[AppRoleAssignmentId <String>]`: key: id of appRoleAssignment
  - `[ApplicationId <String>]`: key: id of application
  - `[ApplicationTemplateId <String>]`: key: id of applicationTemplate
  - `[ClaimsMappingPolicyId <String>]`: key: id of claimsMappingPolicy
  - `[ConnectorGroupId <String>]`: key: id of connectorGroup
  - `[ConnectorId <String>]`: key: id of connector
  - `[DelegatedPermissionClassificationId <String>]`: key: id of delegatedPermissionClassification
  - `[DirectoryDefinitionId <String>]`: key: id of directoryDefinition
  - `[DirectoryObjectId <String>]`: key: id of directoryObject
  - `[EndpointId <String>]`: key: id of endpoint
  - `[ExtensionPropertyId <String>]`: key: id of extensionProperty
  - `[FederatedIdentityCredentialId <String>]`: key: id of federatedIdentityCredential
  - `[GroupId <String>]`: key: id of group
  - `[HomeRealmDiscoveryPolicyId <String>]`: key: id of homeRealmDiscoveryPolicy
  - `[LicenseDetailsId <String>]`: key: id of licenseDetails
  - `[OAuth2PermissionGrantId <String>]`: key: id of oAuth2PermissionGrant
  - `[OnPremisesAgentGroupId <String>]`: key: id of onPremisesAgentGroup
  - `[OnPremisesAgentGroupId1 <String>]`: key: id of onPremisesAgentGroup
  - `[OnPremisesAgentId <String>]`: key: id of onPremisesAgent
  - `[OnPremisesPublishingProfileId <String>]`: key: id of onPremisesPublishingProfile
  - `[PublishedResourceId <String>]`: key: id of publishedResource
  - `[ServicePrincipalId <String>]`: key: id of servicePrincipal
  - `[SynchronizationJobId <String>]`: key: id of synchronizationJob
  - `[SynchronizationTemplateId <String>]`: key: id of synchronizationTemplate
  - `[TokenIssuancePolicyId <String>]`: key: id of tokenIssuancePolicy
  - `[TokenLifetimePolicyId <String>]`: key: id of tokenLifetimePolicy
  - `[UserId <String>]`: key: id of user

## RELATED LINKS
