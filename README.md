# before you make any questions
don't exepct a reply to any of your questions about how to run this test server. you are on your own. you can find out how to run a minecraft server on google or just google any of the issues/questions you have, or ask chatgpt. this video tutorial should guide you pretty good on how to setup everything:
[![image](https://github.com/user-attachments/assets/a363c04c-9e26-4a41-9d48-0e1c745ce69b)](https://youtu.be/di6s3Q7b_vg)

# this is licensed content
### TL;DR - you are not allowed to make your own monetized server from the setup on this repo
[![image](https://mirrors.creativecommons.org/presskit/icons/cc.svg)](https://mirrors.creativecommons.org/presskit/icons/cc.svg)
[![image](https://mirrors.creativecommons.org/presskit/icons/by.svg)](https://mirrors.creativecommons.org/presskit/icons/by.svg)
[![image](https://mirrors.creativecommons.org/presskit/icons/nc.svg)](https://mirrors.creativecommons.org/presskit/icons/nc.svg)

# how to run the server?
1. first, click on the branch you are looking for (simply, cool, etc) on the branch selector (appears as "main" by default)
2. click on the green button "code" and click "download zip", and extract it (or clone the repo if you know how to do that)
3. make sure the java version specified [here](https://docs.papermc.io/paper/getting-started) is installed on your compute, and is set as your default java version (you can check that by opening a terminal window on your computer and taking a look at what ``java --version`` says)
4. open a terminal window, and do ``cd <your extracted folder location - you can find that by clicking on the address bar of your file explorer and copying it while being on the extracted folder>``, then ``cd server``
5. on the same terminal window, after executing the ``cd``s, run the server with ``java -jar <binary>``, you can check the provided binary name by taking a look at the "server" folder. it will likely be one of these: ``pufferfish.jar``, ``paper.jar``, ``spigot.jar``, ``bukkit.jar``, ``fabric.jar``, ``minecraft-server.jar``
6. make sure to OP yourself so you are able to execute commands by typing ``op <your username>`` once the server finished starting (will display "done")

# how to teleport to an empty world?
run ``/execute in minecraft:otherside run minecraft:tp <your username> 0 65 0``

# how to test farms?
the server won't behave any different than a mostly out-of-the-box paper server (aka, a normal minecraft server but with some dupes and glitches patched). if you want to test if your farm will break, you'll need to stress out the server to see if any of the reactive protections will kick-in. you can do so with any of the stress tests provided by the command ``/stress``. you can find out more information [here](https://www.spigotmc.org/resources/stress.79374/).

# good to know
- worldedit is bundled on the server, you can import schematics by downloading an schematic and placing it on ``/server/plugins/WorldEdit|FastAsyncWorldEdit/schematics``, then do ``//schem load <file name>``, and then ``//schem paste`` while you are on the server
- you can profile the performance of the server with spark easily with ``/tps``, ``/mspt``, and a variety of web panel tools provided on the ``/spark`` command
