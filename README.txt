Name: Kaleb Maulding
Date: 2/16/2025

Operating System: Windows 11
Default Browser: Chrome

=========================================================================================

                            Completed Project Requirements:
                                    (read below)

=========================================================================================

1. Your scene should contain at least 3 layers of hierarchy. (3 points)
-----------------------------------------------------------------------
My 2D scene contains 3 layers of hierarchy listed below...

-Global Transformation Layer: this layer handles global transformations for my car
such as the overall transformation along the x and y axis, rotation, and scaling.

-Component Transformation Layer: This layer handles transformations for specific
components that make up the car. Each component (car body, car hood, car top, etc.),
each have their own translation matrix. Additionally the wheels have their own
rotation matrix, while the lights and windows have their own scaling matrix.

-Vertex Layer: This layer defines the geometry for each component such as circles,
rectangles, semi-circles, etc.

------------------------------------------------------------------------
2. Each hierarchy should contain at least one transformation. (3 points)
------------------------------------------------------------------------
My 2D scene has transformations being applied at each layer.

---------------------------------------------------------------------------------------------------------------
3. Each of Translation, Scaling, and Rotation should be correctly implemented and used at least once. (1 point)
---------------------------------------------------------------------------------------------------------------
My 2D scene correctly utilizes translation, scaling, and rotation.

---------------------------------------------------------------------
5. Transformations are bound to user input and interaction. (1 point)
---------------------------------------------------------------------
-w, a, s, and d control the positive and negative x and y movements
of the car. While using 'a' and 'd' to move, the wheels will also
rotate.

-f and b control the negative and positive rotation of the wheels.

-l is used to toggle the lights on the car from off to on.

-u and j control the scale of the car

-r and v control the rotation of the car

---------------------------------------
6. Creativity and aesthetics. (1 point)
---------------------------------------
My scene is a car that can move left to right on the screen, returning on the opposite
side when leaving the screen. This functionality is hard coded and does not work as 
intended when the car is scaled and/or rotated to a non-default size or position. I 
spent some time getting the colors right and moving all of my components to the correct 
places, and added some cool functionality as well.

=========================================================================================

                            Desired Project Interaction:
                                    (read below)

=========================================================================================

-'w' will move the car in the positive y direction, while 's' will move the car in the 
negative y direction.

-'d' will move the car in the positive x direction, while 'a' will move the car in the 
negative x direction.

-'f' will rotate the wheels in the negative direction (backwards), while 'b' will rotate
the wheels in the positive direction (forwards) to simulate a car driving.

-'l' is used to toggle the lights on the car. By default the front is dark yellow and the
back is dark red. When toggled they will turn to bright yellow and bright red, and return 
to their default values when 'l' is pressed again.

-'u' will positively scale the car, while 'j' will negatively scale the car.

-'r' will rotate the car in the positive direction, while 'v' will rotate the car in
the negative direction.

-While the car is in its default state (meaning that it has not been scaled or rotated)
it will appear back on the canvas when moving out of bounds in both x directions, but 
not both y directions.