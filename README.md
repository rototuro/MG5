# MG5
## Devlog
1. I think NavMesh is better for games where the player does not directly control 
the player character's movement with WASD. Usually, you might see this for colony builders. In fact, a really good
example of this is Black and White 1 and 2, where you only have mouse controls and the system does all the pathfinding
for your character for you. Scripting character movement with physics makes more sense in the inverse case, where
you are actively using WASD to path a character around an environment. Pathfinding in this case is unnecessary
because there is generally a much higher emphasis on exploration and player freedom.
2. It appears the Vector3 distance is compared to a minimum distance to ensure that not every single bird on the map
runs away from the player. I fixed the for loop so all sparrows should get scared by the player, PROVIDED they are
close enough. Originally, it had it such that only the first and second sparrows in the array would be scared,
but I assumed this was the bug I was supposed to fix.

## Open-Source Assets
- [Quirky animal 3D models](https://assetstore.unity.com/packages/3d/characters/animals/quirky-series-free-animals-pack-178235)
- [Mountain fantasy environment models](https://www.fab.com/listings/60487a72-3f20-4bb2-aa78-247ed1582656)