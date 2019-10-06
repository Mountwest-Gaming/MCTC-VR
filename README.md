# VR-Classroom


Originally based on room 232, this representation of a Mountwest classroom has so far been equipped (2019) with a small prototype level grey-box. Inside that level is a Player Character that implements an Interface, the walls are seperate Blueprints that also implement the interface. 

Using this technique we can very easily share a function between the classes and have the function perfrom different tasks based on which object is recieving the call.

The Player Blueprint also uses a Capsule trace to fire a single physics query in the direction of the cameras forward vector.

The hit result of this raycast is broken and processed and the information is processed, leading to the firing of an event or nothing.

The walls are broken up into North East West and South.

At the time of writting this they are all seperate classes. The objective is have the studet realize a much more efficient way to move forward is to have all of the walls inherit from a single Wall class that uses the interface, iEvent, and then make children of that class so each wall inherits from a master wall. Now we can program the functionality they all share in one place.

.. in 215 students should have a solid understanding of Class relationships, inhertiance, and interfaces. 

//to be continued
