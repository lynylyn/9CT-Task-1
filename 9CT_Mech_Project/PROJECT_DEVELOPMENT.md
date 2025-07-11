# 9CT Assessment Task 1
### By Evelyn Starling
***


## Requirements Outline
###  Functional Requirements
+  Defining the Purpose
    + I need to create a program for the EV3 MINDSTORMS robot to allow it to transport a red block and a yellow block to designated positions while avoiding the other blocks.
+ Identify Key Actions
    + Object Detection: Move forward until an object is detected
        + Use Case: The robot is moving forward and detects an obstacle. The ultrasonic sensor detects an object within 10 cm. The robot stops and turns 45° to avoid the obstacle. The robot avoids the obstacle and continues its path.
    + Colour Check: Check the colour; if it is yellow or red, capture
        + Use Case: The robot is moving forward and detects an obstacle. The colour sensor checks whether the object is yellow or red. If it is, the robot captures the block. The robot successfully captures the correct colour.
    + Return: The robot returns the box back to the specified area
        + The robot has captured the box. As it moves back to the specified area, it uses the ultrasonic sensor to check for obstacles. If it comes across an obstacle, it turns 45°. The robot successfully takes the box back home.
+ Test Cases
    + | Test Case | Input     | Expected Output   |
      |---------- |---------- |----------------   |
      |Avoids Obstacle|Ultrasonic sensor detects an object within 10cm|The robot turns 45° to avoid the obstacle|
      |Checks Colour|Colour sensor detects that an obstacle is yellow or red|The robot captures the box|
      |Returns|The box has been captured and 'avoids obstacles' has been performed again|The box is successfully returned|
### Non-Functional Requirements
As well as completing the above requirements, the robot should react to the ultrasonic sensor's inputs within 2 seconds to prevent it from crashing into an object, complete the task with a moderate level of efficiency (it shouldn't take hours to get the blocks), and accurately skewer the blocks and drag them back to the starting area.
***


## Design
### Pseudocode (Warmup Activities)
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
    Set total to total + 1
ENDFOR
PRINT total
~~~~
### Flowcharts (Warmup Activities)
![Flowchart 1A](Flowchart1.png "Flowchart 1A")
![Flowchart 1B](Flowchart2.png "Flowchart 1B")

### Flowcharts (assesment task)
![Mainline](ProjectFlowchart1.png "Mainline")
![Subroutine1](ProjectFlowchart2.png "Subroutine1")
![Subroutine2](ProjectFlowchart3.png "Subroutine2")


## Development and Integration
***
### Testing and Debugging
### Test case - colour detection
Aim: for the robot to follow the black line
- #### Failure Of The Colour Sensor
    Upon starting to test our programs, we realised the colour sensor was not functioning (and unusable). We attempted to make the EV3 follow the black line; which would either cause the robot to collide with obstacles, or leave the mat. We then attempted moving the colour sensor, rebuilding the robot various times, but most of these interfered with the results (e.g, underneath and near the front). After performing many tests and changing as much as we could, we realised that it was unrealistic  to use the colour sensor. In the end, we chose to scrap the colour sensor altogether.


Evaluation: failed, but we were able to move past the step


### Test case - avoiding obstacles
Aim: for the robot to accurately move along the mat, avoiding the blue and green boxes
- #### Hard Code/Measuring
   After the sensors had failed through all our tests, we made the decision to hard code the EV3. Although it wasn't the most efficient in the program, it was functional, which was our main priority. However, hard coding the robot was still tricky; the measurements were always slightly off and we spent quite a while trying to get angles and distances correct.


Evaluation: tedious, but successful


### Test case - capturing boxes
Aim: for the robot to successfully collect the red and yellow blocks while avoiding the blue and green
- #### Developing The First Grabber
    While Emma and I worked on hard coding the robot to move around the mat, Juliet was chosen to create the grabber; as we decided against just piercing the blocks. This grabber was the first of three designs. Design #1 featured a one sided grabber intended to catch the block and funnel it toward the centre. It was shaped similarly to half a hexagon.


