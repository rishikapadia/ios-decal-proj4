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

## Features
* Scene on top of a train, characters are running forward
* Knives being thrown at the agent from the front, player swipes down to roll /
dodge
* Jumping over different cars on the train, player swipes up
* Avoiding railway posts by either jumping or rolling
* Speed of runners increases as time goes on
* Game ends when agent gets hit or falls off train

Possible additional features (after above is implemented):
* Ability to change characters (both agent and suspect)
* Multiple trains side by side (3-4 paths, must jump between trains to avoid
falling on tracks)
* Collecting items along the way
  * Use to unlock more characters/scenes
* Additional scenes

## Control Flow
* User sees a splash screen
* An animation is presented that circles around the characters to show the
scene
* User sees a menu screen
  * The user's high score
  * New Game button
  * possibly other settings (see additional features above)
* Clicking New Game starts a game, as described above
* At the end of the game, another screen is shown
  * Shows the score of the recently ended game
  * New Game button
  * Menu button

## Implementation
The Unity 3D game development platform will be used to create this game.
I will be using Maya to create the scene models, and possibly free models I can
find online.
The code will be implemented mainly in C#.

### Model
* AgentController.cs
* CameraController.cs
* SceneManager.cs
* SuspectController.cs

### View
* GUIManager.cs

### Controller
* GameEventManager.cs

