---
description: "Learn more about: Table.ReplaceValue"
title: "Table.ReplaceValue"
ms.date: 5/19/2022
---
# Table.ReplaceValue

## Syntax

<pre>
Table.ReplaceValue(<b>table</b> as table, <b>oldValue</b> as any, <b>newValue</b> as any, <b>replacer</b> as function, <b>columnsToSearch</b> as list) as table
</pre>
  
## About

Replaces `oldValue` with `newValue` in the specified columns of the `table`.

## Example 1

Replace the text "goodbye" with the text "world" in the table.

**Usage**

```powerquery-m
Table.ReplaceValue(
    Table.FromRecords({
        [a = 1, b = "hello"],
        [a = 3, b = "goodbye"]
    }),
    "goodbye",
    "world",
    Replacer.ReplaceText,
    {"b"}
)
```

**Output**

```powerquery-m
Table.FromRecords({
    [a = 1, b = "hello"],
    [a = 3, b = "world"]
})
```

## Example 2

Replace the text "ur" with the text "or" in the table.

**Usage**

```powerquery-m
Table.ReplaceValue(
    Table.FromRecords({
        [a = 1, b = "hello"],
        [a = 3, b = "wurld"]
    }),
    "ur",
    "or",
    Replacer.ReplaceText,
    {"b"}
)
```

**Output**

```powerquery-m
Table.FromRecords({
    [a = 1, b = "hello"],
    [a = 3, b = "world"]
})
```
