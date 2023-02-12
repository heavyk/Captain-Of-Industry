# captain

### bugs (recently noticed)

- copying preferences from retaining wall to another doesn't copy priority
- tutorials panel doesn't exit with right+click away from window
- (unverified) when deconstructing, if there 2 buildings constructing that need 30 cp1 and I'm deconstructing a building with > 60 cp1, the truck will make 2 loads, instead of loading 60 and dropping max to each construction site (then probably leaving the rest in the shipyard)
- (broken pipes save) build the pipe and it'll immediately crash. seems on that slope, it makes invalid pillars placement, but doesn't recognise it until after constructed
- if I unpause cargo boat, it starts to leave, I pause it right afterward and it goes and fetches cargo but without crew ald comes back still paused (it does consume fuel though)
- when the trucks bring parts to build/upgrade a bunch of building/pipes in an area, they don't seem to bring enough parts. I think it's the same problem as the next tree lookup, also where they're simply not looking into a big enough area -- because, unless the rest of the parts need to be delivered across the island (and there are parts available over there), it's always more efficient to carry as many parts to a bunch of locations within an area.

### features (recently noticed)

- ability to set speed of a belt. sometimes I want to reduce the speed of a belt, to limit loopback output.
- put balancers and sorters at altitude > 0
- ability to put pillars above balancers and sorters.
  - in fact, as a performance improvement, it'd be nice to not render pillars where belts are stacked (they already look like they're on top of each other)
- ability to set something "idle" priority (meaning, that only do this if there are no other jobs for some seconds)
- alarm to notify me (or visual way to see) when a building has not been active for some period of time
- on world resources, "load cargo" has an option (checkbox?) to return after loading.
- it'd be cool to have the blueprints folder match the blueprints dir structure in the game as well.. probably not optimised for large amounts of bps, but it's easier for having a diff. maybe a developer mode where the bps are even stored in a text format.

### improvements to existing functionality (recently noticed)

- ability to expand mining areas by clicking and draging them (horizontal and diagonals).
- in the research and recipes panels, when hovering over the machine, it'd be nice to see a popup with the machine's stats (like buildings listed in resarch panel under "unlocks")
- groundwater pump and oil pump can try out a "sliding alert" (like the keep empty/full sliders) to set at what amount it tells me the reserve is low.
- sometimes I want to just make a connector. perhaps, when clicking on the belt/pipe when it shows the connector (this starts the pipe laying), if I click again on the same spot, it'll just put the connector (*screenshot*). workaround is to just copy an existing connector.

### annoyances (recently noticed)

- sometimes it says that the fuel station does not have fuel, when in fact it does (this happens, I think, because the station has committed the fuel to various trucks at once, and even though they haven't picked up the fuel, yet, the station is considered empty)
- sometimes, there is a structure in the way which makes excavators take a really long direction around (*save*)
- sometimes it says the excavator has no fuel when the fuel truck is already on the way.
- I really wish belts would join together (or have some way to do it) when copying and pasting (or extending a belt). workaround right now is to make a connecting belt/pipe at the break and then delete the belt/pipe.

### features (reported)

- it would be really nice to be able to click and drag a priority to a whole block of buildings (just like the upgrade tool does, but to set priorities for blocks of buildings, instead of having to click on each set of factories). maybe a way to do this, is to change the upgrade tool to edit settings (or upgrade) for the group of buildings selected.

- ASAP build: ability to unity build something as soon as unity and material reqirements are available.

- also the ability to partially unity build something sending the hand to get materials acrooss the map easily (also useful in the early game to save diesel)

- priorites panel: it'd be cool to have a panel where priorities can be given names and their priorities reordered by dragging them around. the idea is I can create a list of priorities like "oil", "iron", "steel", etc. and then I can arrange their order.
  - additional options can be set on a per-priority basis like:
    - "allow partial loads"
    - "idle priority" with the ability to customise after how much time of being idle threshold.


### improvements to existing functionality (reported)

- storage alerts are kinda wierd -- it would be easier to just press the alert button (to enable alerts) and then  pull two sliders for minimum and/or maximum alert (like the target fertilization slider)

- in a mess of pipes with many connections, it's difficult to see where it goes. it'd be nice to have a button or something to show the complete path the pipe/belt takes and what resources ports it's connecting to (just like a plain colour line that follows the pipes/belts paths and has an arrow along the path to show direction).
  - an easier implementation is just an arrow on the pipe segment, instead of line for the whole path/network.

- it takes forever to add servers to a data centre. three possible solutions are:
  - hold shift to add 5 at a time
  - "max" button which adds as many as can be added
  - a slider like the buckets/boxes to set how full you want the data centre to be.

### small things (reported)

- when upgrading a world structure, the only way to cancel the upgrade is in the shipyard. also, the "load cargo"  button doesn't exist until I cancel the upgrade in the shipyard (no way to cancel the upgrade in the world). (same thing for "start repairs button" -- also, no way to cancel it)

- when upgrading a building, it puts the green chevrons, but if I pause the upgrade the green chevrons don't turn grey or something to note that it's paused (like the grey upgrade button on botton left).

- I have pickups put on my fuel stations because they carry 20 and are fast. however, even though there are many excavators (with 27 fuel tank) at 7 or less fuel, the pickup does not refuel them until they're empty -- at which time they refill the excavator to ~21 fuel.

- it seems like the fuel trucks should also load up fuel to the shipyard, cargo depots, and potentially fluid storages accepting diesel.

- instead of up and down arrows to reorder recipes, it'd be nicer if there were like two/three horizontal bars showing that the recipe can be dragged up or down to reorder it.

- maybe add dust clouds to when terrain falls down, just for a visual effect.

- when unity building things, it'd be nice to see the resources cost for the upgrade (in addition to the unity cost)

- in the load game dialog, it'd be really nice to show the in-game time in addition to the wall clock time (and potentially some other stats pulled out of save data), so I can tell how far along in the game each save is at (I'm often saving the year and month in the save title to remember).

- console command to remove all terrain designatons that are completely surrounded by blank or at the correct height areas. (leaving only the active ones)

- not sure if it's intentional, but retaining walls looks like it needs tech lab 2, otherwise the research looks like it should be between smart routing and research lab 2 (in screenshot below, see how I researched the retaining walls but I can't research mdepot2 - also, it looks like I have tech lab 2, but I don't).

### bugs (reported)

- floating pipes

- if I am deconstructing a storage of CP2 and it's set to be empty, and then I unity build some belts costing CP2, it'll take the CP2 out of the shipyard before the storage of CP2 (save p- 0.3.4-1)

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
