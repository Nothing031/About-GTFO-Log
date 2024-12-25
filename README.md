# About-GTFO-Log
## Rundowns
keyword that contains about rundown
: SelectActiveExpedition
* R1 : Local_32
* R2 : Local_33
* R3 : Local_34
* R4 : Local_37
* R5 : Local_38
* R6 : Local_41
* R7 : Local_31
* R8 : Local_35
## States

* rundown selected(contains rundown data) :SelectActiveExpedition
* dropping : GAMESTATEMANAGER CHANGE STATE FROM : Lobby TO: Generating
* Key loading and etc...
* load done : BUILDER : BuildDone
* game start(start of timer) : GAMESTATEMANAGER CHANGE STATE FROM : ReadyToStartLevel TO: InLevel
* game done (failed) : GAMESTATEMANAGER CHANGE STATE FROM : InLevel TO: ExpeditionFail
* game done (abort) : GAMESTATEMANAGER CHANGE STATE FROM : InLevel TO: ExpeditionAbort
* game done (success) : GAMESTATEMANAGER CHANGE STATE FROM : InLevel TO: ExpeditionSuccess

## Keys
#### log
* 06:33:21.393 - <color=purple>CreateKeyItemDistribution, keyItem: PublicName: KEY_WHITE_259 SpawnedItem: KeyItemPickup_Core(Clone)_GateKeyItem:KEY_WHITE_259_terminalKey: KEY_WHITE_259 (KeyItemPickup_Core) placementData: DimensionIndex: Reality LocalIndex: Zone_1 ZonePlacementWeights, Start: 0 Middle: 50000 End: 0</color>
* 06:33:21.394 - <color=#C84800>>>>> CalcAreaWeights START: FindContainerFor PublicName: KEY_WHITE_259 SpawnedItem: KeyItemPickup_Core(Clone)_GateKeyItem:KEY_WHITE_259_terminalKey: KEY_WHITE_259 (KeyItemPickup_Core) --- Zone: ZONE505, AreaCount: 9 half: 4 even: False ZonePlacementWeights, Start: 0 Middle: 50000 End: 0</color>
* 06:33:21.395 - <color=#C84800>>>>> CalcAreaWeights AREA RESULT: AreaIndex: 0 StartMul: 1 MiddleMul: 0 EndMul: 0 --- ZonePlacementWeights, Start: 0 Middle: 50000 End: 0 Total area weight: 1</color>
* 06:33:21.396 - <color=#C84800>>>>> CalcAreaWeights AREA RESULT: AreaIndex: 1 StartMul: 0.75 MiddleMul: 0.25 EndMul: 0 --- ZonePlacementWeights, Start: 0 Middle: 50000 End: 0 Total area weight: 12501</color>
* 06:33:21.397 - <color=#C84800>>>>> CalcAreaWeights AREA RESULT: AreaIndex: 2 StartMul: 0.5 MiddleMul: 0.5 EndMul: 0 --- ZonePlacementWeights, Start: 0 Middle: 50000 End: 0 Total area weight: 25001</color>
* 06:33:21.398 - <color=#C84800>>>>> CalcAreaWeights AREA RESULT: AreaIndex: 3 StartMul: 0.25 MiddleMul: 0.75 EndMul: 0 --- ZonePlacementWeights, Start: 0 Middle: 50000 End: 0 Total area weight: 37501</color>
* 06:33:21.399 - <color=#C84800>>>>> CalcAreaWeights AREA RESULT: AreaIndex: 4 StartMul: 0 MiddleMul: 1 EndMul: 0 --- ZonePlacementWeights, Start: 0 Middle: 50000 End: 0 Total area weight: 50001</color>
* 06:33:21.400 - <color=#C84800>>>>> CalcAreaWeights AREA RESULT: AreaIndex: 5 StartMul: 0 MiddleMul: 0.75 EndMul: 0.25 --- ZonePlacementWeights, Start: 0 Middle: 50000 End: 0 Total area weight: 37501</color>
* 06:33:21.403 - <color=#C84800>>>>> CalcAreaWeights AREA RESULT: AreaIndex: 6 StartMul: 0 MiddleMul: 0.5 EndMul: 0.5 --- ZonePlacementWeights, Start: 0 Middle: 50000 End: 0 Total area weight: 25001</color>
* 06:33:21.405 - <color=#C84800>>>>> CalcAreaWeights AREA RESULT: AreaIndex: 7 StartMul: 0 MiddleMul: 0.25 EndMul: 0.75 --- ZonePlacementWeights, Start: 0 Middle: 50000 End: 0 Total area weight: 12501</color>
* 06:33:21.407 - <color=#C84800>>>>> CalcAreaWeights AREA RESULT: AreaIndex: 8 StartMul: 0 MiddleMul: 0 EndMul: 1 --- ZonePlacementWeights, Start: 0 Middle: 50000 End: 0 Total area weight: 1</color>
* 06:33:21.408 - <color=#C84800>TryGetExistingGenericFunctionDistributionForSession, foundDist in zone: ZONE505 function: ResourceContainerWeak available: 51 randomValue: 0.1441305 ri: 17 had weight: 25001</color>
#### info
* ri : box index (17)
* zone : zone (505)
* publicName : key name (KEY_WHITE_259)
* area : check down below (2 = C)
##### how to get area
* go to the ri line
* check random value(0.1441305)
* go to first "AREA RESULT" line
* get sum of every total area weight
* randomValue * sum = final weight

