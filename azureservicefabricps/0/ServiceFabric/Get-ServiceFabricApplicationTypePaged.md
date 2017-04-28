---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 04/06/2017 14:04 PM
ms.date: 04/06/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/V5.6_Updates/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricApplicationTypePaged.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/V5.6_Updates/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricApplicationTypePaged.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/8cc7df560eb5276f5793b86a2b9d29aa7dfc34dd
ms.topic: reference
author: oanapl
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: vipulm
open_to_public_contributors: false
ms.service: service-fabric
---

# Get-ServiceFabricApplicationTypePaged

## SYNOPSIS
{{Fill in the Synopsis}}

## SYNTAX

### OnePage (Default)
```
Get-ServiceFabricApplicationTypePaged [-ApplicationTypeName <String>] [-ExcludeApplicationParameters]
 [-MaxResults <Int64>] [-ContinuationToken <String>] [-ExcludeContinuationToken] [-TimeoutSec <Int32>]
```

### AllPages
```
Get-ServiceFabricApplicationTypePaged [-ApplicationTypeName <String>] [-ExcludeApplicationParameters]
 [-MaxResults <Int64>] [-ContinuationToken <String>] [-GetAllPages] [-TimeoutSec <Int32>]
```

## DESCRIPTION
{{Fill in the Description}}

## EXAMPLES

### Example 1
```
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -ApplicationTypeName
{{Fill ApplicationTypeName Description}}

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ContinuationToken
{{Fill ContinuationToken Description}}

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

### -ExcludeApplicationParameters
{{Fill ExcludeApplicationParameters Description}}

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

### -ExcludeContinuationToken
{{Fill ExcludeContinuationToken Description}}

```yaml
Type: SwitchParameter
Parameter Sets: OnePage
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GetAllPages
{{Fill GetAllPages Description}}

```yaml
Type: SwitchParameter
Parameter Sets: AllPages
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MaxResults
{{Fill MaxResults Description}}

```yaml
Type: Int64
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeoutSec
{{Fill TimeoutSec Description}}

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

### System.String


## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS

