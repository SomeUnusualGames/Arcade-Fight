# Arcade-Fight

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

Note that the raylib binding ([nelua-raylib](https://github.com/AbdulKalam21/nelua-raylib)) is already included in this repository.

## Build the game

`nelua main.nelua`

By default, the game compiles for the desktop with the keyboard/mouse as the controls.
You can add the following optional parameters in no particular order:

`web`: Replace the main loop with `emscripten_set_main_loop`. You can then compile the game for the web using emscripten. Note that you must [compile raylib for the web](https://github.com/raysan5/raylib/wiki/Working-for-Web-(HTML5)) first.

`desktop|mobile`: Whether to use the keyboard/mouse (`desktop`) or the touchscreen (`mobile`). The former is the default option.

`skip`: Skip the splash screen.