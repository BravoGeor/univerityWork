Tutorial 1 
 Character movement 


Basic setup: 

First thing you would want to do is create an empty. Here you will store all your first person objects such as player mesh and camera. You are going to label this empty as Player. 

Next you'll need to add into the Player a Character controller. This will create a boundary box along with a collider that is fitted to the mesh we will import later. Make sure you set the height to 2 and the radius to 0.5 so that it wraps around the mesh.

Right click the Player and create an object that serves as a placeholder. I will be using a capsule as that's my preference and is the most human-like simple object. The boundary box will automatically follow the player's geometry. 


Make sure you remove the collider it automatically added as, as mentioned previously, we already have a collider aka the character controller. 

Camera 

Locate the world start up camera and drag it into the player empty. Now that this is grouped together, When the empty moves, so will the camera. To make this a first person camera, drag it into your Capsule so that it's positioned where the head would be. Make sure a little gap is left so that the player wont clip into ceilings. 

![1](https://github.com/BravoGeor/univerityWork/assets/146854370/c94dce7f-25ad-4ef8-91fa-423c82fda5a0)

Coding 

Code 1: 
Looking around code

Create a new script on the camera named MouseLook. Make sure this variable stays consistent or you may have problems later. 

Create these two floats as demonstrated in the photo. These will grab the information on the mouse's location. By x the mouse sensitivity, it'll ensure it'll move by how much we want it too. By x by the time too, it'll automatically update to follow the framerate. 

For the ability to control the mouse speed add the following 
Make sure you set it as a public float so that you can change the sensitivity within unity without needing to open the code to change it manually. 







The highlighted area is inputting the mouse values and x by the inputted mouse sensitivity along with the frame count. This comes into play on controlling the camera. 



This code clamps the amount that the player can turn their head up and down. We need this so that the player cannot look all the way behind them and break the character's neck. 



Finally this part will allow the x of your mouse control where you look.

This is what your final code will look like. 


Code 2: character movements. 
This code is responsible for checking the ground on whether the player is in the air, jumping and general movements. 



Create a new script and label it PlayerMovement

First off, you want to create all the floats you'll need. Remember to set them in public if you want to change these later in unity. 
 

What each class does is self explanatory. 


These are specific to the ground checking that the players model will be doing and creating the isGrounded call. 


This section is continuously checking to see if the character is grounded and if they sre not, to add more speed to the falling depending on the gravity. 



This final section creates the movement and jump call. Luckily for us, the jump call is already embedded into unity and is as simple as calling it. 









Your final code should look like this: 

Setting up ground check:
 
First thing you're going to want to do is create an empty under PlayerBody. This empty will serve as your ground check. Locate your ground check in the unity world and move it to the bottom of your character. Assembly:


Here's the fun part! Putting together all the code so that it works. First thing you're going to want to do is create a character controller for your Playerbody components. This will create a collider. 
 
You are going to set your tag to the player and drag your character controller into the controller dropdown along with groundcheck into the ground check dropdown. 

Make sure to go to the ground plane and set that too Ground tag. 













Go to your Players Camera and drag in your mouse look script. Then finally pull in your PlayerBody. 






That's everything! Make sure you test through your code and adjust things to better suit your game and gravity 

Video in reference: 
https://youtu.be/_QajrabyTJc?si=RqJviEGvVL4UXKFS
