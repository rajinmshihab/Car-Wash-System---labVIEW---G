# Car-Wash-System---labVIEW---G

Car Wash Operating Rules

Only one purchase selection can be made at a time. The car wash should not accept a second purchase selection while the car wash is in operation.
Not all cycles are performed for each wash. The more expensive wash performs more cycles. The list of cycles performed are:
Cycles performed for the Deluxe Wash: 1 – 2 – 3 – 4 – 5
Cycles performed for the Economy Wash: 2 – 3 – 4
Each cycle is initiated by a switch. If the vehicle rolls off of the switch, the wash immediately pauses and illuminates an indication to the driver to re-position the vehicle. The amount of time that expires while the car is out of position should not count against the wash time.
Underbody Wash Cycle: The spray heads for this wash are located near the entrance of the car wash. The underbody spray heads are fixed in position, and require the vehicle to slowly drive over them to wash the underbody of the vehicle. The Underbody Wash is activated under the following conditions:
The Deluxe Wash has been purchased.
The car wash is in the Underbody Wash cycle.
Under Body Wash Position Switch is closed (proximity switch).
This cycle of the wash should last for 10 seconds. Upon completion of this cycle the controller should signal moving to the next cycle by activating the Vehicle Out of Position LED.
Main Wash Cycle: Main Wash Position Switch verifies the vehicle is in the correct location for the wash cycles (cycles 2, 3 and 4) to operate. Each cycle should last for 5 seconds. If the vehicle rolls off of the Main Wash Position Switch, the wash immediately pauses and illuminates an indication to the driver to re-position the vehicle. The amount of time that expires while the car is out of position should not count against the wash time. The wash resumes after the vehicle is properly positioned. Upon completion of this cycle the controller should signal moving to the next cycle by activating the Vehicle Out of Position LED.
Air Dry Cycle: The air drier is a set of fixed position blowers located near the exit of the car wash. They require the vehicle to drive slowly out of the car wash through the air stream to dry the vehicle. The Air Dry Cycle activates on the following conditions:
The deluxe wash has been purchased
The car wash has reached the Air Dry cycle
Air Dry Position Switch is closed (proximity switch)
If the vehicle rolls off of the Air Dry Position Switch, the wash immediately pauses and illuminates an indication to the driver to re-position the vehicle. The amount of time that expires while the car is out of position should not count against the Air Dry time. The wash resumes after the vehicle is properly positioned. This cycle of the wash should last for 10 seconds. Upon completion of this cycle the controller should allow the next vehicle in line to select another wash.
The Car Wash must respond to the STOP Boolean and Vehicle Position Switches within 100mS. The STOP Boolean aborts the operation of the VI.
