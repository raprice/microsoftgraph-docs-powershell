---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.identity.signins/new-mgidentityconditionalaccesspolicy
schema: 2.0.0
ms.prod: "identity-and-sign-in"
---

# New-MgIdentityConditionalAccessPolicy

## SYNOPSIS
Create a new conditionalAccessPolicy.

## SYNTAX

### CreateExpanded (Default)
```
New-MgIdentityConditionalAccessPolicy [-AdditionalProperties <Hashtable>]
 [-Conditions <IMicrosoftGraphConditionalAccessConditionSet1>] [-CreatedDateTime <DateTime>]
 [-Description <String>] [-DisplayName <String>]
 [-GrantControls <IMicrosoftGraphConditionalAccessGrantControls1>] [-Id <String>]
 [-ModifiedDateTime <DateTime>] [-SessionControls <IMicrosoftGraphConditionalAccessSessionControls1>]
 [-State <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgIdentityConditionalAccessPolicy -BodyParameter <IMicrosoftGraphConditionalAccessPolicy1> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new conditionalAccessPolicy.

## EXAMPLES

### Example 1: Require MFA to access Exchange Online outside of trusted locations
```powershell
Connect-MgGraph -Scopes 'Policy.ReadWrite.ConditionalAccess'


$params = @{
  DisplayName = "Access to EXO requires MFA"
  State = "enabled"
  Conditions = @{
    ClientAppTypes = @(
      "mobileAppsAndDesktopClients"
      "browser"
    )
    Applications = @{
      IncludeApplications = @(
        "b457cbac-03cb-4b15-9eef-79f24f8d3247"
      )
    }
    Users = @{
      IncludeGroups = @(
        "f39e2655-3fae-43ad-94e2-c2b593cfc473"
       )
    }
    Locations = @{
      IncludeLocations = @(
        "All"
      )
      ExcludeLocations = @(
        "AllTrusted"
      )
    }
   }
   GrantControls = @{
     Operator = "OR"
     BuiltInControls = @(
       "mfa"
     )
   }
}

New-MgIdentityConditionalAccessPolicy -BodyParameter $params

Id                                   CreatedDateTime      Description DisplayName                ModifiedDateTime State
--                                   ---------------      ----------- -----------                ---------------- -----
1c9afd06-3f59-464e-a6d9-193d99764a01 7/29/2022 9:46:18 AM             Access to EXO requires MFA                  enabled
```

This example shows a request to require multi-factor authentication for access to Exchange Online from modern authentication clients outside of trusted locations for a particular group.

### Example 2: Block access to Exchange Online from non-trusted regions
```powershell
Connect-MgGraph -Scopes 'Policy.ReadWrite.ConditionalAccess'

$params = @{
  DisplayName = "Block access to EXO non-trusted regions."
  State = "enabled"
  Conditions = @{
    ClientAppTypes = @(
      "all"
    )
    Applications = @{
      IncludeApplications = @(
        "b457cbac-03cb-4b15-9eef-79f24f8d3247"
      )
    }
    Users = @{
      IncludeGroups = @(
        "f39e2655-3fae-43ad-94e2-c2b593cfc473"
      )
    }
    Locations = @{
      IncludeLocations = @(
        "0824dbaf-6277-4db0-8112-b29fd356f2c4"
      )
    }
  }
  GrantControls = @{
    Operator = "OR"
    BuiltInControls = @(
      "block"
    )
    }
  }

New-MgIdentityConditionalAccessPolicy -BodyParameter $params

Id                                   CreatedDateTime       Description DisplayName                              ModifiedDateTime State
--                                   ---------------       ----------- -----------                              ---------------- -----
61c7530f-5c1d-44b2-a972-4ae658b7a9ac 7/29/2022 10:03:30 AM             Block access to EXO non-trusted regions.                  enabled
```

This example shows a request to block access to Exchange Online from non-trusted/unknown regions.
This example assumes that the named location `0824dbaf-6277-4db0-8112-b29fd356f2c4` corresponds to a list of non-trusted/unknown regions.

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

### -BodyParameter
conditionalAccessPolicy
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphConditionalAccessPolicy1
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Conditions
conditionalAccessConditionSet
To construct, please use Get-Help -Online and see NOTES section for CONDITIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphConditionalAccessConditionSet1
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreatedDateTime
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Readonly.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
Not used.

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

### -DisplayName
Specifies a display name for the conditionalAccessPolicy object.

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

### -GrantControls
conditionalAccessGrantControls
To construct, please use Get-Help -Online and see NOTES section for GRANTCONTROLS properties and create a hash table.

```yaml
Type: IMicrosoftGraphConditionalAccessGrantControls1
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

