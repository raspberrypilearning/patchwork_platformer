## End your level

You need a condition to end your level.

Your level will end, and the next one will start, when the variable `level change`{:class="block3variables"} is set to `true`.

You might end your level by the player reaching a score.

```blocks3
forever
if <(hull code club score)> [20]> then
set [level change v] to [true]
```

You could end your level when the player touches another sprite

```blocks3
forever
if <touching (Player v) ?> then
set [level change v] to [true]
```

Or choose another way to end the level. Just remember, you **CAN'T CHANGE THE CODE ON THE PLAYER SPRITE**