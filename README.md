# NSASecurityGuard

Developed with Unreal Engine 4

Controls:

W, A, S, D  - Player movement

J           - Attack

K           - Pickup

Spacebar    - Lie-down

While in "lie-down", any action to stand back up.

---
Features:

Custom robust movements -

Best attempt at haveing 0 acceperation, to create the retro top down pixel game style.
Created a direction stack so when the user held down another direction while moving, it will change to the new direction.
So, if more than one movement is held down, it will always move to the newly inputed value.
Similarly, when releasing a movement while others are held down, it will set the movement to the next stack element.
Of course, when in any action (except for movements), the current action cannot be canceld while it has finished playing the flipbook. 


Character states - 

The character currently have two states, one being able to move freely and another is lie-down. While in lie-down it cannot perform any actions.
If another action is pressed while in lie-down, it will assume the user wants to get back up and will change the state recordingly.

Tilemap layers-

The current tilemap has 3 layers which separate to ground, background, and forground. When a player is at a structure,
the roof will be separated the in foreground thus blocking the character.
While the ground and the background are for collisions and the character should be ubove them.