### -ModifiedDateTime
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Readonly.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SessionControls
conditionalAccessSessionControls
To construct, please use Get-Help -Online and see NOTES section for SESSIONCONTROLS properties and create a hash table.

```yaml
Type: IMicrosoftGraphConditionalAccessSessionControls1
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -State
conditionalAccessPolicyState

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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphConditionalAccessPolicy1
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphConditionalAccessPolicy1
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IMicrosoftGraphConditionalAccessPolicy1>`: conditionalAccessPolicy
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[Conditions <IMicrosoftGraphConditionalAccessConditionSet1>]`: conditionalAccessConditionSet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Applications <IMicrosoftGraphConditionalAccessApplications1>]`: conditionalAccessApplications
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ApplicationFilter <IMicrosoftGraphConditionalAccessFilter>]`: conditionalAccessFilter
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Mode <String>]`: filterMode
        - `[Rule <String>]`: Rule syntax is similar to that used for membership rules for groups in Azure Active Directory (Azure AD). For details, see rules with multiple expressions
      - `[ExcludeApplications <String[]>]`: Can be one of the following:  The list of client IDs (appId) explicitly excluded from the policy. Office365 - For the list of apps included in Office365, see Conditional Access target apps: Office 365
      - `[IncludeApplications <String[]>]`: Can be one of the following:  The list of client IDs (appId) the policy applies to, unless explicitly excluded (in excludeApplications)  All  Office365 - For the list of apps included in Office365, see Conditional Access target apps: Office 365
      - `[IncludeAuthenticationContextClassReferences <String[]>]`: Authentication context class references include. Supported values are c1 through c25.
      - `[IncludeUserActions <String[]>]`: User actions to include. Supported values are urn:user:registersecurityinfo and urn:user:registerdevice
    - `[ClientAppTypes <String[]>]`: Client application types included in the policy. Possible values are: all, browser, mobileAppsAndDesktopClients, exchangeActiveSync, easSupported, other. Required.
    - `[ClientApplications <IMicrosoftGraphConditionalAccessClientApplications1>]`: conditionalAccessClientApplications
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ExcludeServicePrincipals <String[]>]`: Service principal IDs excluded from the policy scope.
      - `[IncludeServicePrincipals <String[]>]`: Service principal IDs included in the policy scope, or ServicePrincipalsInMyTenant.
      - `[ServicePrincipalFilter <IMicrosoftGraphConditionalAccessFilter>]`: conditionalAccessFilter
    - `[DeviceStates <IMicrosoftGraphConditionalAccessDeviceStates>]`: conditionalAccessDeviceStates
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ExcludeStates <String[]>]`: States excluded from the scope of the policy. Possible values: Compliant, DomainJoined.
      - `[IncludeStates <String[]>]`: States in the scope of the policy. All is the only allowed value.
    - `[Devices <IMicrosoftGraphConditionalAccessDevices1>]`: conditionalAccessDevices
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DeviceFilter <IMicrosoftGraphConditionalAccessFilter>]`: conditionalAccessFilter
      - `[ExcludeDeviceStates <String[]>]`: 
      - `[ExcludeDevices <String[]>]`: States excluded from the scope of the policy. Possible values: Compliant, DomainJoined. Cannot be set if deviceFIlter is set.
      - `[IncludeDeviceStates <String[]>]`: 
      - `[IncludeDevices <String[]>]`: States in the scope of the policy. All is the only allowed value. Cannot be set if deviceFIlter is set.
    - `[Locations <IMicrosoftGraphConditionalAccessLocations>]`: conditionalAccessLocations
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ExcludeLocations <String[]>]`: Location IDs excluded from scope of policy.
      - `[IncludeLocations <String[]>]`: Location IDs in scope of policy unless explicitly excluded, All, or AllTrusted.
    - `[Platforms <IMicrosoftGraphConditionalAccessPlatforms>]`: conditionalAccessPlatforms
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ExcludePlatforms <String[]>]`: Possible values are: android, iOS, windows, windowsPhone, macOS, linux, all, unknownFutureValue.
      - `[IncludePlatforms <String[]>]`: Possible values are: android, iOS, windows, windowsPhone, macOS, linux, all, unknownFutureValue.
    - `[ServicePrincipalRiskLevels <String[]>]`: Service principal risk levels included in the policy. Possible values are: low, medium, high, none, unknownFutureValue.
    - `[SignInRiskLevels <String[]>]`: Sign-in risk levels included in the policy. Possible values are: low, medium, high, hidden, none, unknownFutureValue. Required.
    - `[UserRiskLevels <String[]>]`: User risk levels included in the policy. Possible values are: low, medium, high, hidden, none, unknownFutureValue. Required.
    - `[Users <IMicrosoftGraphConditionalAccessUsers1>]`: conditionalAccessUsers
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ExcludeGroups <String[]>]`: Group IDs excluded from scope of policy.
      - `[ExcludeGuestsOrExternalUsers <IMicrosoftGraphConditionalAccessGuestsOrExternalUsers>]`: conditionalAccessGuestsOrExternalUsers
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[ExternalTenants <IMicrosoftGraphConditionalAccessExternalTenants>]`: conditionalAccessExternalTenants
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[MembershipKind <String>]`: conditionalAccessExternalTenantsMembershipKind
        - `[GuestOrExternalUserTypes <String>]`: conditionalAccessGuestOrExternalUserTypes
      - `[ExcludeRoles <String[]>]`: Role IDs excluded from scope of policy.
      - `[ExcludeUsers <String[]>]`: User IDs excluded from scope of policy and/or GuestsOrExternalUsers.
      - `[IncludeGroups <String[]>]`: Group IDs in scope of policy unless explicitly excluded, or All.
      - `[IncludeGuestsOrExternalUsers <IMicrosoftGraphConditionalAccessGuestsOrExternalUsers>]`: conditionalAccessGuestsOrExternalUsers
      - `[IncludeRoles <String[]>]`: Role IDs in scope of policy unless explicitly excluded, or All.
      - `[IncludeUsers <String[]>]`: User IDs in scope of policy unless explicitly excluded, or None or All or GuestsOrExternalUsers.
  - `[CreatedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z. Readonly.
  - `[Description <String>]`: Not used.
  - `[DisplayName <String>]`: Specifies a display name for the conditionalAccessPolicy object.
  - `[GrantControls <IMicrosoftGraphConditionalAccessGrantControls1>]`: conditionalAccessGrantControls
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AuthenticationStrength <IMicrosoftGraphAuthenticationStrengthPolicy>]`: authenticationStrengthPolicy
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique idenfier for an entity. Read-only.
      - `[AllowedCombinations <String[]>]`: A collection of authentication method modes that are required be used to satify this authentication strength.
      - `[CombinationConfigurations <IMicrosoftGraphAuthenticationCombinationConfiguration[]>]`: Settings that may be used to require specific types or instances of an authentication method to be used when authenticating with a specified combination of authentication methods.
        - `[Id <String>]`: The unique idenfier for an entity. Read-only.
        - `[AppliesToCombinations <String[]>]`: Which authentication method combinations this configuration applies to. Must be an allowedCombinations object that's defined for the authenticationStrengthPolicy. The only possible value for fido2combinationConfigurations is 'fido2'.
      - `[CreatedDateTime <DateTime?>]`: The datetime when this policy was created.
      - `[Description <String>]`: The human-readable description of this policy.
      - `[DisplayName <String>]`: The human-readable display name of this policy. Supports $filter (eq, ne, not , and in).
      - `[ModifiedDateTime <DateTime?>]`: The datetime when this policy was last modified.
      - `[PolicyType <String>]`: authenticationStrengthPolicyType
      - `[RequirementsSatisfied <String>]`: authenticationStrengthRequirements
    - `[BuiltInControls <String[]>]`: List of values of built-in controls required by the policy. Possible values: block, mfa, compliantDevice, domainJoinedDevice, approvedApplication, compliantApplication, passwordChange, unknownFutureValue.
    - `[CustomAuthenticationFactors <String[]>]`: List of custom controls IDs required by the policy. To learn more about custom control, see Custom controls (preview).
    - `[Operator <String>]`: Defines the relationship of the grant controls. Possible values: AND, OR.
    - `[TermsOfUse <String[]>]`: List of terms of use IDs required by the policy.
  - `[ModifiedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z. Readonly.
  - `[SessionControls <IMicrosoftGraphConditionalAccessSessionControls1>]`: conditionalAccessSessionControls
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ApplicationEnforcedRestrictions <IMicrosoftGraphApplicationEnforcedRestrictionsSessionControl>]`: applicationEnforcedRestrictionsSessionControl
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IsEnabled <Boolean?>]`: Specifies whether the session control is enabled.
    - `[CloudAppSecurity <IMicrosoftGraphCloudAppSecuritySessionControl>]`: cloudAppSecuritySessionControl
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IsEnabled <Boolean?>]`: Specifies whether the session control is enabled.
      - `[CloudAppSecurityType <String>]`: cloudAppSecuritySessionControlType
    - `[ContinuousAccessEvaluation <IMicrosoftGraphContinuousAccessEvaluationSessionControl>]`: continuousAccessEvaluationSessionControl
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Mode <String>]`: continuousAccessEvaluationMode
    - `[DisableResilienceDefaults <Boolean?>]`: Session control that determines whether it is acceptable for Azure AD to extend existing sessions based on information collected prior to an outage or not.
    - `[PersistentBrowser <IMicrosoftGraphPersistentBrowserSessionControl>]`: persistentBrowserSessionControl
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IsEnabled <Boolean?>]`: Specifies whether the session control is enabled.
      - `[Mode <String>]`: persistentBrowserSessionMode
    - `[SignInFrequency <IMicrosoftGraphSignInFrequencySessionControl>]`: signInFrequencySessionControl
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IsEnabled <Boolean?>]`: Specifies whether the session control is enabled.
      - `[AuthenticationType <String>]`: signInFrequencyAuthenticationType
      - `[FrequencyInterval <String>]`: signInFrequencyInterval
      - `[Type <String>]`: signinFrequencyType
      - `[Value <Int32?>]`: The number of days or hours.
  - `[State <String>]`: conditionalAccessPolicyState

CONDITIONS `<IMicrosoftGraphConditionalAccessConditionSet1>`: conditionalAccessConditionSet
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Applications <IMicrosoftGraphConditionalAccessApplications1>]`: conditionalAccessApplications
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ApplicationFilter <IMicrosoftGraphConditionalAccessFilter>]`: conditionalAccessFilter
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Mode <String>]`: filterMode
      - `[Rule <String>]`: Rule syntax is similar to that used for membership rules for groups in Azure Active Directory (Azure AD). For details, see rules with multiple expressions
    - `[ExcludeApplications <String[]>]`: Can be one of the following:  The list of client IDs (appId) explicitly excluded from the policy. Office365 - For the list of apps included in Office365, see Conditional Access target apps: Office 365
    - `[IncludeApplications <String[]>]`: Can be one of the following:  The list of client IDs (appId) the policy applies to, unless explicitly excluded (in excludeApplications)  All  Office365 - For the list of apps included in Office365, see Conditional Access target apps: Office 365
    - `[IncludeAuthenticationContextClassReferences <String[]>]`: Authentication context class references include. Supported values are c1 through c25.
    - `[IncludeUserActions <String[]>]`: User actions to include. Supported values are urn:user:registersecurityinfo and urn:user:registerdevice
  - `[ClientAppTypes <String[]>]`: Client application types included in the policy. Possible values are: all, browser, mobileAppsAndDesktopClients, exchangeActiveSync, easSupported, other. Required.
  - `[ClientApplications <IMicrosoftGraphConditionalAccessClientApplications1>]`: conditionalAccessClientApplications
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ExcludeServicePrincipals <String[]>]`: Service principal IDs excluded from the policy scope.
    - `[IncludeServicePrincipals <String[]>]`: Service principal IDs included in the policy scope, or ServicePrincipalsInMyTenant.
    - `[ServicePrincipalFilter <IMicrosoftGraphConditionalAccessFilter>]`: conditionalAccessFilter
  - `[DeviceStates <IMicrosoftGraphConditionalAccessDeviceStates>]`: conditionalAccessDeviceStates
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ExcludeStates <String[]>]`: States excluded from the scope of the policy. Possible values: Compliant, DomainJoined.
    - `[IncludeStates <String[]>]`: States in the scope of the policy. All is the only allowed value.
  - `[Devices <IMicrosoftGraphConditionalAccessDevices1>]`: conditionalAccessDevices
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DeviceFilter <IMicrosoftGraphConditionalAccessFilter>]`: conditionalAccessFilter
    - `[ExcludeDeviceStates <String[]>]`: 
    - `[ExcludeDevices <String[]>]`: States excluded from the scope of the policy. Possible values: Compliant, DomainJoined. Cannot be set if deviceFIlter is set.
    - `[IncludeDeviceStates <String[]>]`: 
    - `[IncludeDevices <String[]>]`: States in the scope of the policy. All is the only allowed value. Cannot be set if deviceFIlter is set.
  - `[Locations <IMicrosoftGraphConditionalAccessLocations>]`: conditionalAccessLocations
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ExcludeLocations <String[]>]`: Location IDs excluded from scope of policy.
    - `[IncludeLocations <String[]>]`: Location IDs in scope of policy unless explicitly excluded, All, or AllTrusted.
  - `[Platforms <IMicrosoftGraphConditionalAccessPlatforms>]`: conditionalAccessPlatforms
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ExcludePlatforms <String[]>]`: Possible values are: android, iOS, windows, windowsPhone, macOS, linux, all, unknownFutureValue.
    - `[IncludePlatforms <String[]>]`: Possible values are: android, iOS, windows, windowsPhone, macOS, linux, all, unknownFutureValue.
  - `[ServicePrincipalRiskLevels <String[]>]`: Service principal risk levels included in the policy. Possible values are: low, medium, high, none, unknownFutureValue.
  - `[SignInRiskLevels <String[]>]`: Sign-in risk levels included in the policy. Possible values are: low, medium, high, hidden, none, unknownFutureValue. Required.
  - `[UserRiskLevels <String[]>]`: User risk levels included in the policy. Possible values are: low, medium, high, hidden, none, unknownFutureValue. Required.
  - `[Users <IMicrosoftGraphConditionalAccessUsers1>]`: conditionalAccessUsers
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ExcludeGroups <String[]>]`: Group IDs excluded from scope of policy.
    - `[ExcludeGuestsOrExternalUsers <IMicrosoftGraphConditionalAccessGuestsOrExternalUsers>]`: conditionalAccessGuestsOrExternalUsers
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ExternalTenants <IMicrosoftGraphConditionalAccessExternalTenants>]`: conditionalAccessExternalTenants
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[MembershipKind <String>]`: conditionalAccessExternalTenantsMembershipKind
      - `[GuestOrExternalUserTypes <String>]`: conditionalAccessGuestOrExternalUserTypes
    - `[ExcludeRoles <String[]>]`: Role IDs excluded from scope of policy.
    - `[ExcludeUsers <String[]>]`: User IDs excluded from scope of policy and/or GuestsOrExternalUsers.
    - `[IncludeGroups <String[]>]`: Group IDs in scope of policy unless explicitly excluded, or All.
    - `[IncludeGuestsOrExternalUsers <IMicrosoftGraphConditionalAccessGuestsOrExternalUsers>]`: conditionalAccessGuestsOrExternalUsers
    - `[IncludeRoles <String[]>]`: Role IDs in scope of policy unless explicitly excluded, or All.
    - `[IncludeUsers <String[]>]`: User IDs in scope of policy unless explicitly excluded, or None or All or GuestsOrExternalUsers.

