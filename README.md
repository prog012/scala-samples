scala-samples
=============

Sometimes we need read some articles, forums, blogs to understand Scala features.
But if we want just remind yourself something we already knew, then is better just look at code sample.
You could easily change it and play with it and see what's going on.

There are samples of Scala code that explains how to use some scala features.

This code is supposed to be isolated as much as possible - like if we wish to explain/remember one feature of Scala then we are not
going to use 5 more extra features for that (which might not be gotten yet by a reader of this code).

Each example has no more than 100 lines of code. Also there is tagging is used in order to show to the reader what feature is involved
for particular example. Like #feature-1 #feature-3.

"Use the course, Luke!" (R)

<h3>HOW TO INSTALL:</h3>

This is <b>SBT project</b>. So you may follow general <a href="http://www.scala-sbt.org/release/docs/index.html" target="_blank">rules</a> about how to open it in your ide or console.

For example To convert project to <b>IntellijIdea</b>:

BEFORE: make sure than in your IDE, here "File->Setting->Plugins->Browse repositories":
 1. "Scala v.0.22.302" (> 83 000 downloads) plugin installed
 2. "SBT v. 1.5.1" (>10 000 downloads)" plugin installed

Those versions that I have right now (4 November 2013)



<ol>
 <li> If you use sbt v 0.13 then make sure you have this directory (in your home directory): <code>'~/.sbt/0.13/plugins'</code> </li>
 <li> in that file <code>'~/.sbt/0.13/plugins/build.sbt'</code> make sure you have content like this: <br />
    <code>addSbtPlugin("com.github.mpeltonen" % "sbt-idea" % "1.5.2")</code>
 </li>


    For more info: <a href="https://github.com/mpeltonen/sbt-idea">sbt-idea plugin</a>
 </ol>

 Then usual steps are:
 <ol>
  <li>cd ~/[your-path]/scala-samples</li>
  <li>sbt</li>
  <li>gen-idea</li>
  <li>Open project in IDE - just open it as usual IntelliJ idea project</li>
</ol>

<h3>How to launch</h3>

Then let's say you want run some file from this project using <b>SBT support</b>.

An an example,
 1. CTRL+N in IDE, type: "ClassWithApplyMethod", go in this file
 2. CTL+G, type "17" (line number), CTRL+SHIFT+F10 (launch the file project, from line number 17)
  - you will see it will start compiling.. (actually now with no SBT support. That's a lame.. I know).
    You may stop it ! Just click red cross on the bottom panel.
 3. In the top toolbar panel, just under menu-panel "Run" & "Tools" you will be able to see "Starter":
   - click on it and go to "Edit Configuration" window
   - There is "Before launch" section:
     - delete "make" from there
     - then click on "+" and add select SBT and select "compile" option
     - click OK to close the "Edit Configuration" window
 4. Now click "Starter" again in the toolbar panel. Now it use SBT for this particular case / class to run.
   (firs time it's going to take some time. But next time - it will compile and launch it much faster)

