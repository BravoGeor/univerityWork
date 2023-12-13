**Tutorial 3** 


Creating a door with a passcode. This will be my main door that stops the player from going to where they need to go. Clues on the code will be found around the map. 



Setting everything up 

First thing you are going to want to do is create a door and resize it accounting to what you need / to your character's size. Once you're happy with this, create an empty and label it Door. Drag your door object under this and create another empty. You're going to label this Hinge. Move it to where the door will rotate.

I labeled my door as H as I did not want to give it a complicated name.  


Next create a door collider. This will be where the player will walk into that will trigger the passcode to appear. 


Creating the keypad: 

First thing your going to want to do is create an empty and name it canvas. Put this under the door parent. Next create an image and resize it. This will be your base.
Next your going to create a Text. This will later show the player the buttons they have entered and will clear if it is incorrect . Next we are going to create some buttons. And set them as an array. You’ll end up with this: 




Animation:
Every door needs an open animation right? Simple animation in unity is extremely simple. Go into your Timeline and click Create to start a new animation and save the animation as OpenDoor. Hit the red dot to start recording your animation. Go to frame 20 and translate your door open. Your door animation will now be saved in your assets. 





Set up your nodes like this. This is so that when the door open function is called, the door will open. Make sure you untick the loop tickbox
. 
Coding: 

Now we get to coding. Click your Door parent and create a c# code, name this DoorOpen. This code is going to hide the code for the mechanism for a coded door along with opening it. 



We are going to start off by creating all of our variables. 



This calls in our animator. 




This section defines that the code will equal the value to the door code along with setting how long the door code will be. Here, we set it to 4 digits. 

The codeTextValue will be decided later as my  game progresses.


This calls upon when I is pressed, the code panel will pop up.


The segment above tells the code that if the player collides with the collider, that the player is at the door and to follow through the IsAtDoor.



Finally, this last bit tells the code if the player is not near the door, to hide the CodePanel. 


Getting the buttons to work 

Head over to your buttons under DigitNumber and select them all. Scroll on the inspector to ‘on click’ Here You will hit the + and drag the door parent into the None (object). Finally under No function, change this to OpenDoor -> AddDiget(string) 

Last step: Type in the digits you need in the box 

 

Thats it! You now have a functioning door. 


Video used in reference: 
https://youtu.be/dVUIg8A71RE?si=kfJeLU0WJFTJo80j