- #### Developing The Second Grabber
    Similarly to Design #1, the funnel was on one side of the robot. However, this grabber stuck outwards more, and was straighter. This ensured that the second block would stay within the grabber whilst the EV3 turned. While this grabber was generally successful,  it was mistakenly disassembled at the end of the lesson.




- #### Developing The Final Grabber
    The 'stag beetle' was our third and final grabber design. It had two, long lego technic blocks reaching out ahead of it, giving it its name. This grabber was long enough, grabbed the blocks, and held them in place.


Evaluation: although it took a few lessons, our final design was very functional


### Test case - beginning the program
Aim: to begin the problem by pressing the button on the touch sensor
- #### Implementing The Touch Sensor
    As our code required the use of two sensors, using the touch sensor was vital. While Emma and I were hard coding yet again, Juliet worked on programming the touch sensor. This, thankfully, worked immediately!


Evaluation: worked perfectly on the first try


## Peer Evaluation
***
### Juliet

*When rating 1-5 with 1 being lacklustre effort and 5 being outstanding effort, how much effort do you feel this group member put into this project?*: 5/5

*Explain the reason for this score in detail:* Juliet gave a great amount of effort to this task, performing extremely well in all areas while she stayed on task throughout the whole project and ensured that we did the same.

*When rating 1-5 with 1 being not at all and 5 being an exceptional amount, how much did this team member contribute to the team's efforts throughout this project?*: 5/5

*Explain the reason for this score in detail:* Juliet was an incredibly hard working group member throughout the course of the task, mainly working on assembly of the robot but also offering ideas and solutions when it came to debugging and creating our program. She involved herself in all areas of the task without going off track.

*When rating 1-5 with 1 being not well at all and 5 being exceptionally well, how well do you think this team member performed throughout all stages of the project?:* 5/5

*Explain the reason for this score in detail*: Juliet performed extremely well throughout, being an incredible debugger with unique solutions. Her design for the grabber and work on coding the sensors were vital for our final test.

### Emma
*When rating 1-5 with 1 being lacklustre effort and 5 being outstanding effort, how much effort do you feel this group member put into this project?*: 5/5

*Explain the reason for this score in detail:* Emma was an astounding group member, doing a majority of the code and a lot of the tedious work throughout. She was very helpful to both me and Juliet, helping with whatever we were doing whilst completing what she was tasked to do.

*When rating 1-5 with 1 being not at all and 5 being an exceptional amount, how much did this team member contribute to the team's efforts throughout this project?*: 5/5

*Explain the reason for this score in detail:* Emma is a very talented programmer, and contributed most of the code for the project. She was great at problem solving when it came to getting the angles and distances right with hard coding.

*When rating 1-5 with 1 being not well at all and 5 being exceptionally well, how well do you think this team member performed throughout all stages of the project?* 5/5

*Explain the reason for this score in detail:* Emma did great both independently and when we were all working on the same thing at once, being the backbone of our team. She did exceptionally in the coding aspect and helped with everything else as well.

### Altogether: 4/5
*When rating 1-5 with 1 being entirely non-functional and 5 being completely functional, how effective was the team's final test case?*: Although our final was successful, we were unfortunately unable to properly incorporate two sensors (due to the ultrasonic sensor not working). The coding could have been more efficient but it worked and we were able to complete it without being hurt by time restraints.

## Final Evaluation
***
*Evaluate your INDIVIDUAL Final Test in Relation to Functional Criteria*: Did not meet the functional requirements due to the sensors not working. Also, was unable to perfect my individual final test due to time constraints.

*Evaluate your INDIVIDUAL Final Test in Relation to Non-Functional Criteria*: Similarly to above, did not meet the non-functional requirements as we focused on the group's final test.

*Evaluate your GROUP'S Final Performance in Relation to the Identified Need*: The EV3 performed very well according to the identified need; it successfully 

Evaluate your Project in Relation to Project Management

Evaluate your Project in Relation to Team Collaboration

Justify Future Improvements you could make to your Final Product