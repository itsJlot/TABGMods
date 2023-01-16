# commands (enter in chat):

```py
#set your color
color [r g b a]
#make yourself go rainbow
rainbow
#Set gravity in x y and z directions:
gravity x y z
#Set timescale factor
time (factor)
#Load a scene, this completely breaks the game, but allows looking at some scenes that are usually not available, 0-4 can be loaded.
#dont expect too much from this. Press alt + f4 to exit the game after exploring a scene
sload (scene num)
#launch yourself, leave factor at 0 to launch on spot
launch (launch factor)
# load up the database of all assets in the game and allow spawning them through a filtered list - very experimental
loaddb
# toggle generic spawning UI
sp
#toggle car and item spawning
!
```

## loaddb usage
press a button in the displayed list to spawn that object, which may be visible or not, and may or may not have a collider or other effects to go with it.
Enter a keyword into the textbox at the top left to filter the list of objects.
This is not a well implemented feature, sorry about this, it might get better.

