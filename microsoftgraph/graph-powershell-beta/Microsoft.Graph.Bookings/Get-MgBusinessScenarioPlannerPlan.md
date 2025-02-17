---
external help file: Microsoft.Graph.Bookings-help.xml
Module Name: Microsoft.Graph.Bookings
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.bookings/get-mgbusinessscenarioplannerplan
schema: 2.0.0
---

# Get-MgBusinessScenarioPlannerPlan

## SYNOPSIS
Invoke action getPlan

## SYNTAX

### GetExpanded (Default)
```
Get-MgBusinessScenarioPlannerPlan -BusinessScenarioId <String> [-AdditionalProperties <Hashtable>]
 [-Target <IMicrosoftGraphBusinessScenarioTaskTargetBase>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Get
```
Get-MgBusinessScenarioPlannerPlan -BusinessScenarioId <String>
 -BodyParameter <IPaths1Tvx8HxSolutionsBusinessscenariosBusinessscenarioIdPlannerMicrosoftGraphGetplanPostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### GetViaIdentityExpanded
```
Get-MgBusinessScenarioPlannerPlan -InputObject <IBookingsIdentity> [-AdditionalProperties <Hashtable>]
 [-Target <IMicrosoftGraphBusinessScenarioTaskTargetBase>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgBusinessScenarioPlannerPlan -InputObject <IBookingsIdentity>
 -BodyParameter <IPaths1Tvx8HxSolutionsBusinessscenariosBusinessscenarioIdPlannerMicrosoftGraphGetplanPostRequestbodyContentApplicationJsonSchema>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Invoke action getPlan

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: GetExpanded, GetViaIdentityExpanded
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
Type: IPaths1Tvx8HxSolutionsBusinessscenariosBusinessscenarioIdPlannerMicrosoftGraphGetplanPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Get, GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -BusinessScenarioId
key: id of businessScenario

```yaml
Type: String
Parameter Sets: GetExpanded, Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, please use Get-Help -Online and see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IBookingsIdentity
Parameter Sets: GetViaIdentityExpanded, GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Target
businessScenarioTaskTargetBase
To construct, please use Get-Help -Online and see NOTES section for TARGET properties and create a hash table.

```yaml
Type: IMicrosoftGraphBusinessScenarioTaskTargetBase
Parameter Sets: GetExpanded, GetViaIdentityExpanded
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

### Microsoft.Graph.PowerShell.Models.IBookingsIdentity
### Microsoft.Graph.PowerShell.Models.IPaths1Tvx8HxSolutionsBusinessscenariosBusinessscenarioIdPlannerMicrosoftGraphGetplanPostRequestbodyContentApplicationJsonSchema
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphBusinessScenarioPlanReference
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IPaths1Tvx8HxSolutionsBusinessscenariosBusinessscenarioIdPlannerMicrosoftGraphGetplanPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Target <IMicrosoftGraphBusinessScenarioTaskTargetBase>]`: businessScenarioTaskTargetBase
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[TaskTargetKind <String>]`: plannerTaskTargetKind

INPUTOBJECT `<IBookingsIdentity>`: Identity Parameter
  - `[BookingAppointmentId <String>]`: key: id of bookingAppointment
  - `[BookingBusinessId <String>]`: key: id of bookingBusiness
  - `[BookingCurrencyId <String>]`: key: id of bookingCurrency
  - `[BookingCustomQuestionId <String>]`: key: id of bookingCustomQuestion
  - `[BookingCustomerBaseId <String>]`: key: id of bookingCustomerBase
  - `[BookingCustomerId <String>]`: key: id of bookingCustomer
  - `[BookingServiceId <String>]`: key: id of bookingService
  - `[BookingStaffMemberBaseId <String>]`: key: id of bookingStaffMemberBase
  - `[BookingStaffMemberId <String>]`: key: id of bookingStaffMember
  - `[BusinessScenarioId <String>]`: key: id of businessScenario
  - `[BusinessScenarioTaskId <String>]`: key: id of businessScenarioTask
  - `[PlannerPlanConfigurationLocalizationId <String>]`: key: id of plannerPlanConfigurationLocalization

TARGET `<IMicrosoftGraphBusinessScenarioTaskTargetBase>`: businessScenarioTaskTargetBase
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[TaskTargetKind <String>]`: plannerTaskTargetKind

## RELATED LINKS
