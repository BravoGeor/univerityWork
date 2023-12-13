LESSON 2: 

Picking up Objects

This tutorial I will be showing you how to pick up objects in unity that are affected by gravity. I will be using this in my game as a way to jump onto platforms. 


First thing your going to want to do is create an empty under camera.  This will serve as your pickup point. Label it as PickupPoint. 



Move this pickup point to where you want your player's hand to be. Mine is at this distance as i am picking up large objects. 

Code:


Create a new script under playerBody and label it as PhysicsPickup 



These first few lines are essential as they are creating the core aspects of what the code requires. They are set to private as I do not want to edit them within unity. It is also calling in the RigidBody. 



This input calls on the code to get the input of E. This means if E is pressed, the code will be triggered to start. 

The next section calls for the object to use gravity; however, if there is no object, the code will end. 

This calls on a raycaster from the player camera to the pickup point to see if there is an object there. 




Finally , this section tells the program that, if an object is detected, to move with the direction of the point with the distance it moves. (the point moves automatically with the camera. 




This is what your final code should look like. 

Assembly: 

Return to unity and create your block(s). I made mine red so that it stands out from the ground. 



Create a new layer and label this as pickup.  Assign it to your object. Make sure to add a rigidbody so the player doesn't walk through it.


Last part, assign everything to the correct places 









That's everything! Have fun throwing blocks around!



Video used in reference:  
(1395) How to Make a Physics Pickup System in Unity in 3 Minutes - YouTube
