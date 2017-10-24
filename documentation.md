# MCP73831T LiPo Charger

This board was designed by William Laney as part of the College of William and Mary's physics undergraduate research, 2017. 
Questions or concerns can be directed to William Laney at welaney@email.wm.edu

This is a LiPo battery chargining board based on the  MCP73831T IC. The MCP73831T  is a charging chip for 3.3V single cell lipo batteries. 

The chip is connected to a red LED. The LED is on while the battery is charging and turns off when the battery has completed its charge cycle.

Power enters the through a microUSB port on one side of the board, the LiPo to be charged in plugged into a JPL connector on the bottom of the board. The microUSB port and JPl connector are on oppistie sides of the board to more realistily simulate the set up of the Sharkduino system it is being developed for.

On the silk screen, IN corrosponds to the voltage from the microUSB port. OUT is voltage from the battery. GND is ground

All traces on this board are 0.016" and the vias have 0.034" drill holes. This is more than sufficient to handle the current through the traces. Right angles in the trace are avoid to help ensure data integrity.

Decoupling capacitors were added as near to the chips as possible to minimize noise to the chips. This is detailed in the relevant data sheets.

0805 package size is used for all passive components. This size was selected because I believe it to be a good compromise between size and ease of placement.

On October 5, 2017 six boards were ordered from OSHpark for \$4.90. This corresponds to \$0.81 per board.

## Assembily Information

Assemblie steps:
(please note that these steps represent what I beilive to be the optimal order of operations. They may not be. Addionaly not all boards were assembled in this way as I expermented with the order)

1. Applie solder paste for MCP73831T
2. Applie solder past for passive components
3. Applie solder past for microUSB port
4. Place MCP73831T
5. Place passive components
   * Start with components closest to the board and work inward
6. Place full board into solder reflow oven
7. Wipe down with isopropal alchohal 
8. Hand solder JPL connector onto the bottom of the board
9. Hand solder the through hole portions of the microUSB port
10. Check if board is shorted between GND and IN/OUT

## Notes/Feature Requests

*this information is subject to change with as more boards are assembled*

The microUSB port on the BOM does not match the land pattern on the board

