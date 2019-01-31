# Andrew Denman

## C#

### Mods for Rimworld:

Both these mods use a runtime patching library called Harmony. They are hosted on a separate GitHub account for privacy reasons.

#### NightVision: [Steam](https://steamcommunity.com/sharedfiles/filedetails/?id=1464989530&searchtext=) | [Source](https://github.com/AndTheManDrew/NightVision/tree/master/NightVision/Source) | [Youtube review](https://www.youtube.com/watch?v=5lTOfqgUMMo)

Approximately 2000 Steam subscribers.

Extends the light/dark mechanic from the base game. Affects combat, AI, character stats and gear, and in-game events.

- Detects all compatible game objects including other modded content ([Example](https://github.com/AndTheManDrew/NightVision/blob/master/NightVision/Source/ModInit/Init_Hediffs.cs)).
- Customises the results of the game's random character generator ([Link](https://github.com/AndTheManDrew/NightVision/blob/master/NightVision/Source/Incidents/SolarRaid_PawnGenerator.cs)) with xml output for testing ([Link](https://github.com/AndTheManDrew/NightVision/blob/master/NightVision/Source/Testing/DebugFlareRaidPawnGenXml.cs)).
- Dynamically patches methods depending on the users settings choices ([Example](https://github.com/AndTheManDrew/NightVision/blob/master/NightVision/Source/Settings/SettingOption.cs)).



#### SquadUITweaks: [Steam Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=1455382219) | [Source](https://github.com/AndTheManDrew/SquadUITweaks/tree/master/Source)
Approximately 3000 Steam subscribers.

A simple QoL mod. Tweaks part of the game's UI by decorating a base game class with a callback.




## C++

#### Learning Project: [Source](https://github.com/asedenman/cpp_learning_project/tree/master/ProjectEuler/src)

A project for learning C++ by answering problems from projecteuler.net. Includes a win32 GUI.

- A custom window procedure ([Link](https://github.com/asedenman/cpp_learning_project/blob/master/ProjectEuler/src/windows/ProblemWindow.cpp)).
- Using memoisation to cut down problem solving time ([Link](https://github.com/asedenman/cpp_learning_project/blob/master/ProjectEuler/src/problems/Prob15.cpp)).
- Unit tests ([Link](https://github.com/asedenman/cpp_learning_project/blob/master/UnitTests/ProblemTests.cpp)).
