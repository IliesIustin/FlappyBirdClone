# FlappyBirdClone
 A Flappy bird clone game build with libGDX libraries 

This game is pretty simple to build . First of all I introduced textures for the background,tubes and two for the bird (one with wings up and the other down).
The render() function switches the two textures of the birds so that to the user it looks like he is flying
Every time the render() is called the velocity is increased with the gravity and it's gonna decrease the the bird Y coordinate by the velocity. For all of this to happen the game state
must be 1 (this means that the player tapped the screen once). Every time the player touches the screen the velocity is decreased with -30
This apps uses 4 pairs of tubes(with a fixed speed) each one positioned at random Y with the same gap between them . Between the pairs there is a set up distance.
Every time that a pair of tubes passes to the left side of the screen is recycled ( by any means is X coordinate is moved to the left) 
What is happening in the backend of this app is simple . The bird is circle(invisible for the player) and the tubes are rectangles (that are also invisible).
So basically the player try to avoid a circle and some pairs of rectangles intersect one with another .  
If the player loses(game state = 2) an end game texture is shown and the game starts again if the screen is tapped again
