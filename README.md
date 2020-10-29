# AI in Mario
This repository features a pathfinder AI (A* algorithm) for the 2009 Mario AI Competition. The repository is a clone of [github.com/LHerskind/MarioA_Neural](https://github.com/LHerskind/MarioA_Neural), which is partially authored by me.
The work done is inspired by Robin Baumgarten.

## How it looks like (NOT sped up)
### Difficulty 2
![lvl2](gifs/lvl2.gif)
### Difficulty 15
![lvl15](gifs/lvl15.gif)

## How it works
The red line shown in the gif is the path that the A* algorithm suggests. This path is computed by using an A* algorithm and by using the code in the game engine to predict movement and behaviour of the enemies in the game. The heuristic function returns the distance to the princess at the end of the level. The A* is penalized for losing lives (going from big mario to small mario) and for jumping into gaps. 

## Project setup
The code is guaranteed to be stable on Java SE 8. 
The following libraries are required:
1. [ASM](https://mvnrepository.com/artifact/org.objectweb/asm/3.3.1)
2. [TestNG](https://mvnrepository.com/artifact/org.testng/testng/5.12.1)
3. [JUnit](https://mvnrepository.com/artifact/junit/junit/4.8.2)
4. [JDOM](https://mvnrepository.com/artifact/org.jdom/jdom/1.1)

The main class is *src/ch.idsia/scenarios/Play.java*.
