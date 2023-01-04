_Modifica el proyecto de RobotGuard para hacer que el NPC vuelva a la última poisición donde vio al jugador antes de huir. Debe volver después de que su salud se haya recuperado por encima de 40._

---

Se ha creado un nuevo árbol llamado "GoToLastKnownPositionOfPlayer" al que se le han nodos condicionantes para que su workflow sea el siguiente: mientras su salud no esté por debajo de 40, no esté en peligro, y además el estado de huida esté activado, se mueva hacia donde se vio por última vez al jugador. Para ello, se crearon varias tasks como "SetTargetDestinationToLastKnownPositionOfPlayer", "SetFleeStatus", y "IsFleeingFromPlayer". El resto de árboles han sido modificados para implementar el comportamiento correspondiente a la huida. 

![](/gif.gif)

A new tree was created called "GoToLastKnownPositionOfPlayer" with conditioning nodes so that its workflow is as follows: as long as its health is not below 40, it is not in danger, and also its fleeing status is true, then move to where the player was last seen. For this, several tasks were created, such as "SetTargetDestinationToLastKnownPositionOfPlayer", "SetFleeStatus", and "IsFleeingFromPlayer". The rest of the trees have been modified to implement the fleeing behaviour.
