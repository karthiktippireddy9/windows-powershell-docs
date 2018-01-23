---
external help file: WssCmdlets.dll-Help.xml
online version: 
schema: 2.0.0
title: Set-WssFileHistoryManagementStatus
description: 
keywords: powershell, cmdlet
author: brianlic
manager: alanth
ms.date: 2017-12-05
ms.topic: reference
ms.prod: powershell
ms.technology: powershell
ms.assetid: 896C4B21-95AA-4BE0-B8FA-F727222C47AC
---

# Set-WssFileHistoryManagementStatus

## SYNOPSIS
Changes the File History managed status of a user account.

## SYNTAX

```
Set-WssFileHistoryManagementStatus [-UserName] <String> [-UnManage] [-Delete] [-Force] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
The **Set-WssFileHistoryManagementStatus** cmdlet changes the File History managed status of a user account.
Specify the **UnManage** parameter if you do not want the server to manage the user account that you specify in the **UserName** parameter.

## EXAMPLES

### Example 1: Change the File History managed status of a computer
```
PS C:\> Set-WssFileHistoryManagementStatus -UserName "DaveB" -UnManage -Delete
```

This command changes the File History managed status of a user named DaveB to unmanaged, and deletes the File History Backup folder for that account.

## PARAMETERS

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Delete
Indicates that the cmdlet also deletes the File History Backup folder for the user account when you specify the **UnManage** parameter.

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

### -Force
Forces the command to run without asking for user confirmation.

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

### -UnManage
Indicates that the server no longer manages the File History of the user account.

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

### -UserName
Specifies the user name whose File History you want to manage.

```yaml
Type: String
Parameter Sets: (All)
Aliases: un

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
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
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

## NOTES

## RELATED LINKS
