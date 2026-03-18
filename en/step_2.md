## Create your level

You can add any sprites you like to the game, or duplicate the cat sprite and change its costume. Rename the sprites so that their name includes your unique level name.

Copy over the scripts from the cat to any new sprites that you add.

Your level can be about anything you choose. Here are the rules that you must follow.

1. You can't use `when flag clicked`{:class="block3events"} blocks.
2. `when I receive my level`{:class="block3events"} is the block that will start your scripts.
3. All variables, lists, or custom blocks you add must be named using your unique level name. e.g. `my_level_name score`{:class="block3variables"}
4. You can not change the code on the sprites included in the starter project. Leave `start player`, `end player`, `start floor` and `end floor` alone.
5. You can not add or edit code on the Stage. You can not add Backdrops. If you want your own background scenery then it will have to be a sprite.
6. If the player needs instructions for your level, they need to be included by having sprites `say`{:class="block3looks"} what needs to be done.
7. Set the starting position of **all** your sprites, using `go to x: y:`{:class="block3motion"} blocks.

Your level needs to end at some point. Maybe the player reaches a goal, answers some questions, achieves a certain score.

The following code is included with the `my level cat`. This will end your level and progress to the next level.

```blocks3
set [level change v] to [true]
hide
stop [this script v]
```

In testing, your sprites might not be visible. You can press **M** on your keyboard to reveal sprites, so long as they have this script on them.

```blocks3
when I receive [edit mode v]
show
```

In testing you might want to manually move to the next level. You can press **N** on your keyboard to set `level change`{:class="block3variables"} to `true` and move to the next level.

--- task ---

Add sprites, variables and code blocks to make your own level.

When you are done you should be able to click the green flag, complete the first level, see your level and complete it, see the end level.

--- /task ---