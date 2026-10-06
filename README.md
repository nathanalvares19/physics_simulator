# Physics Simulator

A simple implementation of a physics simulator in C++

## Requirements

- Windows 10 / 11
- MSYS2 installed
- Use **MSYS2 MinGW64** shell

---

## Install the compiler and raylib

Open **MSYS2 MinGW64** and run:

```bash
pacman -S --needed mingw-w64-x86_64-gcc mingw-w64-x86_64-raylib
```

Verify:

```bash
ls /mingw64/include/raylib.h
```

---

## Compile and run

In **MSYS2 MinGW64**, change to the project directory (replace the path if needed):

```bash
cd /c/Users/natha/ip/etc/physics_sim
```

Compile from the project root:

```bash
g++ -std=c++17 -I include main.cpp src/window.cpp src/body.cpp src/globals.cpp src/vector2.cpp src/scene.cpp src/state_utils.cpp -o main.exe -lraylib
```

This includes the headers in `include/`, compiles all current source files, and links raylib to create `main.exe`.

Run the simulator from the same shell:

```bash
./main.exe
```

---

## Resources

- [Raylib Examples](https://www.raylib.com/examples.html)

- [Raylib Functions](https://www.raylib.com/cheatsheet/cheatsheet.html)

- [Verlet Integration for Kinematics Simulation](https://www.youtube.com/watch?v=3HjO_RGIjCU)

- [Allen Chou Blog](https://allenchou.net/game-physics-series/)
