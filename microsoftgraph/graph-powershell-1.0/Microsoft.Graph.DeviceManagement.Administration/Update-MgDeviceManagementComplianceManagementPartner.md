---
external help file: Microsoft.Graph.DeviceManagement.Administration-help.xml
Module Name: Microsoft.Graph.DeviceManagement.Administration
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.devicemanagement.administration/update-mgdevicemanagementcompliancemanagementpartner
schema: 2.0.0
---

# Update-MgDeviceManagementComplianceManagementPartner

## SYNOPSIS
Update the navigation property complianceManagementPartners in deviceManagement

## SYNTAX

### UpdateExpanded1 (Default)
```
Update-MgDeviceManagementComplianceManagementPartner -ComplianceManagementPartnerId <String>
 [-AdditionalProperties <Hashtable>]
 [-AndroidEnrollmentAssignments <IMicrosoftGraphComplianceManagementPartnerAssignment[]>] [-AndroidOnboarded]
 [-DisplayName <String>] [-Id <String>]
 [-IosEnrollmentAssignments <IMicrosoftGraphComplianceManagementPartnerAssignment[]>] [-IosOnboarded]
 [-LastHeartbeatDateTime <DateTime>]
 [-MacOSEnrollmentAssignments <IMicrosoftGraphComplianceManagementPartnerAssignment[]>] [-MacOSOnboarded]
 [-PartnerState <DeviceManagementPartnerTenantState>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update1
```
Update-MgDeviceManagementComplianceManagementPartner -ComplianceManagementPartnerId <String>
 -BodyParameter <IMicrosoftGraphComplianceManagementPartner1> [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### UpdateViaIdentityExpanded1
```
Update-MgDeviceManagementComplianceManagementPartner -InputObject <IDeviceManagementAdministrationIdentity>
 [-AdditionalProperties <Hashtable>]
 [-AndroidEnrollmentAssignments <IMicrosoftGraphComplianceManagementPartnerAssignment[]>] [-AndroidOnboarded]
 [-DisplayName <String>] [-Id <String>]
 [-IosEnrollmentAssignments <IMicrosoftGraphComplianceManagementPartnerAssignment[]>] [-IosOnboarded]
 [-LastHeartbeatDateTime <DateTime>]
 [-MacOSEnrollmentAssignments <IMicrosoftGraphComplianceManagementPartnerAssignment[]>] [-MacOSOnboarded]
 [-PartnerState <DeviceManagementPartnerTenantState>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity1
```
Update-MgDeviceManagementComplianceManagementPartner -InputObject <IDeviceManagementAdministrationIdentity>
 -BodyParameter <IMicrosoftGraphComplianceManagementPartner1> [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property complianceManagementPartners in deviceManagement

## EXAMPLES

## PARAMETERS

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

### -AndroidEnrollmentAssignments
User groups which enroll Android devices through partner.
To construct, please use Get-Help -Online and see NOTES section for ANDROIDENROLLMENTASSIGNMENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphComplianceManagementPartnerAssignment[]
Parameter Sets: UpdateExpanded1, UpdateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AndroidOnboarded
Partner onboarded for Android devices.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded1, UpdateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
Compliance management partner for all platforms
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphComplianceManagementPartner1
Parameter Sets: Update1, UpdateViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ComplianceManagementPartnerId
key: id of complianceManagementPartner

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

### -DisplayName
Partner display name

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
Type: IDeviceManagementAdministrationIdentity
Parameter Sets: UpdateViaIdentityExpanded1, UpdateViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IosEnrollmentAssignments
User groups which enroll ios devices through partner.
To construct, please use Get-Help -Online and see NOTES section for IOSENROLLMENTASSIGNMENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphComplianceManagementPartnerAssignment[]
Parameter Sets: UpdateExpanded1, UpdateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IosOnboarded
Partner onboarded for ios devices.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded1, UpdateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastHeartbeatDateTime
Timestamp of last heartbeat after admin onboarded to the compliance management partner

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded1, UpdateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MacOSEnrollmentAssignments
User groups which enroll Mac devices through partner.
To construct, please use Get-Help -Online and see NOTES section for MACOSENROLLMENTASSIGNMENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphComplianceManagementPartnerAssignment[]
Parameter Sets: UpdateExpanded1, UpdateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MacOSOnboarded
Partner onboarded for Mac devices.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded1, UpdateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PartnerState
Partner state of this tenant.

```yaml
Type: DeviceManagementPartnerTenantState
Parameter Sets: UpdateExpanded1, UpdateViaIdentityExpanded1
Aliases:

Required: False
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

### Microsoft.Graph.PowerShell.Models.IDeviceManagementAdministrationIdentity
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphComplianceManagementPartner1
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


ANDROIDENROLLMENTASSIGNMENTS <IMicrosoftGraphComplianceManagementPartnerAssignment\[]>: User groups which enroll Android devices through partner.
  - `[Target <IMicrosoftGraphDeviceAndAppManagementAssignmentTarget>]`: Base type for assignment targets.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.

BODYPARAMETER `<IMicrosoftGraphComplianceManagementPartner1>`: Compliance management partner for all platforms
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[AndroidEnrollmentAssignments <IMicrosoftGraphComplianceManagementPartnerAssignment[]>]`: User groups which enroll Android devices through partner.
    - `[Target <IMicrosoftGraphDeviceAndAppManagementAssignmentTarget>]`: Base type for assignment targets.
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AndroidOnboarded <Boolean?>]`: Partner onboarded for Android devices.
  - `[DisplayName <String>]`: Partner display name
  - `[IosEnrollmentAssignments <IMicrosoftGraphComplianceManagementPartnerAssignment[]>]`: User groups which enroll ios devices through partner.
  - `[IosOnboarded <Boolean?>]`: Partner onboarded for ios devices.
  - `[LastHeartbeatDateTime <DateTime?>]`: Timestamp of last heartbeat after admin onboarded to the compliance management partner
  - `[MacOSEnrollmentAssignments <IMicrosoftGraphComplianceManagementPartnerAssignment[]>]`: User groups which enroll Mac devices through partner.
  - `[MacOSOnboarded <Boolean?>]`: Partner onboarded for Mac devices.
  - `[PartnerState <DeviceManagementPartnerTenantState?>]`: Partner state of this tenant.

INPUTOBJECT `<IDeviceManagementAdministrationIdentity>`: Identity Parameter
  - `[AuditEventId <String>]`: key: id of auditEvent
  - `[CartToClassAssociationId <String>]`: key: id of cartToClassAssociation
  - `[CloudPcAuditEventId <String>]`: key: id of cloudPcAuditEvent
  - `[CloudPcDeviceImageId <String>]`: key: id of cloudPcDeviceImage
  - `[CloudPcExportJobId <String>]`: key: id of cloudPcExportJob
  - `[CloudPcExternalPartnerSettingId <String>]`: key: id of cloudPcExternalPartnerSetting
  - `[CloudPcGalleryImageId <String>]`: key: id of cloudPcGalleryImage
  - `[CloudPcId <String>]`: key: id of cloudPC
  - `[CloudPcOnPremisesConnectionId <String>]`: key: id of cloudPcOnPremisesConnection
  - `[CloudPcProvisioningPolicyAssignmentId <String>]`: key: id of cloudPcProvisioningPolicyAssignment
  - `[CloudPcProvisioningPolicyId <String>]`: key: id of cloudPcProvisioningPolicy
  - `[CloudPcServicePlanId <String>]`: key: id of cloudPcServicePlan
  - `[CloudPcSharedUseServicePlanId <String>]`: key: id of cloudPcSharedUseServicePlan
  - `[CloudPcSnapshotId <String>]`: key: id of cloudPcSnapshot
  - `[CloudPcSupportedRegionId <String>]`: key: id of cloudPcSupportedRegion
  - `[CloudPcUserSettingAssignmentId <String>]`: key: id of cloudPcUserSettingAssignment
  - `[CloudPcUserSettingId <String>]`: key: id of cloudPcUserSetting
  - `[ComanagementEligibleDeviceId <String>]`: key: id of comanagementEligibleDevice
  - `[ComplianceManagementPartnerId <String>]`: key: id of complianceManagementPartner
  - `[DeviceAndAppManagementRoleAssignmentId <String>]`: key: id of deviceAndAppManagementRoleAssignment
  - `[DeviceManagementDomainJoinConnectorId <String>]`: key: id of deviceManagementDomainJoinConnector
  - `[DeviceManagementExchangeConnectorId <String>]`: key: id of deviceManagementExchangeConnector
  - `[DeviceManagementExchangeOnPremisesPolicyId <String>]`: key: id of deviceManagementExchangeOnPremisesPolicy
  - `[DeviceManagementPartnerId <String>]`: key: id of deviceManagementPartner
  - `[GroupPolicyCategoryId <String>]`: key: id of groupPolicyCategory
  - `[GroupPolicyCategoryId1 <String>]`: key: id of groupPolicyCategory
  - `[GroupPolicyDefinitionFileId <String>]`: key: id of groupPolicyDefinitionFile
  - `[GroupPolicyDefinitionId <String>]`: key: id of groupPolicyDefinition
  - `[GroupPolicyMigrationReportId <String>]`: key: id of groupPolicyMigrationReport
  - `[GroupPolicyObjectFileId <String>]`: key: id of groupPolicyObjectFile
  - `[GroupPolicyOperationId <String>]`: key: id of groupPolicyOperation
  - `[GroupPolicyPresentationId <String>]`: key: id of groupPolicyPresentation
  - `[GroupPolicySettingMappingId <String>]`: key: id of groupPolicySettingMapping
  - `[GroupPolicyUploadedDefinitionFileId <String>]`: key: id of groupPolicyUploadedDefinitionFile
  - `[IntuneBrandingProfileAssignmentId <String>]`: key: id of intuneBrandingProfileAssignment
  - `[IntuneBrandingProfileId <String>]`: key: id of intuneBrandingProfile
  - `[IosUpdateDeviceStatusId <String>]`: key: id of iosUpdateDeviceStatus
  - `[ManagedAllDeviceCertificateStateId <String>]`: key: id of managedAllDeviceCertificateState
  - `[MobileThreatDefenseConnectorId <String>]`: key: id of mobileThreatDefenseConnector
  - `[NdesConnectorId <String>]`: key: id of ndesConnector
  - `[RemoteAssistancePartnerId <String>]`: key: id of remoteAssistancePartner
  - `[ResourceOperationId <String>]`: key: id of resourceOperation
  - `[RestrictedAppsViolationId <String>]`: key: id of restrictedAppsViolation
  - `[RoleAssignmentId <String>]`: key: id of roleAssignment
  - `[RoleDefinitionId <String>]`: key: id of roleDefinition
  - `[RoleScopeTagAutoAssignmentId <String>]`: key: id of roleScopeTagAutoAssignment
  - `[RoleScopeTagId <String>]`: key: id of roleScopeTag
  - `[TelecomExpenseManagementPartnerId <String>]`: key: id of telecomExpenseManagementPartner
  - `[TermsAndConditionsAcceptanceStatusId <String>]`: key: id of termsAndConditionsAcceptanceStatus
  - `[TermsAndConditionsAssignmentId <String>]`: key: id of termsAndConditionsAssignment
  - `[TermsAndConditionsGroupAssignmentId <String>]`: key: id of termsAndConditionsGroupAssignment
  - `[TermsAndConditionsId <String>]`: key: id of termsAndConditions
  - `[UnsupportedGroupPolicyExtensionId <String>]`: key: id of unsupportedGroupPolicyExtension
  - `[UserPfxCertificateId <String>]`: key: id of userPFXCertificate

IOSENROLLMENTASSIGNMENTS <IMicrosoftGraphComplianceManagementPartnerAssignment\[]>: User groups which enroll ios devices through partner.
  - `[Target <IMicrosoftGraphDeviceAndAppManagementAssignmentTarget>]`: Base type for assignment targets.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.

MACOSENROLLMENTASSIGNMENTS <IMicrosoftGraphComplianceManagementPartnerAssignment\[]>: User groups which enroll Mac devices through partner.
  - `[Target <IMicrosoftGraphDeviceAndAppManagementAssignmentTarget>]`: Base type for assignment targets.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.

## RELATED LINKS
