---
title: Regular expressions - Azure Data Explorer
description: This article describes Regular expressions in Azure Data Explorer.
ms.reviewer: alexans
ms.topic: reference
ms.date: 04/29/2021
---
# RE2 syntax

RE2 regular expression syntax describes the syntax of the regular expression library used by Kusto (re2).
There are a few functions in Kusto that perform string matching, selection, and extraction by using a regular expression

- [countof()](countoffunction.md)
- [extract()](extractfunction.md)
- [extract_all()](extractallfunction.md)
- [matches regex](datatypes-string-operators.md)
- [parse operator](parseoperator.md)
- [replace()](replace-regex-function.md)
- [trim()](trimfunction.md)
- [trimend()](trimendfunction.md)
- [trimstart()](trimstartfunction.md)

The regular expression syntax supported by Kusto is that of the
[re2 library](re2-library.md). These expressions must be encoded in Kusto as `string` literals, and all of Kusto's string quoting rules apply. For example, the regular expression `\A` matches the beginning of a line, and is specified in Kusto as the string literal `"\\A"` (note the "extra" backslash (`\`) character).
