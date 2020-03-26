## Assignment 5 //  CS6310 // Spring 2020 // Team 23
### Rita Borelli, Patrick Carron, Robert Newling, Andy Koh, Maria Rossi

#### Project Modifications
1. Data Persistence [ … ]

2. Modifications to the Space Region: Warp Gates
This modification introduces warp gates into the space region. This novel square state will allow drones to travel through space on a non-contiguous path between pre-defined warp gates. When a drone thrusts to a warp gate square, it transports the drone to the paired warp gate square somewhere else on the board. A scan of the space region will inform the drone of the presence of a warp gate but will include no indication of where the gate spits the drone out. If a drone thrusts through a warp gate, the action will terminate the thrust early at the exit gate (i.e. the drone will not continue the remainder of the thrust magnitude after warping through the gate). This is an enhancement over the current operation, which requires drones to travel through adjacent squares in a linear path. The new feature will allow the drones to skip from an explored corner of the board to a new zone more efficiently and potentially reduce the number of turns to fully explore the space region. The change will require some moderate refactoring to the current codebase, mainly in terms of adding the new type of space square and reworking the logic that the simulation applies to update the space region accordingly. The squares containing warp gates will not have stars and thus will not need to be explored. 

3. Additions of Other Objects: AWACS

4. As an additional note, we propose increasing the maximum size for the space region 
