---
external help file: Microsoft.Graph.DeviceManagement.Administration-help.xml
Module Name: Microsoft.Graph.DeviceManagement.Administration
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.devicemanagement.administration/update-mgdevicemanagementgrouppolicymigrationreport
schema: 2.0.0
---

# Update-MgDeviceManagementGroupPolicyMigrationReport

## SYNOPSIS
Update the navigation property groupPolicyMigrationReports in deviceManagement

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgDeviceManagementGroupPolicyMigrationReport -GroupPolicyMigrationReportId <String>
 [-AdditionalProperties <Hashtable>] [-CreatedDateTime <DateTime>] [-DisplayName <String>]
 [-GroupPolicyCreatedDateTime <DateTime>] [-GroupPolicyLastModifiedDateTime <DateTime>]
 [-GroupPolicyObjectId <String>] [-GroupPolicySettingMappings <IMicrosoftGraphGroupPolicySettingMapping[]>]
 [-Id <String>] [-LastModifiedDateTime <DateTime>] [-MigrationReadiness <GroupPolicyMigrationReadiness>]
 [-OuDistinguishedName <String>] [-RoleScopeTagIds <String[]>] [-SupportedSettingsCount <Int32>]
 [-SupportedSettingsPercent <Int32>] [-TargetedInActiveDirectory] [-TotalSettingsCount <Int32>]
 [-UnsupportedGroupPolicyExtensions <IMicrosoftGraphUnsupportedGroupPolicyExtension[]>] [-PassThru] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgDeviceManagementGroupPolicyMigrationReport -GroupPolicyMigrationReportId <String>
 -BodyParameter <IMicrosoftGraphGroupPolicyMigrationReport> [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgDeviceManagementGroupPolicyMigrationReport -InputObject <IDeviceManagementAdministrationIdentity>
 [-AdditionalProperties <Hashtable>] [-CreatedDateTime <DateTime>] [-DisplayName <String>]
 [-GroupPolicyCreatedDateTime <DateTime>] [-GroupPolicyLastModifiedDateTime <DateTime>]
 [-GroupPolicyObjectId <String>] [-GroupPolicySettingMappings <IMicrosoftGraphGroupPolicySettingMapping[]>]
 [-Id <String>] [-LastModifiedDateTime <DateTime>] [-MigrationReadiness <GroupPolicyMigrationReadiness>]
 [-OuDistinguishedName <String>] [-RoleScopeTagIds <String[]>] [-SupportedSettingsCount <Int32>]
 [-SupportedSettingsPercent <Int32>] [-TargetedInActiveDirectory] [-TotalSettingsCount <Int32>]
 [-UnsupportedGroupPolicyExtensions <IMicrosoftGraphUnsupportedGroupPolicyExtension[]>] [-PassThru] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgDeviceManagementGroupPolicyMigrationReport -InputObject <IDeviceManagementAdministrationIdentity>
 -BodyParameter <IMicrosoftGraphGroupPolicyMigrationReport> [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property groupPolicyMigrationReports in deviceManagement

## EXAMPLES

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
The Group Policy migration report.
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphGroupPolicyMigrationReport
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CreatedDateTime
The date and time at which the GroupPolicyMigrationReport was created.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
The name of Group Policy Object from the GPO Xml Content

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

### -GroupPolicyCreatedDateTime
The date and time at which the GroupPolicyMigrationReport was created.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GroupPolicyLastModifiedDateTime
The date and time at which the GroupPolicyMigrationReport was last modified.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GroupPolicyMigrationReportId
key: id of groupPolicyMigrationReport

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

### -GroupPolicyObjectId
The Group Policy Object GUID from GPO Xml content

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

### -GroupPolicySettingMappings
A list of group policy settings to MDM/Intune mappings.
To construct, please use Get-Help -Online and see NOTES section for GROUPPOLICYSETTINGMAPPINGS properties and create a hash table.

```yaml
Type: IMicrosoftGraphGroupPolicySettingMapping[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Type: IDeviceManagementAdministrationIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -LastModifiedDateTime
The date and time at which the GroupPolicyMigrationReport was last modified.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MigrationReadiness
Indicates if the Group Policy Object file is covered and ready for Intune migration.

```yaml
Type: GroupPolicyMigrationReadiness
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OuDistinguishedName
The distinguished name of the OU.

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

### -RoleScopeTagIds
The list of scope tags for the configuration.

```yaml
Type: String[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SupportedSettingsCount
The number of Group Policy Settings supported by Intune.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SupportedSettingsPercent
The Percentage of Group Policy Settings supported by Intune.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TargetedInActiveDirectory
The Targeted in AD property from GPO Xml Content

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TotalSettingsCount
The total number of Group Policy Settings from GPO file.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UnsupportedGroupPolicyExtensions
A list of unsupported group policy extensions inside the Group Policy Object.
To construct, please use Get-Help -Online and see NOTES section for UNSUPPORTEDGROUPPOLICYEXTENSIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnsupportedGroupPolicyExtension[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphGroupPolicyMigrationReport
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IMicrosoftGraphGroupPolicyMigrationReport>`: The Group Policy migration report.
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[CreatedDateTime <DateTime?>]`: The date and time at which the GroupPolicyMigrationReport was created.
  - `[DisplayName <String>]`: The name of Group Policy Object from the GPO Xml Content
  - `[GroupPolicyCreatedDateTime <DateTime?>]`: The date and time at which the GroupPolicyMigrationReport was created.
  - `[GroupPolicyLastModifiedDateTime <DateTime?>]`: The date and time at which the GroupPolicyMigrationReport was last modified.
  - `[GroupPolicyObjectId <String>]`: The Group Policy Object GUID from GPO Xml content
  - `[GroupPolicySettingMappings <IMicrosoftGraphGroupPolicySettingMapping[]>]`: A list of group policy settings to MDM/Intune mappings.
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[AdmxSettingDefinitionId <String>]`: Admx Group Policy Id
    - `[ChildIdList <String[]>]`: List of Child Ids of the group policy setting.
    - `[IntuneSettingDefinitionId <String>]`: The Intune Setting Definition Id
    - `[IntuneSettingUriList <String[]>]`: The list of Intune Setting URIs this group policy setting maps to
    - `[IsMdmSupported <Boolean?>]`: Indicates if the setting is supported by Intune or not
    - `[MdmCspName <String>]`: The CSP name this group policy setting maps to.
    - `[MdmMinimumOSVersion <Int32?>]`: The minimum OS version this mdm setting supports.
    - `[MdmSettingUri <String>]`: The MDM CSP URI this group policy setting maps to.
    - `[MdmSupportedState <MdmSupportedState?>]`: Mdm Support Status of the setting.
    - `[ParentId <String>]`: Parent Id of the group policy setting.
    - `[SettingCategory <String>]`: The category the group policy setting is in.
    - `[SettingDisplayName <String>]`: The display name of this group policy setting.
    - `[SettingDisplayValue <String>]`: The display value of this group policy setting.
    - `[SettingDisplayValueType <String>]`: The display value type of this group policy setting.
    - `[SettingName <String>]`: The name of this group policy setting.
    - `[SettingScope <GroupPolicySettingScope?>]`: Scope of the group policy setting.
    - `[SettingType <GroupPolicySettingType?>]`: Setting type of the group policy.
    - `[SettingValue <String>]`: The value of this group policy setting.
    - `[SettingValueDisplayUnits <String>]`: The display units of this group policy setting value
    - `[SettingValueType <String>]`: The value type of this group policy setting.
  - `[LastModifiedDateTime <DateTime?>]`: The date and time at which the GroupPolicyMigrationReport was last modified.
  - `[MigrationReadiness <GroupPolicyMigrationReadiness?>]`: Indicates if the Group Policy Object file is covered and ready for Intune migration.
  - `[OuDistinguishedName <String>]`: The distinguished name of the OU.
  - `[RoleScopeTagIds <String[]>]`: The list of scope tags for the configuration.
  - `[SupportedSettingsCount <Int32?>]`: The number of Group Policy Settings supported by Intune.
  - `[SupportedSettingsPercent <Int32?>]`: The Percentage of Group Policy Settings supported by Intune.
  - `[TargetedInActiveDirectory <Boolean?>]`: The Targeted in AD property from GPO Xml Content
  - `[TotalSettingsCount <Int32?>]`: The total number of Group Policy Settings from GPO file.
  - `[UnsupportedGroupPolicyExtensions <IMicrosoftGraphUnsupportedGroupPolicyExtension[]>]`: A list of unsupported group policy extensions inside the Group Policy Object.
    - `[Id <String>]`: The unique idenfier for an entity. Read-only.
    - `[ExtensionType <String>]`: ExtensionType of the unsupported extension.
    - `[NamespaceUrl <String>]`: Namespace Url of the unsupported extension.
    - `[NodeName <String>]`: Node name of the unsupported extension.
    - `[SettingScope <GroupPolicySettingScope?>]`: Scope of the group policy setting.

GROUPPOLICYSETTINGMAPPINGS <IMicrosoftGraphGroupPolicySettingMapping\[]>: A list of group policy settings to MDM/Intune mappings.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[AdmxSettingDefinitionId <String>]`: Admx Group Policy Id
  - `[ChildIdList <String[]>]`: List of Child Ids of the group policy setting.
  - `[IntuneSettingDefinitionId <String>]`: The Intune Setting Definition Id
  - `[IntuneSettingUriList <String[]>]`: The list of Intune Setting URIs this group policy setting maps to
  - `[IsMdmSupported <Boolean?>]`: Indicates if the setting is supported by Intune or not
  - `[MdmCspName <String>]`: The CSP name this group policy setting maps to.
  - `[MdmMinimumOSVersion <Int32?>]`: The minimum OS version this mdm setting supports.
  - `[MdmSettingUri <String>]`: The MDM CSP URI this group policy setting maps to.
  - `[MdmSupportedState <MdmSupportedState?>]`: Mdm Support Status of the setting.
  - `[ParentId <String>]`: Parent Id of the group policy setting.
  - `[SettingCategory <String>]`: The category the group policy setting is in.
  - `[SettingDisplayName <String>]`: The display name of this group policy setting.
  - `[SettingDisplayValue <String>]`: The display value of this group policy setting.
  - `[SettingDisplayValueType <String>]`: The display value type of this group policy setting.
  - `[SettingName <String>]`: The name of this group policy setting.
  - `[SettingScope <GroupPolicySettingScope?>]`: Scope of the group policy setting.
  - `[SettingType <GroupPolicySettingType?>]`: Setting type of the group policy.
  - `[SettingValue <String>]`: The value of this group policy setting.
  - `[SettingValueDisplayUnits <String>]`: The display units of this group policy setting value
  - `[SettingValueType <String>]`: The value type of this group policy setting.

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

UNSUPPORTEDGROUPPOLICYEXTENSIONS <IMicrosoftGraphUnsupportedGroupPolicyExtension\[]>: A list of unsupported group policy extensions inside the Group Policy Object.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[ExtensionType <String>]`: ExtensionType of the unsupported extension.
  - `[NamespaceUrl <String>]`: Namespace Url of the unsupported extension.
  - `[NodeName <String>]`: Node name of the unsupported extension.
  - `[SettingScope <GroupPolicySettingScope?>]`: Scope of the group policy setting.

## RELATED LINKS

## RELATED LINKS
