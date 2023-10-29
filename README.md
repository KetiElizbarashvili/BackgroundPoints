# BackgroundPoints
Points on background using three.js



live - https://www.linkedin.com/static?_l=en_US 
The code begins by defining an immediately invoked function expression (IIFE) to encapsulate its functionality. Inside this function, it initializes variables for dimensions (width and height), an HTML canvas element (canvas), a 2D rendering context (ctx), an array for points, and an object called target to track mouse position for interaction.

It creates a grid of points on the canvas, where each point has x and y coordinates and stores its original position. The code then establishes connections between each point and its five closest neighbors, forming a network. These points are associated with small circles for rendering.

Event listeners are added for mouse movement, scroll, and window resize to enable user interaction with the animation. The mouseMove function updates the target position based on mouse movements.

The initAnimation function starts the animation loop, which runs continuously to render the points and lines on the canvas. Points' opacity and line colors change based on their distance from the mouse pointer, creating a dynamic visual effect.

Additionally, the shiftPoint function uses TweenLite to animate points' positions, giving them a drifting behavior over time. This creates a subtle but engaging animation effect.

The code also defines a Circle constructor for drawing points, which takes position, radius, and color as parameters.

The drawLines function draws lines between points if they are active, contributing to the connectivity and aesthetics of the animation.

Finally, the getDistance function calculates the squared Euclidean distance between two points. 
