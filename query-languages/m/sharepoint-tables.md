---
description: "Learn more about: SharePoint.Tables"
title: "SharePoint.Tables"
ms.date: 10/7/2022
---
# SharePoint.Tables

## Syntax

<pre>
SharePoint.Tables(<b>url</b> as text, optional <b>options</b> as nullable record) as table
</pre>

## About

Returns a table containing a row for each List item found at the specified SharePoint list, `url`. Each row contains properties of the List. `options` may be specified to control the following options:

* `ApiVersion`: A number (14 or 15) or the text "Auto" that specifies the SharePoint API version to use for this site. When not specified, API version 14 is used. When Auto is specified, the server version will be automatically discovered if possible, otherwise version defaults to 14. Non-English SharePoint sites require at least version 15.
* `Implementation`
* `ViewMode`
