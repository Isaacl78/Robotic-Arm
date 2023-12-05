# Robotic-Arm
The process of building the robotic arm was an exciting project, but it turned out to be 
more challenging than we initially expected. The arm consisted of around 40 3D-printed pieces, 
each of which needed to be precisely designed and assembled for the arm to function correctly. 
However, when we began assembling the arm, we quickly realized that many of the pieces did 
not fit together as they should have.
![9fdc0909-1e05-470d-8c06-da361e51889a (1)](https://github.com/Isaacl78/Robotic-Arm/assets/99940722/dc89eadf-6947-424e-a0a1-c960e30716f8)


This issue mainly arose with the screws, ball bearings, and motors, which were often too 
big to fit in most of the holes. We needed to spend considerable time sanding down the pieces 
carefully, making them gradually smaller but not too small as that could cause some parts to fall 
apart. We also had to drill carefully on some of the parts of the arm to expand the holes that 
needed it.
![03666f8c-1787-4e52-9ba5-58935786794c](https://github.com/Isaacl78/Robotic-Arm/assets/99940722/30a36c5a-b360-44a8-af7e-bf079c8ee408)


We coded the robotic arm with Arduino. We had to test each of the six servo motors to 
make it work properly. Assigning the correct degrees to each servo motor (minimum angle and 
maximum angle) is crucial; not only for the functionality of the robot but also to avoid any 
damage that the structure could suffer due to collisions or pressure. To deal with multiple servo 
motors, we used the hcpca9685 servo driver so that we had more free pins in the Arduino Uno 
Board that were used for the stepper motor, and especially the Arduino keypad, which allows us 
to input data to control and command the movement of the robotic arm so that we do not need to 
always connect a laptop (our initial choice) every time we want to move the arm.


We could program the robotic arm using different libraries required for the servo driver 
and the keypad. First, we initialized every part of the system, setting all the correct pins for each 
part and the initial position of each servo. Then, to make the arm move as we want, we included 
a while loop in the void loop; we created a variable to collect the input gotten from the button of 
the keypad that the user presses, and depending on which button it is, a specific part of the 
robotic arm moves, this way we can control every junction separately. Also, when a servo motor 
reaches its minimum or maximum degrees, it can no longer move in the direction that was 
moving, even if the button of the keypad assigned to move it in that direction is pressed multiple 
times. This prevents problems that can be caused when commanding the robot.
![778f1293-ebc4-42b4-869f-fd55a4b9653c](https://github.com/Isaacl78/Robotic-Arm/assets/99940722/369c9f17-7b7b-4343-b754-0832eafd336d)


Despite the challenges, we persevered and eventually assembled the robotic arm 
successfully. It was imperfect, and we knew many of the problems could have been avoided if 
we had taken more time to ensure the pieces fit together before printing them. Nevertheless, we 
were pleased with our final project and the learning experience throughout the semester. 
Looking ahead, there are several ways we can enhance the functionality of the robotic arm. 
Firstly, by implementing kinematics, we could achieve more efficient and accurate control over 
the arm's movements, enabling it to reach specific distances with greater precision. Additionally, 
adding a separate battery and stepper driver to the stepper motor would improve its performance 
and reduce the risk of damage due to voltage fluctuations. Furthermore, modifying the design of 
the base to incorporate rotation capabilities would provide greater flexibility, allowing the arm to 
access a wider range of positions. Another modification we could make is to the wrist of the arm, 
making it adaptable to different types of grippers. This would allow for greater versatility and 
expand the range of applications for the robotic arm. Finally, resolving the issues with Bluetooth 
connectivity would enable us to control the arm from a distance using a remote control or even a 
mobile app, greatly increasing its practicality and convenience. This could also inspire us to 
explore the option of adding wheels to the design, enabling the arm to move and manipulate 
objects in different locations. Overall, these improvements would make our arm an even more 
effective tool for various applications


https://github.com/Isaacl78/Robotic-Arm/assets/99940722/e7c3ec79-6c32-4a13-a76e-048abcb9387b

