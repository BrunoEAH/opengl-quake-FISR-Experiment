# opengl-quake

A simple Quake map viewer in OpenGL originally made by Johan Gardhage and further improved by Bruno Hayek.

The main goal for this fork is render the Quake map viewer using the Fast Inverse Square Root and a traditional calculation method. We have further improved the building file so that it also generates a executable for Windows and we also made adaptations to C++20.

![Screenshot](/screenshots/quake.png "quake")

## Prerequisites

To build opengl-quake, you must first install the following tools:

- [SDL 2.0.4](https://www.libsdl.org/download-2.0.php) (or later)
- [GLU](https://en.wikipedia.org/wiki/OpenGL_Utility_Library)
- [Ninja 1.5](https://ninja-build.org/) (or later)
- C++20

### Install dependencies

#### openSUSE

`$ sudo zypper install ninja gcc-c++ libSDL2-devel glu-devel`

#### Ubuntu

`$ sudo apt install ninja-build g++ libsdl2-dev libglu1-mesa-dev`

## Build instructions

To build the quake demo program, run:

`$ ninja`

A `build` directory will be created, containing the demo program.

## Usage

```
Usage: quake [OPTION]...

Options:
 -h, --help         Display this text and exit
 -w, --window       Render in a window
     --fullwindow   Render in a fullscreen window
 -f, --fullscreen   Render in fullscreen
 -c, --showcursor   Show mouse cursor
     --nocursor     Hide mouse cursor
```

## License

Licensed under MIT license. See [LICENSE](LICENSE) for more information.

## Authors

* Johan Gardhage
* Bruno Hayek