::: {.fullPage}
::: {.twikiMiddleContainer}
::: {.twikiLeftBar}
::: {.twikiLeftBarContents}
  ----------------------------------------------------------------------------------
  [![](../pub/Stratego/StrategoLogo/StrategoLogoTextlessWhite-100px.png)](WebHome)
  ----------------------------------------------------------------------------------

**[Home](WebHome){.twikiLink}**

-   [Documentation](StrategoDocumentation){.twikiLink}
-   [Language](StrategoLanguage){.twikiLink}
-   [Research Papers](StrategoPublications){.twikiLink}
-   [Applications](StrategoApplication){.twikiLink}

**[Download](StrategoDownload){.twikiLink}**

-   [Continuous build](ContinuousBuild){.twikiLink}
-   [Extensions](AdditionalPackageDownload){.twikiLink}

**[Support](StrategoSupport){.twikiLink}**

-   [Mailing lists](MailingList){.twikiLink}
-   [IRC](irc://irc.freenode.net/#stratego)
-   [Users Days](StrategoUsersDay){.twikiLink}
-   [Bug Reports](http://yellowgrass.org/project/StrategoXT)

**[Developers](StrategoDev){.twikiLink}**

-   [Subversion](https://svn.strategoxt.org/repos/StrategoXT/strategoxt/trunk)
-   [Buildfarm
    results](http://hydra.nixos.org/jobset/strategoxt/strategoxt-release/all)
:::
:::

::: {.twikiMain}
::: {.toolBar}
::: {.flexMenuBar}
::: {.flexMenu onmouseover="return showMenu(event, 100);" onmouseout="return hideMenu(event, 100);"}
Page

::: {#flexMenuContent100 .flexMenuContent}
-   [Edit
    Page](http://www.program-transformation.org/edit/Stratego/ConstantTermCaching?t=1536825558)
-   [Rename
    Page](http://www.program-transformation.org/rename/Stratego/ConstantTermCaching)
-   [Attach
    File](http://www.program-transformation.org/attach/Stratego/ConstantTermCaching)

<!-- -->

-   [Printable](http://www.program-transformation.org/view/Stratego/ConstantTermCaching?skin=print.pattern)
-   [Wiki
    Source](http://www.program-transformation.org/view/Stratego/ConstantTermCaching?skin=text&raw=on&contenttype=text/plain)

<!-- -->

-   [Rev
    2](http://www.program-transformation.org/view/Stratego/ConstantTermCaching?rev=1.2)
    [(diff 1)](http://www.program-transformation.org/rdiff/Stratego/ConstantTermCaching?rev1=1.2&rev2=1.1)
-   [Rev
    1](http://www.program-transformation.org/view/Stratego/ConstantTermCaching?rev=1.1)
-   [Total
    History](http://www.program-transformation.org/rdiff/Stratego/ConstantTermCaching)

<!-- -->

-   [More
    \...](http://www.program-transformation.org/oops/Stratego/ConstantTermCaching?template=oopsmore&param1=1.2&param2=1.2)
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
    \...](http://www.program-transformation.org/oops/Stratego/ConstantTermCaching?template=oopsmore&param1=1.2&param2=1.2)
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
Constant Term Caching {#constant-term-caching .twikiTopicTitle}
=====================

::: {.twikiWebTitle}
Stratego \-- Strategies for Program Transformation
:::

Terms are constructed dynamically, even when they are are constant at
compile time. Constant term caching is a transformation that lifts out
constant terms and constructs them once at program initialization time.

Advantages

-   repeated construction of the same term becomes O(1)

Drawbacks

-   constant terms that would never be constructed dynamically are now
    constructed
-   the order of term construction changes, this may affect strategies
    such as `new`
-   constant terms can no longer be garbage collected

Lifting may done by nested function calls during initialization or by
storing the constant term in a string (either in textual or
[BinaryATermFormat[^?^](http://www.program-transformation.org/edit/Stratego/BinaryATermFormat?topicparent=Stratego.ConstantTermCaching)]{.twikiNewLink
style="background : #FFFFCE;"}) and reading that in at run-time.

\-- [EelcoVisser](../Main/EelcoVisser){.twikiLink} - 09 Dec 2001\

Implemented in [StrategoRelease07](StrategoRelease07){.twikiLink}.
Performance effects should be evaluated.

\-- [EelcoVisser](../Main/EelcoVisser){.twikiLink} - 16 Jan 2002

------------------------------------------------------------------------

[CategoryDone[^?^](http://www.program-transformation.org/edit/Stratego/CategoryDone?topicparent=Stratego.ConstantTermCaching)]{.twikiNewLink
style="background : #FFFFCE;"} \| [ToDo](ToDo){.twikiLink} \|
[StrategoOptimization](StrategoOptimization){.twikiLink}\
[]{#TopicEnd}
:::

::: {.twikiTopicInfo .twikiRevInfo .twikiGrayText .twikiMoved}
:::
:::
:::
:::
