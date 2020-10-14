# NSASecurityGuard

Developed with Unreal Engine 4

Controls:
---
W, A, S, D  - Player movement

J           - Attack

K           - Pickup

ESC         - Pause

space-bar   - regenerate hp(while dead)

Gameplay:
---
The aim of this game is to retain crowd control of the current map. in order to obtain crowd control, the player has to defeat drunk people.
The drunk type will damage all types of people, and if any normal people die, some cc will be lost. The main character cannot be killed,
but he will lose cc and be in a downed state. He then can be revived by pressing the spacebar. 


Features:
---
Custom robust movements -

Best attempt at having 0 acceleration, to create the retro top-down pixel game style.
Created a direction stack so when the user held down another direction while moving, it will change to the new direction.
So, if more than one movement is held down, it will always move to the newly inputted value.
Similarly, when releasing a movement while others are held down, it will set the movement to the next stack element.
Of course, when in any action (except for movements), the current action cannot be canceled while it has finished playing the flipbook. 

Hp and cc (crowd control) system:

All game actors have their own health. When our protagonist has reached 0 health he will end up in the lie-down state and lose some cc as punishment.
When the cc bar has reached full, the game will end with a winning screen and the player can proceed into the next level. On the other hand, if the cc bar reached 0 the player
will lose and will have to play again or quit to the main screen.


Character states - 

The character currently has two states, one being able to move freely and another is lie-down (died). While in lie-down it cannot perform any actions.
The Player will have to spam the spacebar to regen health back to full in order to continue. While the player is dead he cannot perform any actions until he's up again.

Tilemap layers-

The current tilemap has 3 layers which separate to ground, background, and foreground. When a player is at a structure,
the roof will be separated the in foreground thus blocking the character.
While the ground and the background are for collisions and the character should be above them.

To run - install and run the executables.
