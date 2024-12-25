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