GRANTCONTROLS `<IMicrosoftGraphConditionalAccessGrantControls1>`: conditionalAccessGrantControls
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AuthenticationStrength <IMicrosoftGraphAuthenticationStrengthPolicy>]`: authenticationStrengthPolicy
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[AllowedCombinations <String[]>]`: A collection of authentication method modes that are required be used to satify this authentication strength.
    - `[CombinationConfigurations <IMicrosoftGraphAuthenticationCombinationConfiguration[]>]`: Settings that may be used to require specific types or instances of an authentication method to be used when authenticating with a specified combination of authentication methods.
      - `[Id <String>]`: The unique idenfier for an entity. Read-only.
      - `[AppliesToCombinations <String[]>]`: Which authentication method combinations this configuration applies to. Must be an allowedCombinations object that's defined for the authenticationStrengthPolicy. The only possible value for fido2combinationConfigurations is 'fido2'.
    - `[CreatedDateTime <DateTime?>]`: The datetime when this policy was created.
    - `[Description <String>]`: The human-readable description of this policy.
    - `[DisplayName <String>]`: The human-readable display name of this policy. Supports $filter (eq, ne, not , and in).
    - `[ModifiedDateTime <DateTime?>]`: The datetime when this policy was last modified.
    - `[PolicyType <String>]`: authenticationStrengthPolicyType
    - `[RequirementsSatisfied <String>]`: authenticationStrengthRequirements
  - `[BuiltInControls <String[]>]`: List of values of built-in controls required by the policy. Possible values: block, mfa, compliantDevice, domainJoinedDevice, approvedApplication, compliantApplication, passwordChange, unknownFutureValue.
  - `[CustomAuthenticationFactors <String[]>]`: List of custom controls IDs required by the policy. To learn more about custom control, see Custom controls (preview).
  - `[Operator <String>]`: Defines the relationship of the grant controls. Possible values: AND, OR.
  - `[TermsOfUse <String[]>]`: List of terms of use IDs required by the policy.

