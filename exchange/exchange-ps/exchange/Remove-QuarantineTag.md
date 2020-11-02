---
external help file: Microsoft.Exchange.TransportMailflow-Help.xml
online version: https://docs.microsoft.com/powershell/module/exchange/remove-quarantinetag
applicable: Exchange Online, Exchange Online Protection
title: Remove-QuarantineTag
schema: 2.0.0
author: chrisda
ms.author: chrisda
ms.reviewer:
---

# Remove-QuarantineTag

## SYNOPSIS
This cmdlet is available only in the cloud-based service.

Use the Remove-QuarantineTag cmdlet to remove custom quarantine tags from your cloud-based organization.

**Note**: We recommend that you use the Exchange Online PowerShell V2 module to connect to Exchange Online PowerShell. For instructions, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

For information about the parameter sets in the Syntax section below, see [Exchange cmdlet syntax](https://docs.microsoft.com/powershell/exchange/exchange-cmdlet-syntax).

## SYNTAX

```
Remove-QuarantineTag [-Identity] <QuarantineTagIdParameter>
 [-DomainController <Fqdn>]
 [<CommonParameters>]
```

## DESCRIPTION
You can't remove built-in quarantine tags that start with "Default" in the name.

You need to be assigned permissions before you can run this cmdlet. Although this topic lists all parameters for the cmdlet, you may not have access to some parameters if they're not included in the permissions assigned to you. To find the permissions required to run any cmdlet or parameter in your organization, see [Find the permissions required to run any Exchange cmdlet](https://docs.microsoft.com/powershell/exchange/find-exchange-cmdlet-permissions).

## EXAMPLES

### Example 1
```powershell
Remove-QuarantineTag -Identity "Contoso Engineering"
```

This example removes the quarantine tag named Contoso Engineering.

## PARAMETERS

### -Identity
The Identity parameter specifies the quarantine tag you want to remove. You can use any value that uniquely identifies the quarantine tag. For example:

- Name
- Distinguished name (DN)
- GUID

```yaml
Type: QuarantineTagIdParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Online, Exchange Online Protection

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -DomainController
This parameter is reserved for internal Microsoft use.

```yaml
Type: Fqdn
Parameter Sets: (All)
Aliases:
Applicable: Exchange Online, Exchange Online Protection

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](https://go.microsoft.com/fwlink/p/?LinkID=113216).

## INPUTS

###  

## OUTPUTS

###  

## NOTES

## RELATED LINKS