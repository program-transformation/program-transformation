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
    Page](http://www.program-transformation.org/edit/Stratego/StrategoOptimizer?t=1536825553)
-   [Rename
    Page](http://www.program-transformation.org/rename/Stratego/StrategoOptimizer)
-   [Attach
    File](http://www.program-transformation.org/attach/Stratego/StrategoOptimizer)

<!-- -->

-   [Printable](http://www.program-transformation.org/view/Stratego/StrategoOptimizer?skin=print.pattern)
-   [Wiki
    Source](http://www.program-transformation.org/view/Stratego/StrategoOptimizer?skin=text&raw=on&contenttype=text/plain)

<!-- -->

-   [Rev
    7](http://www.program-transformation.org/view/Stratego/StrategoOptimizer?rev=1.7)
    [(diff 6)](http://www.program-transformation.org/rdiff/Stratego/StrategoOptimizer?rev1=1.7&rev2=1.6)
-   [Rev
    6](http://www.program-transformation.org/view/Stratego/StrategoOptimizer?rev=1.6)
    [(diff 5)](http://www.program-transformation.org/rdiff/Stratego/StrategoOptimizer?rev1=1.6&rev2=1.5)
-   [Rev
    5](http://www.program-transformation.org/view/Stratego/StrategoOptimizer?rev=1.5)
    [(diff 4)](http://www.program-transformation.org/rdiff/Stratego/StrategoOptimizer?rev1=1.5&rev2=1.4)
-   [Total
    History](http://www.program-transformation.org/rdiff/Stratego/StrategoOptimizer)

<!-- -->

-   [More
    \...](http://www.program-transformation.org/oops/Stratego/StrategoOptimizer?template=oopsmore&param1=1.7&param2=1.7)
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
    \...](http://www.program-transformation.org/oops/Stratego/StrategoOptimizer?template=oopsmore&param1=1.7&param2=1.7)
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
Stratego Optimizer {#stratego-optimizer .twikiTopicTitle}
==================

::: {.twikiWebTitle}
Stratego \-- Strategies for Program Transformation
:::

The Stratego Optimizer consists of a number of source-to-source
transformation components that are called by the
[StrategoCompiler](StrategoCompiler){.twikiLink}.

Optimizations that are already implemented

-   [Stratego simplifier](StrategoSimplifier){.twikiLink}
-   [Innermost fusion](InnermostFusion){.twikiLink}
-   [Pattern match compilation](PatternMatchCompilation){.twikiLink}
-   [Strategy inlining](StrategyInlining){.twikiLink}
-   [Dead definition elimination](DeadDefinitionElimination){.twikiLink}
-   [Constant and copy
    propagation](ConstantAndCopyPropagation){.twikiLink}
-   [Bound unbound variable
    analysis](BoundUnboundVariableAnalysis){.twikiLink}
-   [Dead variable elimination](DeadVariableElimination){.twikiLink}
-   [Avoid run time checks on
    variables](AvoidRunTimeChecksOnVariables){.twikiLink}
-   [Build match fusion](BuildMatchFusion){.twikiLink}
-   [Lift definitions to top
    level](LiftDefinitionsToTopLevel){.twikiLink}
-   [Worker wrapper splitting](WorkerWrapperSplitting){.twikiLink}

Ideas for new optimizations

-   [Common subexpression
    elimination](CommonSubexpressionElimination){.twikiLink}
-   [Effects analysis](EffectsAnalysis){.twikiLink}

------------------------------------------------------------------------

[CategoryCompiler](CategoryCompiler){.twikiLink}\
[]{#TopicEnd}
:::

::: {.twikiTopicInfo .twikiRevInfo .twikiGrayText .twikiMoved}
:::
:::
:::
:::
