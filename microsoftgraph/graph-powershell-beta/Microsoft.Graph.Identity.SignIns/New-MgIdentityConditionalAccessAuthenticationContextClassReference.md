---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.identity.signins/new-mgidentityconditionalaccessauthenticationcontextclassreference
schema: 2.0.0
ms.prod: "identity-and-sign-in"
---

# New-MgIdentityConditionalAccessAuthenticationContextClassReference

## SYNOPSIS
Create a new authenticationContextClassReference.

## SYNTAX

### CreateExpanded1 (Default)
```
New-MgIdentityConditionalAccessAuthenticationContextClassReference [-AdditionalProperties <Hashtable>]
 [-Description <String>] [-DisplayName <String>] [-Id <String>] [-IsAvailable] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Create1
```
New-MgIdentityConditionalAccessAuthenticationContextClassReference
 -BodyParameter <IMicrosoftGraphAuthenticationContextClassReference> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new authenticationContextClassReference.

## EXAMPLES

### Example 1: Using the New-MgIdentityConditionalAccessAuthenticationContextClassReference Cmdlet
```powershell
Import-Module Microsoft.Graph.Identity.SignIns
$params = @{
	Id = "c1"
	DisplayName = "Contoso medium"
	Description = "Medium protection level defined for Contoso policy"
	IsAvailable = $true
}
New-MgIdentityConditionalAccessAuthenticationContextClassReference -BodyParameter $params
```

This example shows how to use the New-MgIdentityConditionalAccessAuthenticationContextClassReference Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
authenticationContextClassReference
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAuthenticationContextClassReference
Parameter Sets: Create1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Description
A short explanation of the policies that are enforced by authenticationContextClassReference.
This value should be used to provide secondary text to describe the authentication context class reference when building user-facing admin experiences.
For example, a selection UX.

```yaml
Type: String
Parameter Sets: CreateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
The display name is the friendly name of the authenticationContextClassReference object.
This value should be used to identify the authentication context class reference when building user-facing admin experiences.
For example, a selection UX.

```yaml
Type: String
Parameter Sets: CreateExpanded1
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
Parameter Sets: CreateExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsAvailable
Indicates whether the authenticationContextClassReference has been published by the security admin and is ready for use by apps.
When it is set to false, it should not be shown in authentication context selection UX, or used to protect app resources.
It will be shown and available for Conditional Access policy authoring.
The default value is false.
Supports $filter (eq).

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded1
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAuthenticationContextClassReference
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAuthenticationContextClassReference
## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER `<IMicrosoftGraphAuthenticationContextClassReference>`: authenticationContextClassReference
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique idenfier for an entity. Read-only.
  - `[Description <String>]`: A short explanation of the policies that are enforced by authenticationContextClassReference. This value should be used to provide secondary text to describe the authentication context class reference when building user-facing admin experiences. For example, a selection UX.
  - `[DisplayName <String>]`: The display name is the friendly name of the authenticationContextClassReference object. This value should be used to identify the authentication context class reference when building user-facing admin experiences. For example, a selection UX.
  - `[IsAvailable <Boolean?>]`: Indicates whether the authenticationContextClassReference has been published by the security admin and is ready for use by apps. When it is set to false, it should not be shown in authentication context selection UX, or used to protect app resources. It will be shown and available for Conditional Access policy authoring. The default value is false.  Supports $filter (eq).

## RELATED LINKS
