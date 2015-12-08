# Catch Me If You Can
An infinite runner game for iOS and Android

## Author:
* Rishi Kapadia

## Purpose
This is an infinite runner game developed using the Unity 3D game development
platform. The idea behind the game is that you are a secret agent chasing a
shady suspect through various scenes, such as on top of a moving train or
through a crowded street, and you must dodge course obstacles and objects that
the suspect throws at you.

## Implemented Features
* Scene on top of a train, characters are running forward
* Jumping over different cars on the train, player swipes up
* Avoiding railway posts by either jumping or rolling
* Game ends when agent gets hit or falls off train

Possible additional features (after above is implemented):
* Pan camera around both characters to setup scene
* Knives being thrown at the agent from the front, player swipes down to roll /
dodge
* Speed of runners increases as time goes on
* Ability to change characters (both agent and suspect)
* Multiple trains side by side (3-4 paths, must jump between trains to avoid
falling on tracks)
* Collecting items along the way
  * Use to unlock more characters/scenes
* Additional scenes

## Control Flow
* User sees a splash screen
* An animation is presented that circles around the characters to show the
scene (Not implemented yet)
* User sees a menu screen
  * The user's high score
  * Retry button
  * possibly other settings (see additional features above)
* Clicking Retry starts a new game, as described above
* At the end of the game, another screen is shown
  * Game Over message
  * Shows the score of the recently ended game
  * Shows the high score
  * Retry button
  * Menu button

## Implementation
The Unity 3D game development platform was used to create this game.
I used Maya to create all the scene models.
The code will be implemented mainly in C#.

### Maya:
* Creating all meshes (player, 2 train cars, train post, sand background)
* Rigging the player mesh (attaching a skeleton, creating IK controller
  handles)
* Skinning the player mesh (attaching weights from each bone, indicating
  how much each section of the mesh is influenced by each bone)
* Animating the player mesh (very basic animations, due to lack of time)

### Model
* PlayerScript.cs (For physics properties)
* InternalPlayerScript.cs (For animations)
* CameraController.cs (TBD when creating startup scene)
* SuspectController.cs (TBD when creating startup scene)

### View
* GameManager.cs

### Controller
* GameManager.cs
* TrainManager.cs
* SandManager.cs


Note to iOSDecal Staff:
Since the project files are too large to be posted here, please check
the staff email account for the video of the game I created.

