xxyy-archetypes
===============
This repo contains some archetype templates for commonly-used kinds of Spigot plugins. Remember to customize the project
name and text in all files.

Compiling
=======
````bash
git clone https://github.com/xxyy/xxyy-archetypes.git
mvn install
````
This installs all archetypes into your local repository.

Usage
=====
To install an archetype, type the following into your favourite shell fork:
````zsh
mvn archetype:generate \
  -DarchetypeGroupId=io.github.xxyy.archetype \
  -DarchetypeArtifactId=<insert what archetype you want here> \
  -DarchetypeVersion=1.0 \
  -DarchetypeRepository=http://repo.nowak-at.net/xxyy-public/
````
You can omit `-DarchetypeRepository` if you installed the archetypes into your local Maven repository by following the
steps detailed in *Compiling*. Maven will prompt you to interactively enter some properties for your project.

If you're using [IntelliJ IDEA](https://intellij.com) (you really should!), you can also create projects from its GUI
at `File -> New Project... -> Maven -> [X] Create from Archetype`. You can add archetypes using the `[Add archetypes...]`
button. If you've already added your archetype, you can easily find it by clicking on any archetype and typing some
characters of the name (`xxyy` normally does the job)

License
=======
Since this project is not particularly good nor complicated or big, it's licensed under the [WTFPL](http://wtfpl.net):
````
        DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                    Version 2, December 2004

 Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>

 Everyone is permitted to copy and distribute verbatim or modified
 copies of this license document, and changing it is allowed as long
 as the name is changed.

            DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

  0. You just DO WHAT THE FUCK YOU WANT TO.
````

spigot-plugin-archetype
-----------------------
A simple Spigot plugin with no additional dependencies, command, listeners or the alike. Includes a rich pom with
a lot of properties which you may need to adjust.

xyc-plugin-archetype
--------------------
A simple Spigot plugin using the XYC API. That API is private and has not been released to the public (yet).

xyc-sql-plugin-archetype
--------------------
A simple Spigot plugin using the XYC SQL API. That API is private and has not been released to the public (yet).

xyc-game-plugin-archetype
--------------------
A simple Spigot plugin using the XYC Games API. That API is private and has not been released to the public (yet).
