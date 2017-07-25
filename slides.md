<!-- .slide: data-state="no-toc-progress" --> <!-- don't show toc progress bar on this slide -->

# UP AND SIDEWAYS
<!-- .element: class="no-toc-progress" --> <!-- slide not in toc progress bar -->

## Migrating legal content from RTF to XML

[Ari Nordström](ari@sgmlguru.org) | Balisage 2017-07-31 | [online][1] | [src][2]


[1]: https://theno.github.io/revealjs_template
[2]: https://github.com/theno/revealjs_template

[3]: http://lab.hakim.se/reveal-js/
[4]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
[5]: http://www.fabfile.org/
[6]: https://github.com/theno/fabsetup


----  ----

<!-- .slide: data-state="no-toc-progress" --> <!-- don't show toc progress bar on this slide -->

# What we had to work with

----

<!-- .slide: data-state="no-toc-progress" --> <!-- don't show toc progress bar on this slide -->

## Halsbury Laws of England - 104 vols

  - Vol paras
  - Multiple ordered lists
  - Chapter/section/appendix structure
  - Citations (Commentary title refs, caselaw, legislation)


----  ----

<!-- .slide: data-state="no-toc-progress" --> <!-- don't show toc progress bar on this slide -->

# RTF -> docx -> XHTML -> XML

----

<!-- .slide: data-state="no-toc-progress" --> <!-- don't show toc progress bar on this slide -->

* Aspose
* "Flat" XHTML with processing attr = RTF style name

----  ----

<!-- .slide: data-state="no-toc-progress" --> <!-- don't show toc progress bar on this slide -->

# Pipeline approach, multiple steps (one XSLT each)

----

<!-- .slide: data-state="no-toc-progress" --> <!-- don't show toc progress bar on this slide -->

* Nic's XProc tools
* Narrow focus per step
* Easier to add and remove functionality
* Easier to debug
* ID transforms with modes

----  ----

<!-- .slide: data-state="no-toc-progress" --> <!-- don't show toc progress bar on this slide -->

# Adding semantics


----

<!-- .slide: data-state="no-toc-progress" --> <!-- don't show toc progress bar on this slide -->

* Wrappers from flat XHTML
* Start/End RTF styles
* Infer list items, headings, footnotes (label, separator, contents)
* for-each-groups
* following-sibling to add to group, descendant to remove duplicates
* LOTS of regular expressions

----  ----

<!-- .slide: data-state="no-toc-progress" --> <!-- don't show toc progress bar on this slide -->

# QA

----

<!-- .slide: data-state="no-toc-progress" --> <!-- don't show toc progress bar on this slide -->

- XSpec (writing XSLT)
- XSpec (testing conversion steps)
- Schematron
- DTD (obviously)

----  ----

<!-- .slide: data-state="no-toc-progress" --> <!-- don't show toc progress bar on this slide -->

### *Thank You for Your attention!*
<!-- .element: class="no-toc-progress" -->

![](img/thanks.jpg)
