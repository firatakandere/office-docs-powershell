---
external help file: Microsoft.Exchange.TransportMailflow-Help.xml
online version: https://docs.microsoft.com/powershell/module/exchange/get-safeattachmentrule
applicable: Exchange Online, Exchange Online Protection
title: Get-SafeAttachmentRule
schema: 2.0.0
author: chrisda
ms.author: chrisda
ms.reviewer:
---

# Get-SafeAttachmentRule

## SYNOPSIS
This cmdlet is available only in the cloud-based service.

Use the Get-SafeAttachmentRule cmdlet to view safe attachment rules in your cloud-based organization.

For information about the parameter sets in the Syntax section below, see [Exchange cmdlet syntax](https://docs.microsoft.com/powershell/exchange/exchange-cmdlet-syntax).

## SYNTAX

```
Get-SafeAttachmentRule [[-Identity] <RuleIdParameter>]
 [-State <RuleState>]
 [<CommonParameters>]
```

## DESCRIPTION
Safe Attachments is a feature in Microsoft Defender for Office 365 that opens email attachments in a special hypervisor environment to detect malicious activity. For more information, see [Safe Attachments in Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-attachments).

You need to be assigned permissions before you can run this cmdlet. Although this topic lists all parameters for the cmdlet, you may not have access to some parameters if they're not included in the permissions assigned to you. To find the permissions required to run any cmdlet or parameter in your organization, see [Find the permissions required to run any Exchange cmdlet](https://docs.microsoft.com/powershell/exchange/find-exchange-cmdlet-permissions).

## EXAMPLES

### Example 1
```powershell
Get-SafeAttachmentRule
```

This example returns a summary list of all safe attachment rules in your organization.

### Example 2
```powershell
Get-SafeAttachmentRule -Identity "Research Department Attachment Rule" | Format-List
```

This example returns detailed information about the safe attachment rule named Research Department Attachment Rule.

## PARAMETERS

### -Identity
The Identity parameter specifies the safe attachment rule that you want to view.

You can use any value that uniquely identifies the rule. For example:

- Name
- Distinguished name (DN)
- GUID

```yaml
Type: RuleIdParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Online, Exchange Online Protection

Required: False
Position: 1
Default value: None
Accept pipeline input: True
Accept wildcard characters: False
```

### -State
The State parameter filters the results by the state of the rule. Valid values are Enabled and Disabled.

```yaml
Type: RuleState
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
