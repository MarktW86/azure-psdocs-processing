---
external help file: AIP.dll-Help.xml
online version: https://go.microsoft.com/fwlink/?linkid=845215
schema: 2.0.0
updated_at: 06/11/2017 09:06 AM
ms.date: 06/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-ipclient/Azure%20Information%20Protection/AzureInformationProtection/vlatest/Set-AIPFileClassification.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/release-ipclient/Azure%20Information%20Protection/AzureInformationProtection/vlatest/Set-AIPFileClassification.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/43a2eac57c1cf1690958c9436523a941ea3b027f
ms.topic: reference
author: cabailey
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: cabailey
open_to_public_contributors: false
---

# Set-AIPFileClassification

## SYNOPSIS
Scans a file to automatically set an Azure Information Protection label for a file, according to conditions that are configured in the policy.

## SYNTAX

```
Set-AIPFileClassification [-JustificationMessage <String>] [-Force] [-Owner <String>] [-PreserveFileDetails]
 [-Path] <String[]> [<CommonParameters>]
```

## DESCRIPTION
The Set-AIPFileClassification cmdlet can automatically apply an Azure Information Protection label for one or more files when you configure labels in your Azure Information Protection policy to use conditions. Labels are applied when the conditions are configured for automatic classification. For more information about conditions, see [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/information-protection/deploy-use/configure-policy-classification).

When this cmdlet is run, it inspects the file contents and if the condition is met for a label, that label is applied. This action can automatically apply or remove protection when the applied label is also configured for Rights Management protection in the Azure Information Protection policy.

By default, if the file already has a label, the existing label or protection is not replaced.

Currently, you cannot create or edit labels by using PowerShell but must do this by using the Azure portal. For instructions, see [Configuring Azure Information Protection policy](https://docs.microsoft.com/information-protection/deploy-use/configure-policy).

In addition, this cmdlet does not support a service principal account in Azure Active Directory; you must run it interactively with a user account.

## EXAMPLES

### Example 1: Scan all files in a folder and any of its subfolders, and apply labels according to the configured conditions for automatic classification
```
PS C:\> Set-AIPFileClassification -Path C:\Projects\ -PreserveFileDetails


FileName      : C:\Projects\Project1.docx
Status        : Success
Comment       :
MainLabelName : Confidential
MainLabelId   : 074e257c-1234-1234-1234-34a182080e71
SubLabelName  : Finance group
SubLabelId    : d9f23ae3-1234-1234-1234-f515f824c57b

FileName      : C:\Projects\Datasheet.pdf
Status        : Skipped
Comment       : No conditions match for this file
MainLabelName : 
MainLabelId   : 
SubLabelName  : 
SubLabelId    : 

FileName      : C:\Projects\Analysis.xlsx
Status        : Skipped
Comment       : The file is labeled manually
MainLabelName : 
MainLabelId   : 
SubLabelName  : 
SubLabelId    : 

FileName      : C:\Projects\Pricelist.xlsx
Status        : Skipped
Comment       : The file has a higher classification label
MainLabelName : 
MainLabelId   : 
SubLabelName  : 
SubLabelId    : 

FileName      : C:\Projects\Dashboard.xlsx
Status        : Success
Comment       : 
MainLabelName : Public
MainLabelId   : f018e9e7-0cfc-4c69-b27a-ac3cb7df43cc
SubLabelName  : 
SubLabelId    :
```

This command scans all files in the Projects folder and any of its subfolders, and sets labels according to the configured conditions in the Azure Information Protection policy. In this example, there are five files and two files are automatically labeled. The Datasheet.pdf file is not labeled because its contents does not match the configured conditions for automatic classification Analysis.xlsx was already manually labeled, and Pricelist.xlsx has a higher label. Because the command is run without the *-Force* parameter, the existing labels for Analysis.xlsx and Pricelist.xlsx are not overwritten.

If the applied labels are also configured to apply Rights Management protection, the files that are successfully labeled with this command are also protected. In this case, the Rights Management owner (who has the Rights Management Full Control permission) of these files is the user who ran the PowerShell command.

As PreserveFileDetails is specified, the Date Modified of the files isn't changed.

### Example 2: Scan all files in a folder and any of its subfolders, and apply labels according to the configured conditions for automatic classification, overriding any existing labels
```
PS C:\> Set-AIPFileClassification -Path C:\Projects\ -Force -PreserveFileDetails


FileName      : C:\Projects\Project1.docx
Status        : Success
Comment       :
MainLabelName : Confidential
MainLabelId   : 074e257c-1234-1234-1234-34a182080e71
SubLabelName  : Finance group
SubLabelId    : d9f23ae3-1234-1234-1234-f515f824c57b

FileName      : C:\Projects\Datasheet.pdf
Status        : Skipped
Comment       : No conditions match for this file
MainLabelName : 
MainLabelId   : 
SubLabelName  : 
SubLabelId    : 

FileName      : C:\Projects\Analysis.xlsx
Status        : Success
Comment       :
MainLabelName : Public
MainLabelId   : f018e9e7-0cfc-4c69-b27a-ac3cb7df43cc
SubLabelName  : 
SubLabelId    : 

FileName      : C:\Projects\Pricelist.xlsx
Status        : Success
Comment       :
MainLabelName : Public
MainLabelId   : f018e9e7-0cfc-4c69-b27a-ac3cb7df43cc
SubLabelName  : 
SubLabelId    : 

FileName      : C:\Projects\Dashboard.xlsx
Status        : Success
Comment       : 
MainLabelName : Public
MainLabelId   : f018e9e7-0cfc-4c69-b27a-ac3cb7df43cc
SubLabelName  : 
SubLabelId    :
```

This command is similar to the previous example in that it also scans all files in the Projects folder and any of its subfolders, and sets labels according to the configured conditions in the Azure Information Protection policy. However, this time, because the command includes the *-Force* parameter, it also replaces the existing label for Dashboard.xlsx, and Pricelist.xlsx. The contents of Datasheet.pdf did not match any configured conditions and this file remains without a label.  

## PARAMETERS

### -Force
Replaces an existing label when the configured conditions apply.

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

### -JustificationMessage
The justification reason for lowering the classification label, removing a label, or removing protection, if the Azure Information Protection policy requires users to supply this information.

If setting a label triggers the justification and this reason is not supplied, the label is not applied, even if the *-Force* paramter is set. In this case, the status returned is "Skipped" with the comment "Justification required".

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

### -Path
Specifies a local, network path, or Sharepoint url to the files for which you want to get the label and protection information. Wildcards are not supported.

Examples include C:\Folder\, C:\Folder\Filename, \\\Server\Folder, 'http://sharepoint.contoso.com/Shared Documents/Folder', http://sharepoint.contoso.com/Shared%20Documents/Folder/FileName.

Wildcards are not supported.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: FullName, FileName

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Owner
On the label: the email address used in the Owner custom property. On the protection: the encryption uses the -OwnerEmail. This is the person who will get full control for the item and will be considered to be the encryption owner.```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PreserveFileDetails
When setting a label on a local or network file, will not change the file Last Modified date to now, but will leave it unchanged.
When setting a label on a sharepoint file, will not change neither the file Modified date, nor the file Modified By

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String[]

## OUTPUTS

### Microsoft.InformationProtection.Powershell.AIP.Results.SetAIPFileClassificationResult

## NOTES

## RELATED LINKS

[Get-​AI​PFile​Status](./Get-AIPFileStatus.md)

[Set-AIPFileLabel](./Set-AIPFileLabel.md)

