## Add more sprites

You can add more sprites to your game.

Every sprite needs a unique name, so use your id such as `ellis Bear-walking` or `hull code club Cheesy Puffs`

Every sprite must have the starting script and use your id.

```blocks3
when flag clicked
hide
wait until <(id) = [my id]>
wait until <not<(id) = [my id]>>
hide
stop [other scripts in sprite v]
```

They will also need to `show`{:class="block3looks"} and have the starting position set using `go to x: y:`{:class="block3motion"}

```blocks3
when I receive [my id v]
show
go to x:() y:()
```

**If the sprite needs to stop the player's motion, it needs to be `black` in colour.**

You can add any code you like to your other sprites, underneath a `when I receive`{:class="block3events"} block.

**If you are creating variables, lists, or custom blocks, make sure they have unique names such as `hull code club score`{:class="block3variables"} or `ellis random move`{:class="block3custom"}**

New sprites can be things the player can move on, things the player might have to avoid, things the player might have to collect.

**DO NOT ADD OR CHANGE THE BLOCKS ON THE PLAYER SPRITE**

If a sprite needs to be interacted with, then it could use `say`{:class="block3looks"} blocks so that the player knows what they need to do.

```blocks3
say [collect me] for (1) seconds

say [avoid me] for (1) seconds
```