# captain

### small things

- when upgrading a world structure, the only way to cancel the upgrade is in the shipyard, and also the "load cargo" button doesn't exist until I cancel it in the shipyard. (same thing for "start repairs button" -- no way to cancel it)

- when upgrading a building, it puts the green chevrons, but if I pause the upgrade the green chevrons don't turn grey or something to note that it's paused (like the grey upgrade button on botton left).

- when unity building things, it'd be nice to see the resources cost for the upgrade (in addition to the unity cost)

- in the load screen, it'd be really nice to show the in-game time in addition to the wall clock time, so I can tell how far along in the game each save is at.

### bugs

- if I am deconstructing a storage of CP2 and it's set to be empty, and then I unity build some belts costing CP2, it'll take the CP2 out of the shipyard before the storage of CP2 (save 0.3.4-1)

- if a belt or pipe is connected but not built, the building on 'auto' will not receive truck imports (unconfirmed in latest version)

- mine tower dialog disappears if dragging mouse into UI
  - pause the game
  - select a mine tower
  - click 'edit area'
  - drag a box to any size, but let go of the mouse button over the 'paused' box or anywhere on the top bar
  - neither the mine area is set or the mine tower dialog returns to view (it eats the mouse event)
  - same thing also happens if I right click or press esc (not sure if this is intentional or not)

- unintentional pausing of transports under construction:
  - build a pipe
  - unity build the pipe (it turns blue)
  - before the first pipe can build, build a second pipe that connects to the first pipe anywhere.
  - when the second pipe connects to the pipe in the process of being built, it gets paused (pipe turns white)
  - look at the first pipe, it still has all of its CP, so all I have to do is unpause it

- floating pipes:


## features

### priorites panel

it'd be cool to have a panel where priorities can be given names and reordered if necessary. the idea is I can create a list of priorities like "oil", "iron", "steel", etc. and then I can arrange their order by dragging them around. additional options can be set on a per-priority basis like "allow partial loads".
