# hoppingBunny
THREE.js animation of a bunny hopping through a forest while the seasons change
Final Project Description - Sarah Pardo and Annie Liu
CS 307 SP 21
Happy Hopping Bunny
Creating the scene
Our scene shows a hopping bunny traveling through the seasons in a forest. We drew inspiration from an earlier student project that shows a fox walking through the woods. To get started, we drew some sketches of what a forest scene could look like. Ultimately, we changed the structure of our scene to include four seasons and the ability to continually rotate throug them.

scene sketch
Preliminary sketch of the scene
We created a cylinder with a radius of 100 and divided it into quadrants, one for each season. Then we used texture mapping to create the effect of seasonal woods background on the wall and ground on the base of the cylinder.

scene
Scene with no trees or bushes
Adding static objects
We added trees and bushes using nested, composite objects. We had a deciduous model and a pine model, and mapped different textures to the trees and bushes according to the season quadrant they belonged in. To help hide the transitions in seasons, we added tree trunks between each "season" that mask the edge of each background image.

bushes and trees
Placement of bushes, trees, and trunks from above
closeup of foliage
Closeup of trees and bushes.
Creating the bunny
Before coding our bunny, we sketched out some simple designs with pseudo code to get a sense of what THREE.js geometries we would be able to use.

Bunny sketch
Preliminary sketch of bunny
Our final bunny is based on the code from the teddy bear function in class. We created functions for the head, torso, and limbs. We used Phong material for the body and eyes of the bunny (giving the eyes a high shininess to make them reflective) and basic material for the nose.

closeup of bunny
The bunny up close.
Animating the bunny and changing the camera
We used animation to have our bunny hop in a circle (radius of 30) and simultaneously make the legs rotate while it hops to give the illusion of pushing off the ground. Additionally, we changed the camera position so that it follows the movement of the bunny as it hops around in the circle.

bunny at low point in jump
Bunny at lowest point of bounce.
bunny at high point in jump
Bunny at highest point of bounce. Note the difference in the leg and how the camera view point also changed.
User Interaction and Lighting
We implemented simple controls for user interaction, mainly SPC to stop the animation and "g" to continue it. For lighting, we added an ambient, directional, point, and spot light.
