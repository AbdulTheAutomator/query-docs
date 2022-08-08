---
description: "Learn more about: Date.StartOfWeek"
title: "Date.StartOfWeek"
ms.date: 3/11/2022
---
# Date.StartOfWeek

## Syntax

<pre>
Date.StartOfWeek(<b>dateTime</b> as any, optional <b>firstDayOfWeek</b> as nullable number) as any 
</pre>
  
## About

Returns the first value of the week given a `date`, `datetime`, or `datetimezone` value.

## Example 1

Find the start of the week for October 10th, 2011, 8:10:32AM (`#datetime(2011, 10, 10, 8, 10, 32)`).

**Usage**

```powerquery-m
Date.StartOfWeek(#datetime(2011, 10, 10, 8, 10, 32))
```

**Output**

`#datetime(2011, 10, 9, 0, 0, 0)`
