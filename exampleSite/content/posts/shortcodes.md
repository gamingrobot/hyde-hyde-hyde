+++
title = "Hyde-hyde-hyde Shortcodes"
date = "2023-02-16"
description = "A brief description of Hugo Shortcodes"
tags = [
    "shortcodes",
]
+++

Custom shortcodes in hyde-hyde-hyde
<!--more-->
---

## fig

{{< fig src="/img/hugo.png" link="/" caption="no alignment" alt="this is alt text" align="" width="50px" height="50px" >}}

With no alignment the text just goes after the figure

{{< fig src="/img/hugo.png" link="/" caption="center align" alt="this is alt text" align="center" width="50px" height="50px" >}}

With center alignment text behaves the same way as no alignment but now the figure is centered

{{< fig src="/img/hugo.png" link="/" caption="left align" alt="this is alt text" align="left" width="50px" height="50px" >}}

{{< fig src="/img/hugo.png" link="/" caption="right align" alt="this is alt text" align="right" width="50px" height="50px" >}}

With left or right alignment the text is allowed to flow around the figure on either side  
Here is some more filler text to show how that works



---

## kbd

{{< kbd testing >}}

---

## mermaid

{{< mermaid >}}
pie
    title French Words I Know
    "Merde" : 50
    "Oui" : 35
    "Alors" : 10
    "Non" : 5
{{< /mermaid >}}

---

## Notes

### tip

{{< tip >}}
This is a tip note
{{< /tip >}}

### info

{{< info >}}
This is a info note
{{< /info >}}

### warning

{{< warning >}}
This is a warning note
{{< /warning >}}

### danger

{{< danger >}}
This is a danger note
{{< /danger >}}
