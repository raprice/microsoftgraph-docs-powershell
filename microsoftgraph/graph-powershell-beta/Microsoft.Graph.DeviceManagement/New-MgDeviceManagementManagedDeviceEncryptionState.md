---
external help file: Microsoft.Graph.DeviceManagement-help.xml
Module Name: Microsoft.Graph.DeviceManagement
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.devicemanagement/new-mgdevicemanagementmanageddeviceencryptionstate
schema: 2.0.0
---

# New-MgDeviceManagementManagedDeviceEncryptionState

## SYNOPSIS
Create new navigation property to managedDeviceEncryptionStates for deviceManagement

## SYNTAX

### CreateExpanded (Default)
```
New-MgDeviceManagementManagedDeviceEncryptionState [-AdditionalProperties <Hashtable>]
 [-AdvancedBitLockerStates <AdvancedBitLockerState>] [-DeviceName <String>] [-DeviceType <DeviceTypes>]
 [-EncryptionPolicySettingState <String>] [-EncryptionReadinessState <EncryptionReadinessState>]
 [-EncryptionState <EncryptionState>] [-FileVaultStates <FileVaultState>] [-Id <String>] [-OSVersion <String>]
 [-PolicyDetails <IMicrosoftGraphEncryptionReportPolicyDetails[]>] [-TpmSpecificationVersion <String>]
 [-UserPrincipalName <String>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgDeviceManagementManagedDeviceEncryptionState -BodyParameter <IMicrosoftGraphManagedDeviceEncryptionState>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to managedDeviceEncryptionStates for deviceManagement

## EXAMPLES

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

### -AdvancedBitLockerStates
Advanced BitLocker State

```yaml
Type: AdvancedBitLockerState
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
Encryption report per device
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphManagedDeviceEncryptionState
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DeviceName
Device name

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

### -DeviceType
Device type.

```yaml
Type: DeviceTypes
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EncryptionPolicySettingState
complianceStatus

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

### -EncryptionReadinessState
Encryption readiness state

```yaml
Type: EncryptionReadinessState
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EncryptionState
Encryption state

```yaml
Type: EncryptionState
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FileVaultStates
FileVault State

```yaml
Type: FileVaultState
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

### -OSVersion
Operating system version of the device

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

### -PolicyDetails
Policy Details
To construct, please use Get-Help -Online and see NOTES section for POLICYDETAILS properties and create a hash table.

```yaml
Type: IMicrosoftGraphEncryptionReportPolicyDetails[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TpmSpecificationVersion
Device TPM Version

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

### -UserPrincipalName
User name

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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphManagedDeviceEncryptionState
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphManagedDeviceEncryptionState
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IMicrosoftGraphManagedDeviceEncryptionState>`: Encryption report per device
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[AdvancedBitLockerStates <AdvancedBitLockerState?>]`: Advanced BitLocker State
  - `[DeviceName <String>]`: Device name
  - `[DeviceType <DeviceTypes?>]`: Device type.
  - `[EncryptionPolicySettingState <String>]`: complianceStatus
  - `[EncryptionReadinessState <EncryptionReadinessState?>]`: Encryption readiness state
  - `[EncryptionState <EncryptionState?>]`: Encryption state
  - `[FileVaultStates <FileVaultState?>]`: FileVault State
  - `[OSVersion <String>]`: Operating system version of the device
  - `[PolicyDetails <IMicrosoftGraphEncryptionReportPolicyDetails[]>]`: Policy Details
    - `[PolicyId <String>]`: Policy Id for Encryption Report
    - `[PolicyName <String>]`: Policy Name for Encryption Report
  - `[TpmSpecificationVersion <String>]`: Device TPM Version
  - `[UserPrincipalName <String>]`: User name

POLICYDETAILS <IMicrosoftGraphEncryptionReportPolicyDetails\[]>: Policy Details
  - `[PolicyId <String>]`: Policy Id for Encryption Report
  - `[PolicyName <String>]`: Policy Name for Encryption Report

## RELATED LINKS
