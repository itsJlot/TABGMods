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

#Load a scene, player will be spawned in any picked scene. 0-10 are available, but may break things, you may need to alt + f4
# there is also a freecam now, except for scene 4 and 8, this should allow exploring scenes 0-10, but not getting back, at the moment, sadly. 
# This freecam activates when there is no player object in the scene
sload (scene num)

#launch yourself, leave factor at 0 to launch on spot
launch (launch factor)

# load up the database of all assets in the game and allow spawning them through a filtered list - very experimental
loaddb

# load the database, but only load either asset with visuals, or with colliders. This makes it easier to find interesting assets.
loadtype (mesh/colliders/rigidbody)

# makes any gunshot fired enter the name of the hit object into the search bar of the asset spawning system, to make identifying them easy.
# also allows getting parent, or root name, toggles if no argument given
  - `parent` to get the name of the parent object of the thing hit
  - `root` to get the name of the root object of the thing hit
namegun (mode)

# makes any gunshot fired destroy anything it hits, toggles off and on
delgun

# toggle generic spawning UI
sp

# to dual-wield anything
onehanded 

# to delete an object in the scene by exact name
del (name)

# to set the maps waterlevel to an arbitrary value. E.g. scene 5 has a high water-level, and a map below
waterlevel (level) 

# to teleport to a coordinate 
tp (x y z)

#toggle car and item spawning
!
```

## loaddb usage
press a button in the displayed list to spawn that object, which may be visible or not, and may or may not have a collider or other effects to go with it.
Enter a keyword into the textbox at the top left to filter the list of objects.
This is not a well implemented feature, sorry about this, it might get better.

# Freecam

The freecam will activate when there is not a valid player with a camera in the scene, which allows exploring different maps

