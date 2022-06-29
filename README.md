# Core.CargoPath
Harmony plugin replacement and enhancement of rustedits core.paths.

# Install:
Place dll within your HarmonyMods folder<br><br>
# Commands: (Requires admin)
/exportcargopath   -   Exports the currently loaded cargopath to SerializedPathList.xml file in servers root.
<br>
/showcargopath  -  Shows the current path, spawnpoints and stop points.
<br>
/egresscargo  -  Triggers all cargoships on the map to start there leave code.
<br>
/bypasscargospawn   -   Bypasses map placed spawn points.<br><br>
# Enhanced Features:
The cargoship will follow created in rustedit.<br>
If you place down prevent building prefabs it will not be able to trigger a egress leave trigger while its with in them.<br>
Showcargopath will show the areas it cant leave with red numbers and spheres.<br>
You also have the prefab event_cargoship.prefab which will add a spawn point that overrides the random spawn.
When placing more than one of this prefab. It will select one of the prefab locations at random.<br>
cargomarker.prefab will create a stop point that the cargoship will pause at along the path.<br><br>
# Config:
As of writing this there is no config file yet. So defaults are locked in place for now<br>
SinkMode = true;   (Cargo ship will sink instead of leave off edge of map).<br>
StopDelay = 60;    (How many seconds it will wait at a stop).<br>
DistanceFromStop = 35; (How close it needs to get to a stop before it trigger).<br>
DespawnDistance = 80; (How far away a place has to be from sunken cargo for it to despawn.)<br><br>
# SinkMode:
When sinkmode is enabled, Instead of leaving off the edge of the map on a egress trigger. It will explode the engine of the cargoship.<br>
10 seconds later it will start to fill with water and sink to the ocean floor.<br>
Once its on the ocean floor it will start to leak radiation to encrouge players to leave the cargoship even when they have diving gear on.<br>
Once all alive players are atleast 80f distance from the cargoship it will despawn it.
