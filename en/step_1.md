## What you will make

A collaborative game, where each person creates a single level of the game.

## Start your level

--- task ---

The starter project is at [rpf.io/patchwork-game](https://rpf.io/patchwork-game){:target="_blank"}

--- /task ---

The project has five sprites.

Click the green flag to start the game.
1. On the first level the green player sprite will fall to the floor. Use the right arrow key (➡️) to move the player sprite to the end of the screen.
2. The next level will start, showing the Scratch cat appear for three seconds.
3. The next level will start. Move the purple player sprite to the end of the screen to start the game again.

The two player sprites and the two floors are for levels 1 and 3. The Scratch Cat sprite is for level 2. The game you submit will start with level 1, then progress to your level, then finish with level 3.

The level created will need a unique identifier. This identifier should be chosen to avoid clashes with other submitted projects.

--- task ---

Replace `my level`{:class="block3variables"} in the `levels`{:class="block3variables"} list, so that your unique identifier is item 2.

![](images/levels_list.png)

--- /task ---

`my level cat` is a sprite that has the scripts you need for your level. Rename this sprite to include your unique identifier.

--- task ---

The scripts on the cat makes sure that the sprite appears at the start of the level and disappears when the level has been completed.

Edit the `wait until`{:class="block3control"} blocks, so that `level`{:class="block3variables"} is compared to your unique identifier.

```blocks3
when i receive [start v]
hide
+ wait until <(level) = [my level]> //change this to your identifier
+ wait until <not<(level) = [my level]>> //change this to your identifier
hide
stop [other scripts in sprite v]
```

--- /task ---

--- task ---

Edit the script that starts your logic, by adding a broadcast that matches your identifier

Change the `say`{:class="block3looks"} block so the cat says something different.

```blocks3
+ when I receive [my level v] //add a broadcast message matching your level name
show
+ say [my easy level] for [3] seconds //add your own message here to test
```

--- /task ---

--- task ---

Click the green flag.

Complete the first level by moving the player sprite to the right of the screen.

Make sure that the Scratch cat still appears and says the text your wrote.

--- /task ---
