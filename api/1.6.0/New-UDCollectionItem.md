---
external help file: UniversalDashboard-help.xml
online version: 
schema: 2.0.0
---

# New-UDCollectionItem

## SYNOPSIS
Creates a new collection item.

## SYNTAX

### content (Default)
```
New-UDCollectionItem [-Id <String>] [-Content <ScriptBlock>] [-SecondaryContent <ScriptBlock>] [-Active]
```

### link
```
New-UDCollectionItem [-Id <String>] [-Content <ScriptBlock>] [-Url <String>] [-Active]
```

## DESCRIPTION
Creates a new collection item.

## EXAMPLES

### Example 1
```
PS C:\> New-UDCollection -Content {
    New-UDCollectionItem -Content { 
        "Item 1"
    }
    New-UDCollectionItem -Content { 
        "Item 2"
    }
    New-UDCollectionItem -Content { 
        "Item 3"
    }
}
```

Creates a collection of 3 items.

## PARAMETERS

### -Active
Whether this collection item is active.

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

### -Content
The content for this collection item.

```yaml
Type: ScriptBlock
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
The ID of this collection item.

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

### -SecondaryContent
Secondary content for this collection item.

```yaml
Type: ScriptBlock
Parameter Sets: content
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Url
URL for this collection item. This should be used when New-UDCollection has the LinksCollection parameter specified.

```yaml
Type: String
Parameter Sets: link
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

### None


## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS

