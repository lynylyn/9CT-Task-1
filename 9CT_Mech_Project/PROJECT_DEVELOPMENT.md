# 9CT Assesment Task 1
### By Evelyn Starling
***

## Requirements Outline
###  Functional Requirements
+  Defining the Purpose
    + I need to create a program for the EV3 MINDSTORMS robot to allow it to to transport a red block and a yellow block to designated poistions while avoiding the other blocks.
+ Identify Key Actions
    + Object Detection: Move forward until an object is detected
        + Use Case: The robot is moving forward and detects an obstacle. The ultrasonic sensor detects an object within 10 cm. The robot stops and turns 45° to avoid the obstacle. The robot avoids the obstacle and continues its path.
    + Colour Check: Check the colour; if it is yellow or red, capture
        + Use Case: The robot is moving forward and detects an obstacle. The colour sensor checks whether the object is yellow or red. If it is, the robot captures the block. The robot succesfully captures the correct colour.
    + Return: The robot returns the box back to the specified area
        + The robot has captured the box. As it moves back to the specified area, it uses the ultrasonic sensor to check for obstacles. If it comes across an obstacle, it turns 45°. The robot succesfully takes the box back home.
+ Test Cases
    + | Test Case | Input     | Expected Output   |
      |---------- |---------- |----------------   |
      |Avoids Obstacle|Ultrasonic sensor detects an object within 10cm|The robot turns 45° to avoid the obstacle|
      |Checks Colour|Colour sensor detects that an obstacle is yellow or red|The robot captures the box|
      |Returns|The box has been captured and 'avoids obstacles' has been performed again|The box is succesfully returned|
### Non-Functional Requirements
As well as completing the above requirements, the robot should react to the ultrasonic sensor's inputs within 2 seconds to prevent it from crashing into an object, complete the task with a moderate level of efficiency (it shouldn't take hours to get the blocks), and accurately skewer the blocks and drag them back to the starting area.
***

## Design
### Pseudocode
+ ACTIVITY 1A
~~~~
BEGIN
INPUT number
IF number % 2 == 0 THEN
    DISPLAY "even number"
ELSE
    DISPLAY "odd number"
ENDIF
END
~~~~
+ ACTIVITY 1B
~~~~
BEGIN
INPUT i
IF i = 1; i <= a; i++ THEN
    f = f*i
ENDIF
PRINT f
END
~~~~
+ ACTIVITY 2A
~~~~
BEGIN
WHILE price != done
    INPUT price
    total = total + price
ENDWHILE
IF total > 100 THEN
    total = total + total * 10%
ENDIF
PRINT total
END
~~~~
+ ACTIVITY 2B
~~~~
BEGIN
INPUT n
FOR i IN n
