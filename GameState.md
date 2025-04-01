# GameState
#### progress state of game
* rundown selected :SelectActiveExpedition
* dropping : GAMESTATEMANAGER CHANGE STATE FROM : Lobby TO: Generating
* game start(start of timer) : GAMESTATEMANAGER CHANGE STATE FROM : ReadyToStartLevel TO: InLevel
* game done (failed)         : GAMESTATEMANAGER CHANGE STATE FROM : InLevel TO: ExpeditionFail
* game done (abort)          : GAMESTATEMANAGER CHANGE STATE FROM : InLevel TO: ExpeditionAbort
* game done (success)        : GAMESTATEMANAGER CHANGE STATE FROM : InLevel TO: ExpeditionSuccess

