---
description: "Learn more about: Duration.TotalSeconds"
title: "Duration.TotalSeconds"
ms.date: 7/18/2022
---
# Duration.TotalSeconds

## Syntax

<pre>
Duration.TotalSeconds(<b>duration</b> as nullable duration) as nullable number
</pre>
  
## About

Returns the total seconds spanned by `duration`.

## Example 1

Find the total seconds spanned by a duration value.

**Usage**

```powerquery-m
Duration.TotalSeconds(#duration(5, 4, 3, 2))
```

**Output**

`446582`
