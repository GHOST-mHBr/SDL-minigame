# SDL-minigame

head football. The C++ project for BP course of electrical engineering department of Sharif university of technology.

## Installation

at first you should install SDL2, SDL2_gfx, SDL2_image, SDL2_ttf.
in debian based distributions this command will do that:  

```sh
sudo apt install libsdl2*
```

also you will need g++ as compiler. You can install it by runnig this:  

```sh
sudo apt install g++
```

## Building

There are two options for building the project.

* CMake (recommended)
* Build script

<details>

<summary> Building using CMake (recommended)</summary>

You are gonna need CMake. So install it using your favorite package manager. For example under debian systems:

```sh
project-root$ sudo apt install cmake
```

After installing CMake, navigate to the root directory of the project and insert the following command:

```sh
project-root$ cmake . -B build && cd build && make
```

Now, you should be able to run the program placed at the build directory:

```sh
project-root/build$ ./Program
```

</details>


<details>

<summary> Building using the build script </summary>

There is a shell file named make.sh in the project root directory which helps you build the game.
Just try these commands at the project root directory:  

```sh
project-root$ sudo chmod u+x make.sh && ./make.sh
```

To run the program:

```sh
project-root$ ./Program.out
```
</details>

## Playing

After selecting names, characters and ball the game will start.  
there are two characters which are controlled using 'w s a d' and arrow keys.  
also, each character has a special power which is shown below its names (top of the screen).  
the powers can be enabled by pressing 's' or bottom arrow. it is obvious that power bars(below each goal) must be complete.  

you have 90 seconds. if any player scores more than 10 the game will finish!
