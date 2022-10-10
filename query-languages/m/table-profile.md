---
description: "Learn more about: Table.Profile"
title: "Table.Profile"
ms.date: 10/7/2022
---
# Table.Profile

## Syntax

<pre>
Table.Profile(<b>table</b> as table, optional <b>additionalAggregates</b> as nullable list) as table
</pre>
  
## About

Returns a profile for the columns in `table`.

The following information is returned for each column (when applicable):

* minimum
* maximum
* average
* standard deviation
* count
* null count
* distinct count
