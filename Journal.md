# journal


 
 **10/10/22**
 An issue I am already running across is that GitHub has no autocorrect. This is a big deal to me due to my dyslexia. A way I will go about this problem is by typing in Word first, Then pasting into GitHub. 

 
 **12/10/22** 

 First problem i have ran into is that Directly importing a model in from blender to Unity, There are missing walls. A way I have found to fix this is by researching into the sitation and finding out Unity does not show/render backwards faces. To fix this, i have returned to Bldender and reflipped the faces so that they are facing the right way


Another issue i have ran across in the main roation of the maze, is that, in the spectator, I struggled to identify What way it would rotate in each Axis. After trail and error, I worked out it spins orazontally on the Z axis. This has been noted for future referance. 


****

I ran into several errors in my look code. With these two errors on going, the program will not work 

How I fixed it:
I looked through the code along with a friend. The error was then located and realized. There were some missing capital errors. With these fixed, It now works. 


![1](https://github.com/BravoGeor/univerityWork/assets/146854370/6e16302f-1ca8-4e10-a3b3-7f6d42fa45a9)

**5/12/22**

 It appears I may have missed something from my code. I have spent over half an hour trying to find it but i have narrowed it down to an area.

How I fixed it: 
Turns out as stated, I was missing an {


****
Despite following my example closely, it appears to not be working. Whenever I walk into my ‘Death’ zone, I just walk through it.This is not supposed to happen. What is meant to happen, is that when the player touches it, they move to the respawn translations. 

 I have gone through it a few times and cannot find the issue. I will take another look tomorrow. 


https://github.com/BravoGeor/univerityWork/assets/146854370/0db1b155-d83c-4948-ad66-90729625d21f


How I fixed it: 
After leaving it for a day and taking a relook, I still could not find the error. However, i found the solution to my problem in the comments. Turns out in order for the code to work, I had to turn on an option in the settings. It now works perfectly. I have logged this in my tutorial. 
![55](https://github.com/BravoGeor/univerityWork/assets/146854370/9ba48f2b-28df-476f-a0f2-d08cd9c35cf4)




****
Whenever an object touches the lava, the player respawns. This will not help the game was the palaver will need to throw objects in the lava in order to cross it.


How did I fix this?

Turns out I did not specify what touching the lava made the player respawn. So, to fix this, I have added two extra lines of code that specifies the player. 



