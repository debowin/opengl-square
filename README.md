# SquareGL
![Image](squaregl.png)

### Features -

- **Smooth Translation** - Click the mouse _inside_ the square and drag.
- **Scaling** - Click the mouse near the _edges_ and drag.
- **Rotation** - Click the mouse near the _corners_ and drag.

### Challenges - 
> **Problem** - Setting up OpenGL and SDL to work with my project in CLion on Linux Mint 18.2 Sonya.
>
> **Solution** -
> - First I had to install SDL. OpenGL was already installed on my system. libsdl2-dev wasn't easy to install via apt-get
  due to some broken packages present on my system as opposed to the versions of those packages that it needed.
  I fixed this by using the aptitude package manager to resolve the conflicts.
>
> - Since CLion's project model is based on CMake, I had to figure out a way to use SDL and OpenGL with CMake.
  After some digging online, I was able to figure out how to create the CMakeLists file, setting the linker flags as required and got it working as expected.

### DOWNLOAD [Source Code Zip](http://github.com/debowin/opengl-square/zipball/master/)