---
layout: guides
navbar: Guides
title: Java and Eclipse Setup
key: 1
---

<style>
img {
  max-width: 100%;
  height: auto;

  background-color: whitesmoke;
  border-radius: 4px;
  padding: 0.25ex;
}
</style>

This guide will walkthrough the steps necessary to install the latest versions of Java and Eclipse on your local system.

## Install Java 13

You need to make sure you have the latest version of Java **Standard** Edition (SE) **Development** Kit **13** (JDK 13) installed on your system. When downloading, keep in mind:

  - Do NOT download Java 8 or Java 11. We will be using Java 13 in class. There are some differences between Java 8, Java 11, and Java 13, and the lecture code may not compile on your system.

  - Do NOT download Java Enterprise Edition (EE). We will be using the Standard Edition (SE) in class. Java EE is used to create enterprise applications.

  - Do NOT download just the Java Runtime Environment (JRE). The Java Development Kit (JDK) includes the JRE, which is necessary to run Java code. The JDK also includes the Java compiler, which we will need in class.

To install the Java SE 13 JDK, go to:

<https://www.oracle.com/technetwork/java/javase/downloads/index.html>

Click the "JDK Download" button for Java SE 13, accept the license agreement, and download the appropriate file for your system. Run the installer and follow the prompts.

Once done, open a terminal window and verify the version using `java -version` and `javac -version`. The output will be similar to:

```shell
% java -version
java version "13.0.2" 2020-01-14
Java(TM) SE Runtime Environment (build 13.0.2+8)
Java HotSpot(TM) 64-Bit Server VM (build 13.0.2+8, mixed mode, sharing)
% javac -version
javac 13.0.2
```

Note that `%` above indicates the command prompt, and the lines below that are the output.

<i class="fas fa-info-circle"></i>
Java [removed auto-update capability](https://www.oracle.com/technetwork/java/javase/11-relnote-issues-5012449.html#Important_Changes) for Windows and MacOS systems. You will need to manually check when new versions of Java 13 are released.
{: .notification .is-size-7 }

## Install Eclipse

![About Eclipse]({{ "/images/abouteclipse.png" | relative_url }}){: style="width: calc(1070px * 0.5);"}

You need to make sure you have the latest **Eclipse IDE for Java Developers** package for **Eclipse 2019-12**. The direct download link is:

<https://www.eclipse.org/downloads/packages/release/2019-12/r/eclipse-ide-java-developers>

Do NOT download the IDE for Java EE Developers, as we are using Java SE in class. There are installers available for Windows, Mac OSX, and Linux. Once downloaded, double-click the installer.

<i class="fas fa-info-circle"></i>
Mac Users: I recommend you move the Eclipse.app file into your "Applications" folder for easy access.
{: .notification .is-size-7 }

## Setup Folders (Optional)

I recommend you create a `CS 212` (or `cs212`) folder, and within it create these subfolders:

  - `Workspace`: This will be the folder for your Eclipse workspace.

  - `Repositories`: This will be the folder for your GitHub repositories that will be used for homework and project submission (and Eclipse).

    You can configure Eclipse to always save your CS 212 code in this folder in the "Team » Git" settings:

    ![Git Settings]({{ "/images/config-team-git-default.png" | relative_url }}){: style="width: calc(1572px * 0.4);"}  

  - `Libraries`: This will be the folder for your user libraries that will be installed in Eclipse. This folder will start empty, but will grow throughout the semester.

Eclipse does not behave well when you combine or nest the `Workspace` and `Repositories` folders. Keep these separate!

## Configure Eclipse

Eclipse is a free, powerful, open-source, and configurable IDE. I recommend you spend some time configuring Eclipse to meet your needs. For example:

  - Change the fonts used in the editor ([reference](https://help.eclipse.org/2019-12/topic/org.eclipse.platform.doc.user/tasks/tasks-20.htm)). You can find several options on [Google Fonts](https://fonts.google.com/?category=Monospace). My favorites are [Source Code Pro Light](https://fonts.google.com/specimen/Source+Code+Pro), [Roboto Mono Light](https://fonts.google.com/specimen/Roboto+Mono), [Anonymous Pro](https://fonts.google.com/specimen/Anonymous+Pro), and [Incosolata](https://fonts.google.com/specimen/Inconsolata). There are many fans of the customizable [Input](http://input.fontbureau.com/) font as well.

    ![Colors and Fonts]({{ "/images/eclipse-colors-and-fonts.png" | relative_url }}){: style="width: calc(824px * 0.5);"}

  - Change your save actions ([reference](https://help.eclipse.org/2019-12/topic/org.eclipse.jdt.doc.user/reference/preferences/java/editor/ref-preferences-save-actions.htm)). I usually remove unused imports and fix indentation at least.

      ![Save Actions]({{ "/images/eclipse-additional-save-actions.png" | relative_url }}){: style="width: calc(895px * 0.5);"}

  - Customize the autocomplete code templates ([reference](https://help.eclipse.org/2019-12/topic/org.eclipse.jdt.doc.user/reference/preferences/java/codestyle/ref-preferences-code-templates.htm), [examples](https://stackoverflow.com/questions/1028858/useful-eclipse-java-code-templates)). I usually create one for `printf` myself. You can download the templates I use and import them into your Eclipse workspace:

      <script src="https://gist.github.com/sjengle/32b18311714dc62124cb2154339288b2.js"></script>

  - Change the layout and add [different views](https://help.eclipse.org/2019-12/topic/org.eclipse.platform.doc.user/tasks/tasks-3.htm). I usually add the Tasks view, which shows me all of my `TODO` comments. I also prefer to add the Git views to my Java perspective rather than switching to the Git perspective.

  - Change the code formatter ([reference](https://help.eclipse.org/2019-12/topic/org.eclipse.jdt.doc.user/reference/preferences/java/codestyle/ref-preferences-formatter.htm)). You can set the brace style, where newlines and spaces are used, and fix how Eclipse formats try-with-resources code blocks.

    ![Java Code Formatter]({{ "/images/eclipse-java-code-formatter.png" | relative_url }}){: style="width: calc(1242px * 0.5);"}


    I will be using the [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html) to format the code in class. If you also want to use this code style, you can [download the Eclipse settings](https://github.com/google/styleguide/blob/gh-pages/eclipse-java-google-style.xml) and import them.

The official guides for Eclipse are located at:

<https://help.eclipse.org/2019-12/index.jsp>

Keep in mind that Eclipse is under active development, and [bugs happen](https://bugs.eclipse.org/bugs/).

<i class="fas fa-info-circle"></i>
Try to <a href="https://help.eclipse.org/2019-12/topic/org.eclipse.platform.doc.user/tasks/tasks-47.htm">close projects in Eclipse</a> when you are no longer working on them. This can improve performance.
{: .notification .is-size-7 }
