::: {.fullPage}
::: {.twikiMiddleContainer}
::: {.twikiLeftBar}
::: {.twikiLeftBarContents}
**[SDF Home](WebHome){.twikiLink}**

-   [About](SdfLanguage){.twikiLink}
-   [Documentation](SdfDocumentation){.twikiLink}
-   [Publications](SdfPublications){.twikiLink}
-   [Download](SdfSoftware){.twikiLink}
-   [Grammars](SdfGrammars){.twikiLink}

**Users**

-   [Applications](SdfApplications){.twikiLink}
-   [Mailing Lists](MailingList){.twikiLink}
-   [ASF+SDF Users
    Day](http://www.cwi.nl/htbin/sen1/twiki/bin/view/SEN1/ASFSDFUsersDay)
-   [Stratego Users Day](../Stratego/StrategoUsersDay){.twikiLink}

**Development**

-   [Organization](SdfDevelopment){.twikiLink}
-   [Reporting Bugs](SdfBugs){.twikiLink}
:::
:::

::: {.twikiMain}
::: {.toolBar}
::: {.flexMenuBar}
::: {.flexMenu onmouseover="return showMenu(event, 100);" onmouseout="return hideMenu(event, 100);"}
Page

::: {#flexMenuContent100 .flexMenuContent}
-   [Edit
    Page](http://www.program-transformation.org/edit/SdfBackup/GeneralizedLR?t=1536827742)
-   [Rename
    Page](http://www.program-transformation.org/rename/SdfBackup/GeneralizedLR)
-   [Attach
    File](http://www.program-transformation.org/attach/SdfBackup/GeneralizedLR)

<!-- -->

-   [Printable](http://www.program-transformation.org/view/SdfBackup/GeneralizedLR?skin=print.pattern)
-   [Wiki
    Source](http://www.program-transformation.org/view/SdfBackup/GeneralizedLR?skin=text&raw=on&contenttype=text/plain)

<!-- -->

-   [Rev
    8](http://www.program-transformation.org/view/SdfBackup/GeneralizedLR?rev=1.8)
    [(diff 7)](http://www.program-transformation.org/rdiff/SdfBackup/GeneralizedLR?rev1=1.8&rev2=1.7)
-   [Rev
    7](http://www.program-transformation.org/view/SdfBackup/GeneralizedLR?rev=1.7)
    [(diff 6)](http://www.program-transformation.org/rdiff/SdfBackup/GeneralizedLR?rev1=1.7&rev2=1.6)
-   [Rev
    6](http://www.program-transformation.org/view/SdfBackup/GeneralizedLR?rev=1.6)
    [(diff 5)](http://www.program-transformation.org/rdiff/SdfBackup/GeneralizedLR?rev1=1.6&rev2=1.5)
-   [Total
    History](http://www.program-transformation.org/rdiff/SdfBackup/GeneralizedLR)

<!-- -->

-   [More
    \...](http://www.program-transformation.org/oops/SdfBackup/GeneralizedLR?template=oopsmore&param1=1.8&param2=1.8)
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
    \...](http://www.program-transformation.org/oops/SdfBackup/GeneralizedLR?template=oopsmore&param1=1.8&param2=1.8)
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
Generalized LR {#generalized-lr .twikiTopicTitle}
==============

::: {.twikiWebTitle}
SDF: Modular Syntax Definition Formalism
:::

[]{#Introduction} Introduction
------------------------------

A parsing algorithm that maintains multiple LR parsing states in
parallel.

From [*Object Oriented Tree Traversal With
JJForester*](../Transform/ObjectOrientedTreeTraversalWithJJForester){.twikiLink}:

*GeneralizedLR parsing removes the restriction to a non-ambiguous
subclass of the context-free grammars, such as the LR(k) class. This
allows a maximally natural expression of the intended syntax; no more
need for \`bending over backwards\' to encode the intended grammar in a
restricted subclass. Furthermore, generalized parsing leads to better
modularity and allows \`as-is\' syntax reuse.*

[]{#Implementations} Implementations
------------------------------------

Implementations of GLR using a separate scanner

-   [ElkHound](../Transform/ElkHound){.twikiLink} is GLR parser
    generator
-   [Bison](http://www.gnu.org/software/bison/bison.html) includes an
    GLR parser.
-   [PyGgy](http://www.lava.net/~newsham/pyggy/) A Python parser
    generator that generates SLR tables for a GLR parsing engine.

Implementations of [Scannerless Generalized
LR](ScannerlessGeneralizedLR){.twikiLink}

-   [SGLR](SGLR){.twikiLink} is a Scannerless Generalized LR parser
-   [DParser](http://dparser.sourceforge.net) is Scannerless Generalized
    LR parser generator.

The maintainers of
[Elkhound](http://www.cs.berkeley.edu/~smcpeak/elkhound/) maintain a
list of implementations as well.\
[]{#TopicEnd}
:::

::: {.twikiTopicInfo .twikiRevInfo .twikiGrayText .twikiMoved}
*Sdf.GeneralizedLR moved from Tools.GeneralizedLR on 30 Jan 2004 - 16:38
by [MartinBravenboer](../Main/MartinBravenboer){.twikiLink}*
:::
:::
:::
:::
