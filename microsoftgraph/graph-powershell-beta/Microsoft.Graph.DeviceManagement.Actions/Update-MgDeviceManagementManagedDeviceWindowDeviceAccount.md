---
external help file: Microsoft.Graph.DeviceManagement.Actions-help.xml
Module Name: Microsoft.Graph.DeviceManagement.Actions
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.devicemanagement.actions/update-mgdevicemanagementmanageddevicewindowdeviceaccount
schema: 2.0.0
---

# Update-MgDeviceManagementManagedDeviceWindowDeviceAccount

## SYNOPSIS
Invoke action updateWindowsDeviceAccount

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgDeviceManagementManagedDeviceWindowDeviceAccount -ManagedDeviceId <String>
 [-AdditionalProperties <Hashtable>]
 [-UpdateWindowsDeviceAccountActionParameter <IMicrosoftGraphUpdateWindowsDeviceAccountActionParameter>]
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgDeviceManagementManagedDeviceWindowDeviceAccount -ManagedDeviceId <String>
 -BodyParameter <IPaths1L95NseDevicemanagementManageddevicesManageddeviceIdMicrosoftGraphUpdatewindowsdeviceaccountPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgDeviceManagementManagedDeviceWindowDeviceAccount -InputObject <IDeviceManagementActionsIdentity>
 [-AdditionalProperties <Hashtable>]
 [-UpdateWindowsDeviceAccountActionParameter <IMicrosoftGraphUpdateWindowsDeviceAccountActionParameter>]
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgDeviceManagementManagedDeviceWindowDeviceAccount -InputObject <IDeviceManagementActionsIdentity>
 -BodyParameter <IPaths1L95NseDevicemanagementManageddevicesManageddeviceIdMicrosoftGraphUpdatewindowsdeviceaccountPostRequestbodyContentApplicationJsonSchema>
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Invoke action updateWindowsDeviceAccount

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
.
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPaths1L95NseDevicemanagementManageddevicesManageddeviceIdMicrosoftGraphUpdatewindowsdeviceaccountPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, please use Get-Help -Online and see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IDeviceManagementActionsIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ManagedDeviceId
key: id of managedDevice

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

### -UpdateWindowsDeviceAccountActionParameter
updateWindowsDeviceAccountActionParameter
To construct, please use Get-Help -Online and see NOTES section for UPDATEWINDOWSDEVICEACCOUNTACTIONPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphUpdateWindowsDeviceAccountActionParameter
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

### Microsoft.Graph.PowerShell.Models.IDeviceManagementActionsIdentity
### Microsoft.Graph.PowerShell.Models.IPaths1L95NseDevicemanagementManageddevicesManageddeviceIdMicrosoftGraphUpdatewindowsdeviceaccountPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IPaths1L95NseDevicemanagementManageddevicesManageddeviceIdMicrosoftGraphUpdatewindowsdeviceaccountPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[UpdateWindowsDeviceAccountActionParameter <IMicrosoftGraphUpdateWindowsDeviceAccountActionParameter>]`: updateWindowsDeviceAccountActionParameter
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[CalendarSyncEnabled <Boolean?>]`: Not yet documented
    - `[DeviceAccount <IMicrosoftGraphWindowsDeviceAccount>]`: windowsDeviceAccount
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Password <String>]`: Not yet documented
    - `[DeviceAccountEmail <String>]`: Not yet documented
    - `[ExchangeServer <String>]`: Not yet documented
    - `[PasswordRotationEnabled <Boolean?>]`: Not yet documented
    - `[SessionInitiationProtocalAddress <String>]`: Not yet documented

