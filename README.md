# prenis

.obj viewer based on OpenGL

# How to use

Add obj\\default.obj to main executable or use
`prenis.exe obj\whatever.obj`

# Controls

Arrows - move camera\
F1 - reset camera\
F2 - change light\
F3 - change diffuse\
F4 - auto camera\
F5 - blinking background\
F6 - blinking object light

# Using

OpenGL\
Tiny obj loader\
stb_image  

# Linux support

First install deps and toolchain:

    # apt install libglu1-mesa-dev freeglut3-dev libglew-dev gcc

To build, run:

    $ g++ prenis/main.cpp -lGLEW -lGL -lGLU -lglut

# OpenBSD support

First install deps and toolchain:

    # pkg_add llvm freeglut glew

To build, run:

    $ clang++ prenis/main.cpp `pkg-config --libs --cflags freeglut gl glew`

# macOS support

First install deps and toolchain:

    $ brew install llvm glew

To build, run:

    $ clang++ -Wno-deprecated-declarations -std=c++17 prenis/main.cpp -L/System/Library/Frameworks -framework GLUT -framework OpenGL -lGLEW

# Screenshots

![Screenshot1](https://i.imgur.com/Lew0tgp.png)
![Screenshot2](https://i.imgur.com/jMHpvEp.png)
![Screenshot3](https://i.imgur.com/ooBo7zu.png)
![Screenshot4](https://i.imgur.com/C5kXOZo.png)
![Screenshot5](https://nekopon.pl/syf/preniskrowanalinuxHOW.png)
