## Build
Each top level folder must have its own build folder for CMake to
generate its files in. An example to build and run Part A would
look like the following:

    cd part-a
    mkdir build
    cd build
    cmake ..
    make
    ./part_a

Note: This project assumes that valid installs of GLFW, GLEW, OpenGL,
and CMake exist already within your development environment. If you
use a Mac, I recommend installing these components with Homebrew.