INPUTOBJECT `<IDeviceManagementActionsIdentity>`: Identity Parameter
  - `[AlertRecordId <String>]`: key: id of alertRecord
  - `[AndroidDeviceOwnerEnrollmentProfileId <String>]`: key: id of androidDeviceOwnerEnrollmentProfile
  - `[AndroidForWorkEnrollmentProfileId <String>]`: key: id of androidForWorkEnrollmentProfile
  - `[AppLogCollectionRequestId <String>]`: key: id of appLogCollectionRequest
  - `[AppleUserInitiatedEnrollmentProfileId <String>]`: key: id of appleUserInitiatedEnrollmentProfile
  - `[CertificateConnectorDetailsId <String>]`: key: id of certificateConnectorDetails
  - `[CloudPcDeviceImageId <String>]`: key: id of cloudPcDeviceImage
  - `[CloudPcId <String>]`: key: id of cloudPC
  - `[CloudPcOnPremisesConnectionId <String>]`: key: id of cloudPcOnPremisesConnection
  - `[CloudPcProvisioningPolicyId <String>]`: key: id of cloudPcProvisioningPolicy
  - `[CloudPcUserSettingId <String>]`: key: id of cloudPcUserSetting
  - `[DataSharingConsentId <String>]`: key: id of dataSharingConsent
  - `[DepOnboardingSettingId <String>]`: key: id of depOnboardingSetting
  - `[DeviceCompliancePolicyId <String>]`: key: id of deviceCompliancePolicy
  - `[DeviceComplianceScriptId <String>]`: key: id of deviceComplianceScript
  - `[DeviceConfigurationId <String>]`: key: id of deviceConfiguration
  - `[DeviceCustomAttributeShellScriptId <String>]`: key: id of deviceCustomAttributeShellScript
  - `[DeviceEnrollmentConfigurationId <String>]`: key: id of deviceEnrollmentConfiguration
  - `[DeviceHealthScriptId <String>]`: key: id of deviceHealthScript
  - `[DeviceLogCollectionResponseId <String>]`: key: id of deviceLogCollectionResponse
  - `[DeviceManagementCompliancePolicyId <String>]`: key: id of deviceManagementCompliancePolicy
  - `[DeviceManagementConfigurationPolicyId <String>]`: key: id of deviceManagementConfigurationPolicy
  - `[DeviceManagementExchangeConnectorId <String>]`: key: id of deviceManagementExchangeConnector
  - `[DeviceManagementIntentId <String>]`: key: id of deviceManagementIntent
  - `[DeviceManagementPartnerId <String>]`: key: id of deviceManagementPartner
  - `[DeviceManagementResourceAccessProfileBaseId <String>]`: key: id of deviceManagementResourceAccessProfileBase
  - `[DeviceManagementReusablePolicySettingId <String>]`: key: id of deviceManagementReusablePolicySetting
  - `[DeviceManagementScriptId <String>]`: key: id of deviceManagementScript
  - `[DeviceManagementTemplateId <String>]`: key: id of deviceManagementTemplate
  - `[DeviceManagementTemplateId1 <String>]`: key: id of deviceManagementTemplate
  - `[DeviceShellScriptId <String>]`: key: id of deviceShellScript
  - `[EmbeddedSimActivationCodePoolId <String>]`: key: id of embeddedSIMActivationCodePool
  - `[EnrollmentProfileId <String>]`: key: id of enrollmentProfile
  - `[GroupPolicyConfigurationId <String>]`: key: id of groupPolicyConfiguration
  - `[GroupPolicyUploadedDefinitionFileId <String>]`: key: id of groupPolicyUploadedDefinitionFile
  - `[IntuneBrandingProfileId <String>]`: key: id of intuneBrandingProfile
  - `[ManagedDeviceId <String>]`: key: id of managedDevice
  - `[MicrosoftTunnelServerId <String>]`: key: id of microsoftTunnelServer
  - `[MicrosoftTunnelServerLogCollectionResponseId <String>]`: key: id of microsoftTunnelServerLogCollectionResponse
  - `[MicrosoftTunnelSiteId <String>]`: key: id of microsoftTunnelSite
  - `[MobileAppTroubleshootingEventId <String>]`: key: id of mobileAppTroubleshootingEvent
  - `[NotificationMessageTemplateId <String>]`: key: id of notificationMessageTemplate
  - `[OemWarrantyInformationOnboardingId <String>]`: key: id of oemWarrantyInformationOnboarding
  - `[RemoteAssistancePartnerId <String>]`: key: id of remoteAssistancePartner
  - `[RoleScopeTagId <String>]`: key: id of roleScopeTag
  - `[WindowsAutopilotDeploymentProfileId <String>]`: key: id of windowsAutopilotDeploymentProfile
  - `[WindowsAutopilotDeviceIdentityId <String>]`: key: id of windowsAutopilotDeviceIdentity
  - `[WindowsDriverUpdateProfileId <String>]`: key: id of windowsDriverUpdateProfile
  - `[WindowsFeatureUpdateProfileId <String>]`: key: id of windowsFeatureUpdateProfile
  - `[WindowsQualityUpdateProfileId <String>]`: key: id of windowsQualityUpdateProfile
  - `[ZebraFotaDeploymentId <String>]`: key: id of zebraFotaDeployment

UPDATEWINDOWSDEVICEACCOUNTACTIONPARAMETER `<IMicrosoftGraphUpdateWindowsDeviceAccountActionParameter>`: updateWindowsDeviceAccountActionParameter
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[CalendarSyncEnabled <Boolean?>]`: Not yet documented
  - `[DeviceAccount <IMicrosoftGraphWindowsDeviceAccount>]`: windowsDeviceAccount
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Password <String>]`: Not yet documented
  - `[DeviceAccountEmail <String>]`: Not yet documented
  - `[ExchangeServer <String>]`: Not yet documented
  - `[PasswordRotationEnabled <Boolean?>]`: Not yet documented
  - `[SessionInitiationProtocalAddress <String>]`: Not yet documented

## RELATED LINKS
