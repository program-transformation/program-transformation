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
    Page](http://www.program-transformation.org/edit/Stratego/IfThen?t=1536825587)
-   [Rename
    Page](http://www.program-transformation.org/rename/Stratego/IfThen)
-   [Attach
    File](http://www.program-transformation.org/attach/Stratego/IfThen)

<!-- -->

-   [Printable](http://www.program-transformation.org/view/Stratego/IfThen?skin=print.pattern)
-   [Wiki
    Source](http://www.program-transformation.org/view/Stratego/IfThen?skin=text&raw=on&contenttype=text/plain)

<!-- -->

-   [Rev
    2](http://www.program-transformation.org/view/Stratego/IfThen?rev=1.2)
    [(diff 1)](http://www.program-transformation.org/rdiff/Stratego/IfThen?rev1=1.2&rev2=1.1)
-   [Rev
    1](http://www.program-transformation.org/view/Stratego/IfThen?rev=1.1)
-   [Total
    History](http://www.program-transformation.org/rdiff/Stratego/IfThen)

<!-- -->

-   [More
    \...](http://www.program-transformation.org/oops/Stratego/IfThen?template=oopsmore&param1=1.2&param2=1.2)
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
    \...](http://www.program-transformation.org/oops/Stratego/IfThen?template=oopsmore&param1=1.2&param2=1.2)
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
If Then {#if-then .twikiTopicTitle}
=======

::: {.twikiWebTitle}
Stratego \-- Strategies for Program Transformation
:::

[]{#Syntax} Syntax
------------------

    "if" Strategy "then" Strategy "end" -> Strategy

[]{#Description} Description
----------------------------

The strategy

    if s1 then s2 end

applies `s2` if `s1` succeeds. The result of `s1` is ignored. That is,
if the condition

    <s1> t

succeeds, then the result of

    <if s1 then s2 end> t

is

    <s2> t

On the other hand, if the condition fails, then the result is `t`.

[]{#Formatting} Formatting
--------------------------

The if-then construct is usually formatted in the following way:

    if s1 then
      s2
    end

[]{#Implementation} Implementation
----------------------------------

The if-then construct is sugar for a guarded left-choice. The strategy

    if s1 then s2 end

translates into

    where(s1) < s2 + id

\
[]{#TopicEnd}
:::

::: {.twikiTopicInfo .twikiRevInfo .twikiGrayText .twikiMoved}
:::
:::
:::
:::
