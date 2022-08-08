---
description: "Learn more about: Table.Buffer"
title: "Table.Buffer"
ms.date: 4/13/2022
---
# Table.Buffer

## Syntax

<pre>
Table.Buffer(<b>table</b> as table, optional <b>options</b> as nullable record) as table
</pre>
  
## About

Buffers a table in memory, isolating it from external changes during evaluation. Buffering is shallow. It forces the evaluation of any scalar cell values, but leaves non-scalar values (records, lists, tables, and so on) as-is.

Note that using this function might or might not make your queries run faster. In some cases, it can make your queries run more slowly due to the added cost of reading all the data and storing it in memory, as well as the fact that buffering prevents downstream folding. If the data doesn't need to be buffered but you just want to prevent downstream folding, use [Table.StopFolding](/powerquery-m/table-stopfolding) instead.

## Example 1

Load all the rows of a SQL table into memory, so that any downstream operations will no longer be able to query the SQL server.

**Usage**

```powerquery-m
let
    Source = Sql.Database("SomeSQLServer", "MyDb"),
    MyTable = Source{[Item="MyTable"]}[Data],
    BufferMyTable = Table.Buffer(dbo_MyTable)
in
    BufferMyTable
```

**Output**

```powerquery-m
table
```
