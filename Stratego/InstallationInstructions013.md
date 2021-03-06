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
    Page](http://www.program-transformation.org/edit/Stratego/InstallationInstructions013?t=1536825590)
-   [Rename
    Page](http://www.program-transformation.org/rename/Stratego/InstallationInstructions013)
-   [Attach
    File](http://www.program-transformation.org/attach/Stratego/InstallationInstructions013)

<!-- -->

-   [Printable](http://www.program-transformation.org/view/Stratego/InstallationInstructions013?skin=print.pattern)
-   [Wiki
    Source](http://www.program-transformation.org/view/Stratego/InstallationInstructions013?skin=text&raw=on&contenttype=text/plain)

<!-- -->

-   [Rev
    2](http://www.program-transformation.org/view/Stratego/InstallationInstructions013?rev=1.2)
    [(diff 1)](http://www.program-transformation.org/rdiff/Stratego/InstallationInstructions013?rev1=1.2&rev2=1.1)
-   [Rev
    1](http://www.program-transformation.org/view/Stratego/InstallationInstructions013?rev=1.1)
-   [Total
    History](http://www.program-transformation.org/rdiff/Stratego/InstallationInstructions013)

<!-- -->

-   [More
    \...](http://www.program-transformation.org/oops/Stratego/InstallationInstructions013?template=oopsmore&param1=1.2&param2=1.2)
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
    \...](http://www.program-transformation.org/oops/Stratego/InstallationInstructions013?template=oopsmore&param1=1.2&param2=1.2)
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
Stratego/XT 0.13 Installation Instructions {#strategoxt-0.13-installation-instructions .twikiTopicTitle}
==========================================

::: {.twikiWebTitle}
Stratego \-- Strategies for Program Transformation
:::

First of all download the required packages (`.tar.gz`, RPMs or Source
RPMs). You need [aterm](ATermLibrary){.twikiLink} 2.3.1 and
[sdf2-bundle](../Sdf/SdfBundle){.twikiLink} 2.3 The URLs are specified
in the the release page of [Stratego/XT
0.13](StrategoRelease013){.twikiLink}.

[]{#Using_source_tarballs}[]{#_Using_source_tarballs} ![](http://losser.st-lab.cs.uu.nl/~mbravenb/images/src-pkg.png) Using source tarballs
-------------------------------------------------------------------------------------------------------------------------------------------

Use the instructions in this section if you want to install Stratego/XT
using source tarballs (`.tar.gz`). All packages can be installed using
the usual configure, make, make install, so if you are familiar with
installing tarballs there is nothing special about installing
Stratego/XT and its dependencies.

#### []{#Installation_of_aterm_and_sdf2_b} Installation of aterm and sdf2-bundle

The following sequence of commands takes care of building and installing
the [aterm](ATermLibrary){.twikiLink} and the
[sdf2-bundle](Sdf2Bundle){.twikiLink} in `/usr/local`.

    tar zxf aterm-2.3.1.tar.gz
    cd aterm-2.3.1
    ./configure --with-gcc
    make
    make install
    cd ..

    tar zxf sdf2-bundle-2.3.tar.gz
    cd sdf2-bundle-2.3
    ./configure
    make
    make install
    cd ..

Configuring the aterm library `--with-gcc` limits the number of
different aterm libraries that are installed. Just installing the gcc
version makes installation of the aterm library more portable and is
sufficient for StrategoXT.

If you want to install the packages at a different location, you should
specify a \--prefix in the configure command. If you want to install the
packages at two different locations, you must configure the sdf2-bundle
with the location prefix aterm. For example:

    ./configure --prefix=/opt/aterm --with-gcc
    ./configure --prefix=/opt/sdf2-bundle --with-aterm=/opt/aterm

#### []{#Installation_of_StrategoXT} Installation of StrategoXT

Unpack, configure, make and install StrategoXT using the following
commands:

    tar zxf strategoxt-0.13.tar.gz
    cd strategoxt-0.13
    ./configure
    make
    make install

If you want to install StrategoXT at a different prefix, you should
specify a `--prefix`. If you installed the aterm library and the
sdf2-bundle at a different location, you should specify their location
using `--with-aterm` and `--with-sdf`. For example:

    ./configure --prefix=/opt/strategoxt \
      --with-aterm=/opt/aterm --with-sdf=/opt/sdf2-bundle

[]{#Using_source_RPMs}[]{#_Using_source_RPMs} ![](http://losser.st-lab.cs.uu.nl/~mbravenb/images/src-pkg.png) Using source RPMs
-------------------------------------------------------------------------------------------------------------------------------

TODO

[]{#Using_binary_RPMs}[]{#_Using_binary_RPMs} ![](http://losser.st-lab.cs.uu.nl/~mbravenb/images/redhat.png) Using binary RPMs
------------------------------------------------------------------------------------------------------------------------------

Install the RPMs by running the following command in the directory where
you\'ve downloaded the RPMs.

    rpm -i *

Use the upgrade option if you\'ve already installed earlier versions of
RPMs for aterm, strategoxt or the sdf2-bundle.

    rpm -U *

Of course you can also install the RPMs one by one by specifying the
filenames of the RPMs.

[]{#Related_topics} Related topics
----------------------------------

-   Known [Installation troubles](InstallationTrouble){.twikiLink} on
    operating systems.
-   An overview of reported successful
    [configurations](StrategoConfigurations){.twikiLink}
-   [Category installation](CategoryInstallation){.twikiLink} for all
    topics related to the installation of Stratego

------------------------------------------------------------------------

[CategoryInstallation](CategoryInstallation){.twikiLink}

\
[]{#TopicEnd}
:::

::: {.twikiTopicInfo .twikiRevInfo .twikiGrayText .twikiMoved}
:::
:::
:::
:::
