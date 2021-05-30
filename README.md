# Overview


let's implement the old roll-a-ball-in-maze thingy using C/C++ and OpenGL on windows:

[![the old roll-a-ball-maze-thingy](https://img.youtube.com/vi/dywQZTQZUqA/0.jpg)](http://www.youtube.com/watch?v=dywQZTQZUqA)


Sounds fun? Feel free to tag along.  I'll implement something here every now and then..


Note that my C/C++ is a bit rusty...

Learning links:
 - OpenGL:  https://learnopengl.com/book/book_pdf.pdf
 - Maze Generator: https://github.com/rendertom/Maze-Generator


# Status:

CMakefile things are kinda working . No actual things on screen.


# Tasks:

- Startup
	- [x] setup CMake and git submodules to build C/C++ stuff
- Features
 	-  Draw Scene (using OpenGL primitives)
		- [ ] Box ( A cube with walls on the top side )
		- [ ] Maze ( a collection of walls on the top side of the box )
		- [ ] Ball (a sphere place on the top side of the box)
	- Capture input (in windows using C/C++)
		- [ ] Capture input from arrow keys using Win32 API	
	- Game logic (in C/C++)
		- [ ] Implement tilting of box  (in x and z directions )
		- [ ] collection detection ( Detect when the ball hits the walls).
		- [ ] Level start / stop ( place sphere on start postion. Implement collection detection with stop position).
- Extra stuff
	- [ ] Sounds (rolling sound, hit-the-wall sound).
	- [ ] maze generator (procedural generation)
	- [ ] lighing model (shadows ?)
	- [ ] Build installer (for itch.io )

# How to build


* install Visual Studio 19 
* Install CMake 
* Type the following:
```
	cd Build
	cmake -G "Visual Studio 16" ..
```
* Open the "Kugle.sln" in  Visual Studio
* Mark the "Kugle" project as the startup project for the solution.
	(Right-click Solution, Press "Set startup projects" and "Single Startup
	project")
