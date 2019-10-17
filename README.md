# VR-Classroom

-------------------------------------



Originally based on room 232, this representation of a Mountwest classroom has so far been equipped (2019) with a small prototype level grey-box. Inside that level is a Player Character that implements an Interface, the walls are separate Blueprints that also implement the interface.

This is a multilayered lesson. the player character is a class, that inherits from character, character inherits from pawn, inherits from Actor. It's typically thought that you can only possess a Pawn, however, you can also possess an Actor. (Bonus points for how)

Using an interface we can very easily share a function between the classes and have the function perform different tasks based on which object is receiving the call.

The Player Blueprint also uses a Capsule trace to fire a single physics query in the direction of the cameras forward vector.

The hit result of this raycast is broken and processed and the information is processed, leading to the firing of an event or nothing.

The walls are broken up into North East West and South.

At the time of writing this, they are all separate classes. The objective is to have the student realize a much more efficient way to move forward is to have all of the walls inherit from a single Wall class that uses the interface, iEvent, and then make children of that class so each wall inherits from a master wall. Now we can program the functionality they all share in one place.

.. in 215 students should have a solid understanding of Class relationships, inheritance, and interfaces.

-------------------------------------

#Team - 2019

Lead Designer: Seth

Event Programmer: Megan

Player Programmer: Devon

AI Programmer: Hunter

3D Art: Austin

Sound: Gage

VFX: Seth

Design: 

Programming: 

Textures: 


//to be continued
-------------------------------------


#Links


Link to Oculus Fork of the Unreal Engine
https://github.com/Oculus-VR/UnrealEngine/tree/4.23

Design Doc
https://docs.google.com/document/d/1scwpX6WGKFBIi6jMBgyRhl1P3glBQNoceW_3mz-5HT4/edit?usp=sharing


