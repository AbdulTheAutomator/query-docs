---
description: "Learn more about: Text.ToList"
title: "Text.ToList"
ms.date: 3/11/2022
---
# Text.ToList

## Syntax

<pre>
Text.ToList(<b>text</b> as text) as list
</pre>
  
## About

Returns a list of character values from the given text value `text`.

## Example 1

Create a list of character values from the text "Hello World".

**Usage**

```powerquery-m
Text.ToList("Hello World")
```

**Output**

```powerquery-m{
    "H",
    "e",
    "l",
    "l",
    "o",
    " ",
    "W",
    "o",
    "r",
    "l",
    "d"
}
```
