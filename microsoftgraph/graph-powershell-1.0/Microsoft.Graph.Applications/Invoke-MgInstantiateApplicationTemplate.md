---
external help file: Microsoft.Graph.Applications-help.xml
Module Name: Microsoft.Graph.Applications
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.applications/invoke-mginstantiateapplicationtemplate
schema: 2.0.0
---

# Invoke-MgInstantiateApplicationTemplate

## SYNOPSIS
Add an instance of an application from the Azure AD application gallery into your directory.
You can also use this API to instantiate non-gallery apps.
Use the following ID for the **applicationTemplate** object: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.

## SYNTAX

### InstantiateExpanded1 (Default)
```
Invoke-MgInstantiateApplicationTemplate -ApplicationTemplateId <String> [-AdditionalProperties <Hashtable>]
 [-DisplayName <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Instantiate1
```
Invoke-MgInstantiateApplicationTemplate -ApplicationTemplateId <String>
 -BodyParameter <IPathsCuokzfApplicationtemplatesApplicationtemplateIdMicrosoftGraphInstantiatePostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### InstantiateViaIdentityExpanded1
```
Invoke-MgInstantiateApplicationTemplate -InputObject <IApplicationsIdentity>
 [-AdditionalProperties <Hashtable>] [-DisplayName <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### InstantiateViaIdentity1
```
Invoke-MgInstantiateApplicationTemplate -InputObject <IApplicationsIdentity>
 -BodyParameter <IPathsCuokzfApplicationtemplatesApplicationtemplateIdMicrosoftGraphInstantiatePostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Add an instance of an application from the Azure AD application gallery into your directory.
You can also use this API to instantiate non-gallery apps.
Use the following ID for the **applicationTemplate** object: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.

## EXAMPLES

### Example 1: Using the Invoke-MgInstantiateApplicationTemplate Cmdlet
```powershell
Import-Module Microsoft.Graph.Applications
$params = @{
	DisplayName = "Azure AD SAML Toolkit"
}
Invoke-MgInstantiateApplicationTemplate -ApplicationTemplateId $applicationTemplateId -BodyParameter $params
```

This example shows how to use the Invoke-MgInstantiateApplicationTemplate Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: InstantiateExpanded1, InstantiateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApplicationTemplateId
key: id of applicationTemplate

```yaml
Type: String
Parameter Sets: InstantiateExpanded1, Instantiate1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
.
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPathsCuokzfApplicationtemplatesApplicationtemplateIdMicrosoftGraphInstantiatePostRequestbodyContentApplicationJsonSchema
Parameter Sets: Instantiate1, InstantiateViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DisplayName
.

```yaml
Type: String
Parameter Sets: InstantiateExpanded1, InstantiateViaIdentityExpanded1
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
Parameter Sets: InstantiateViaIdentityExpanded1, InstantiateViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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
### Microsoft.Graph.PowerShell.Models.IPathsCuokzfApplicationtemplatesApplicationtemplateIdMicrosoftGraphInstantiatePostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphApplicationServicePrincipal
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IPathsCuokzfApplicationtemplatesApplicationtemplateIdMicrosoftGraphInstantiatePostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DisplayName <String>]`: 

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
