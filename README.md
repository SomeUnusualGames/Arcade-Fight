# Arcade-Fight
Source code for the game Arcade Fight made in Nelua.
Simple top down shooter against a robot boss.

Watch on Youtube (click the image):

[![Watch on Youtube](http://img.youtube.com/vi/YSB4TmimQP4/maxresdefault.jpg)](http://www.youtube.com/watch?v=YSB4TmimQP4 "The making of the game")

# Building instructions

## [Install nelua](https://nelua.io/installing/)

The following version was used:
```
Nelua 0.2.0-dev
Build number: 1528
Git date: 2022-07-21 12:31:19 -0300
Git hash: 112409b9b54468275a4f4700f04e1b03966994bb
Semantic version: 0.2.0-dev.1528+112409b9
```
## [Install raylib v4.0.0](https://github.com/raysan5/raylib/releases/tag/4.0.0)

Look at the [wiki page](https://github.com/raysan5/raylib/wiki#development-platforms) for detailed instructions. 

Using newer versions of raylib is not recommended, it will contain breaking changes.

## Clone this repo.

`git clone https://github.com/SomeUnusualGames/Arcade-Fight.git`

Note that the raylib binding ([nelua-raylib](https://github.com/AbdulKalam21/nelua-raylib)) is already included in this repository.

## Build the game

`nelua main.nelua`

You can add the following optional parameters in no particular order:

- `web`: Replace the main loop with `emscripten_set_main_loop`. You can then compile the game for the web using emscripten. Note that you must [compile raylib for the web](https://github.com/raysan5/raylib/wiki/Working-for-Web-(HTML5)) first.

- `skip`: Skip the splash screen.

- `gc`: Enable the garbage collector.
