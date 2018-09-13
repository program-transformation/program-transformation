::: {.fullPage}
::: {.twikiMiddleContainer}
::: {.twikiLeftBar}
::: {.twikiLeftBarContents}
[Home](WebHome){.twikiLink}

**XT Tools**

-   [Reference Docs](ToolReference){.twikiLink}
-   [GPP](GenericPrettyPrinter){.twikiLink}
-   [ATerm](ATermTools){.twikiLink}
-   [SDF](SdfTools){.twikiLink}
-   [AsFix](AsFixTools){.twikiLink}

**Languages**

-   [Stratego](../Stratego/WebHome){.twikiLink}
-   [SDF](../Sdf/WebHome){.twikiLink}
-   [ATerm](ATermFormat){.twikiLink}

**Software**

-   [Stratego/XT](../Stratego/StrategoDownload){.twikiLink}
-   [SDF2 Bundle](../Sdf/SdfBundle){.twikiLink}
-   [KoalaCompiler](KoalaCompiler){.twikiLink}
-   [AutoBundle](AutoBundle){.twikiLink}
-   [AutoBuild](AutoBuild){.twikiLink}
-   [DailyBuildSystem](DailyBuildSystem){.twikiLink}

[![](http://www.program-transformation.org/twiki/pub/rss.gif "RSS 1.0 feed")](http://www.program-transformation.org/twiki/bin/view/Tools/WebRss?skin=rss)
:::
:::

::: {.twikiMain}
::: {.toolBar}
::: {.flexMenuBar}
::: {.flexMenu onmouseover="return showMenu(event, 100);" onmouseout="return hideMenu(event, 100);"}
Page

::: {#flexMenuContent100 .flexMenuContent}
-   [Edit
    Page](http://www.program-transformation.org/edit/Tools/PrettyPrintTableDiff?t=1536825866)
-   [Rename
    Page](http://www.program-transformation.org/rename/Tools/PrettyPrintTableDiff)
-   [Attach
    File](http://www.program-transformation.org/attach/Tools/PrettyPrintTableDiff)

<!-- -->

-   [Printable](http://www.program-transformation.org/view/Tools/PrettyPrintTableDiff?skin=print.pattern)
-   [Wiki
    Source](http://www.program-transformation.org/view/Tools/PrettyPrintTableDiff?skin=text&raw=on&contenttype=text/plain)

<!-- -->

-   [Rev
    3](http://www.program-transformation.org/view/Tools/PrettyPrintTableDiff?rev=1.3)
    [(diff 2)](http://www.program-transformation.org/rdiff/Tools/PrettyPrintTableDiff?rev1=1.3&rev2=1.2)
-   [Rev
    2](http://www.program-transformation.org/view/Tools/PrettyPrintTableDiff?rev=1.2)
    [(diff 1)](http://www.program-transformation.org/rdiff/Tools/PrettyPrintTableDiff?rev1=1.2&rev2=1.1)
-   [Rev
    1](http://www.program-transformation.org/view/Tools/PrettyPrintTableDiff?rev=1.1)
-   [Total
    History](http://www.program-transformation.org/rdiff/Tools/PrettyPrintTableDiff)

<!-- -->

-   [More
    \...](http://www.program-transformation.org/oops/Tools/PrettyPrintTableDiff?template=oopsmore&param1=1.3&param2=1.3)
:::
:::

::: {.flexMenu onmouseover="return showMenu(event, 102);" onmouseout="return hideMenu(event, 102);"}
Web

::: {#flexMenuContent102 .flexMenuContent}
-   [Recent Changes](WebChanges){.twikiLink}
-   [Notify Service](WebNotify){.twikiLink}
-   [News](WebNews){.twikiLink}

<!-- -->

-   [Page Index](WebIndex){.twikiLink}
-   [Search](WebSearch){.twikiLink}

<!-- -->

-   [More
    \...](http://www.program-transformation.org/oops/Tools/PrettyPrintTableDiff?template=oopsmore&param1=1.3&param2=1.3)
:::
:::

::: {.flexMenu onmouseover="return showMenu(event, 103);" onmouseout="return hideMenu(event, 103);"}
Wiki

::: {#flexMenuContent103 .flexMenuContent}
-   [About
    TWiki](http://www.program-transformation.org/view/TWiki/WebHome)
-   [Text
    Formatting](http://www.program-transformation.org/view/TWiki/TextFormattingRules)

<!-- -->

-   [Registration](http://www.program-transformation.org/view/TWiki/TWikiRegistration)
-   [Change
    Password](http://www.program-transformation.org/view/TWiki/ChangePassword)
-   [Reset
    Password](http://www.program-transformation.org/view/TWiki/ResetPassword)

<!-- -->

-   [Users](http://www.program-transformation.org/view/Main/TWikiUsers)
-   [Groups](http://www.program-transformation.org/view/Main/TWikiGroups)
:::
:::
:::
:::

::: {.twikiTopic}
Pretty Print Table Diff {#pretty-print-table-diff .twikiTopicTitle}
=======================

::: {.twikiWebTitle}
XT \-- A Bundle of Program Transformation Tools
:::

**Name**

pptable-diff

**Synopsis**

pptable-diff \[\--patch\] \[\--prune\] \[-o output\] \[\--new
\<table\>\] \--old \<table\>

**Description**

This program writes to standard error a list of pretty-print rules that
are contained in pretty-print table \"old\" but not in \"new\" and, vice
versa. Optionally, this tool patches the pretty-print table \"old\" by
adding new and/or removing obsolete pretty-print entries.

**Options**

 -h
:   display usage information. Use this option to get information on
    additional options.

<!-- -->

 \--new \<table\>
:   New pretty-print table. Typically, this is a pretty-print table
    recently generated by
    [ppgen[^?^](http://www.program-transformation.org/edit/Tools/PrettyPrintTableGenerator?topicparent=Tools.PrettyPrintTableDiff)]{.twikiNewLink
    style="background : #FFFFCE;"}. If missing, standard input is used
    to read a table from.

<!-- -->

 \--old \<table\>
:   Old pretty-print table. Typically, this is a (manually) customized
    pretty-print table.

<!-- -->

 \--patch
:   Bring old table up-to-date. If this switch is specified, the table
    \"old\" is updated by adding pretty-print rules that are in \"new\"
    but not in \"old\".

<!-- -->

 \--prune
:   Remove obsolete pretty-print entries. If this switch is specified,
    the table \"old\" is returned after removing obsolete pretty-print
    entries (i.e., entries that are not contained in \"new\").

**See also**

[GenericPrettyPrinter](GenericPrettyPrinter){.twikiLink},
[HowToPrettyPrintAGrammar](HowToPrettyPrintAGrammar){.twikiLink},
[HowToDefinePrettyPrintTables](HowToDefinePrettyPrintTables){.twikiLink},
[PrettyPrintTables](PrettyPrintTable){.twikiLink},
[BoxLanguage](BoxLanguage){.twikiLink},
[PrettyPrintTableGenerator[^?^](http://www.program-transformation.org/edit/Tools/PrettyPrintTableGenerator?topicparent=Tools.PrettyPrintTableDiff)]{.twikiNewLink
style="background : #FFFFCE;"}

\-- [MerijnDeJonge](../Main/MerijnDeJonge){.twikiLink} - 10 Feb 2004\
[]{#TopicEnd}
:::

::: {.twikiTopicInfo .twikiRevInfo .twikiGrayText .twikiMoved}
:::
:::
:::
:::