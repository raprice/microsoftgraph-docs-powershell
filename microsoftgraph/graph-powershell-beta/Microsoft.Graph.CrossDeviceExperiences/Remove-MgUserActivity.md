---
external help file: Microsoft.Graph.CrossDeviceExperiences-help.xml
Module Name: Microsoft.Graph.CrossDeviceExperiences
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.crossdeviceexperiences/remove-mguseractivity
schema: 2.0.0
---

# Remove-MgUserActivity

## SYNOPSIS
Delete navigation property activities for users

## SYNTAX

### Delete (Default)
```
Remove-MgUserActivity -UserActivityId <String> -UserId <String> [-IfMatch <String>] [-PassThru] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### DeleteViaIdentity
```
Remove-MgUserActivity -InputObject <ICrossDeviceExperiencesIdentity> [-IfMatch <String>] [-PassThru] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Delete navigation property activities for users

## EXAMPLES

### Example 1: Using the Remove-MgUserActivity Cmdlet
```powershell
Import-Module Microsoft.Graph.CrossDeviceExperiences
# A UPN can also be used as -UserId.
Remove-MgUserActivity -UserId $userId -UserActivityId $userActivityId
```

This example shows how to use the Remove-MgUserActivity Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -IfMatch
ETag

```yaml
Type: String
Parameter Sets: (All)
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
Type: ICrossDeviceExperiencesIdentity
Parameter Sets: DeleteViaIdentity
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

### -UserActivityId
key: id of userActivity

```yaml
Type: String
Parameter Sets: Delete
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserId
key: id of user

```yaml
Type: String
Parameter Sets: Delete
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

### Microsoft.Graph.PowerShell.Models.ICrossDeviceExperiencesIdentity
## OUTPUTS

### System.Boolean
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


INPUTOBJECT `<ICrossDeviceExperiencesIdentity>`: Identity Parameter
  - `[ActivityHistoryItemId <String>]`: key: id of activityHistoryItem
  - `[CommandId <String>]`: key: id of command
  - `[DeviceId <String>]`: key: id of device
  - `[DirectoryObjectId <String>]`: key: id of directoryObject
  - `[ExtensionId <String>]`: key: id of extension
  - `[UsageRightId <String>]`: key: id of usageRight
  - `[UserActivityId <String>]`: key: id of userActivity
  - `[UserId <String>]`: key: id of user

## RELATED LINKS