SESSIONCONTROLS `<IMicrosoftGraphConditionalAccessSessionControls1>`: conditionalAccessSessionControls
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ApplicationEnforcedRestrictions <IMicrosoftGraphApplicationEnforcedRestrictionsSessionControl>]`: applicationEnforcedRestrictionsSessionControl
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IsEnabled <Boolean?>]`: Specifies whether the session control is enabled.
  - `[CloudAppSecurity <IMicrosoftGraphCloudAppSecuritySessionControl>]`: cloudAppSecuritySessionControl
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IsEnabled <Boolean?>]`: Specifies whether the session control is enabled.
    - `[CloudAppSecurityType <String>]`: cloudAppSecuritySessionControlType
  - `[ContinuousAccessEvaluation <IMicrosoftGraphContinuousAccessEvaluationSessionControl>]`: continuousAccessEvaluationSessionControl
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Mode <String>]`: continuousAccessEvaluationMode
  - `[DisableResilienceDefaults <Boolean?>]`: Session control that determines whether it is acceptable for Azure AD to extend existing sessions based on information collected prior to an outage or not.
  - `[PersistentBrowser <IMicrosoftGraphPersistentBrowserSessionControl>]`: persistentBrowserSessionControl
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IsEnabled <Boolean?>]`: Specifies whether the session control is enabled.
    - `[Mode <String>]`: persistentBrowserSessionMode
  - `[SignInFrequency <IMicrosoftGraphSignInFrequencySessionControl>]`: signInFrequencySessionControl
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IsEnabled <Boolean?>]`: Specifies whether the session control is enabled.
    - `[AuthenticationType <String>]`: signInFrequencyAuthenticationType
    - `[FrequencyInterval <String>]`: signInFrequencyInterval
    - `[Type <String>]`: signinFrequencyType
    - `[Value <Int32?>]`: The number of days or hours.

## RELATED LINKS

## RELATED LINKS
