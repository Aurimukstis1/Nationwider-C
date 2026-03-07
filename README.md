# Nationwider C++
Rewritten Nationwider tool in C++, using SDL3 as a graphics lib

With additional SDL3_image library.
With additional Dear ImGui library.

Integrates **Amazon AWS S3** for savefile sharing between Nationwide hosts and players.  
>[!NOTE]
>Will most likely create several different modules to use with different file hosting providers, such as: Hetzner.*

The philosophy here is of a very niche game style called a "Nationwide", where players interact/roleplay as select nations and a host manages the world, changing borders, moving icons, etc.
If you are unfamiliar with the genre, it will be a tiny bit uncomfortable to get used to the program's intended use. All in all, it is a map editing program with placeable icons.

---
Building:
```
cmake -B build
```

```
cmake --build build
```

`SDL3.dll` and `SDL3_image.dll` are required for the executable.

---
<img width="1576" height="1189" alt="nationwidercppdiagram- excalidraw" src="https://github.com/user-attachments/assets/2d30f41d-24e0-48c2-91c1-62876261c3ae" />

Using `std::deque` to efficiently store any amount of layers (lower or upper type).
