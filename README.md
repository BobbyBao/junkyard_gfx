# junkyard_gfx

A Collection of C/C++ libraries for game development

![header](https://user-images.githubusercontent.com/2153610/45614134-c805f980-ba68-11e8-95ab-caba774feb54.jpg)

- [junkyard_gfx](#junkyardgfx)
  - [System](#system)
    - [Base](#base)
    - [Math](#math)
    - [Windowing/Inputs](#windowinginputs)
    - [Threading](#threading)
    - [Sound](#sound)
    - [Networking](#networking)
    - [SIMD](#simd)
  - [Engine Components](#engine-components)
    - [Rendering](#rendering)
    - [UI](#ui)
    - [Scenegraph](#scenegraph)
    - [ECS](#ecs)
    - [Animation](#animation)
    - [Physics](#physics)
    - [Pathfinding](#pathfinding)
    - [Database](#database)
  - [Asset Management](#asset-management)
    - [Meshes/Geometry](#meshesgeometry)
    - [Importers/Exporters](#importersexporters)
    - [Texture Baking/Packing](#texture-bakingpacking)
  - [Misc](#misc)
  
## System
### Base

Lib           | Title
------------- | -------------
[bkaradzic/bx](https://github.com/bkaradzic/bx) | Base library
[septag/sx](https://github.com/septag/sx) | Portable base library for C programmers, tailored for performance and simplicity
[nothings/stb](https://github.com/nothings/stb) | stb single-file public domain libraries for C/C++
[RandyGaul/cute_headers](https://github.com/RandyGaul/cute_headers) | One-file C/C++ libraries with no dependencies, primarily used for games 
[vurtun/mmx](https://github.com/vurtun/mmx) | single header libraries for C/C++ 
[zpl-c/zpl](https://github.com/zpl-c/zpl) | Your C99 Powerkit 

### Math

Lib           | Title
------------- | -------------
[g-truc/glm](https://github.com/g-truc/glm) | OpenGL Mathematics (GLM)
[recp/cglm](https://github.com/recp/cglm) | Optimized OpenGL/Graphics Math (glm) for C
[google/mathfu](https://github.com/google/mathfu) | C++ math library developed primarily for games focused on simplicity and efficiency.
[ferreiradaselva/mathc](https://github.com/ferreiradaselva/mathc) | Pure C math library for 2D and 3D programming
[demianmnave/CML](https://github.com/demianmnave/CML) | The Configurable Math Library http://cmldev.net
[sce_vectormath](https://github.com/erwincoumans/sce_vectormath) | Vector math library
[Imath](https://github.com/openexr/openexr/tree/develop/IlmBase/Imath) | Imath
[Handmade-Math](https://github.com/HandmadeMath/Handmade-Math) | A simple math library for games and computer graphics.
[felselva/mathc](https://github.com/felselva/mathc) | Pure C math library for 2D and 3D programming. 

### Windowing/Inputs

Lib           | Title
------------- | -------------
[SDL](https://github.com/SDL-mirror/SDL) | Simple DirectMedia Layer
[glfw](https://github.com/glfw/glfw) | A multi-platform library
[gainput](https://github.com/jkuhlmann/gainput) | C++ input library for games
[wgois/OIS](https://github.com/wgois/OIS) | Object oriented Input System https://wgois.github.io/OIS/
[ziacko/TinyWindow](https://github.com/ziacko/TinyWindow) | a cross platform (Linux and Windows) OpenGL window library in a single header
[nyorain/ny](https://github.com/nyorain/ny) | Modern C++ cross-platform window abstraction

### Threading

Lib           | Title
------------- | -------------
[rhoot/sc](https://github.com/rhoot/sc) | Cross platform co-routine library exposed through a minimal C API
[deboost.context](https://github.com/septag/deboost.context) | "Deboostified" version of boost.context (coroutines), Plain and simple C API for context switching. Easy build on multiple platforms.
[SergeyMakeev/TaskScheduler](https://github.com/SergeyMakeev/TaskScheduler) | Multithreaded task scheduler experiments
[dougbinks/enkiTS](https://github.com/dougbinks/enkiTS) | C++ and C multithreading task scheduler
[Freeeaky/fiber-job-system](https://github.com/Freeeaky/fiber-job-system) | Multi-Threaded Job System using Fibers
[RichieSams/FiberTaskingLib](https://github.com/RichieSams/FiberTaskingLib) |A library for enabling task-based multi-threading. It allows execution of task graphs with arbitrary dependencies.
[JodiTheTigger/sewing](https://github.com/JodiTheTigger/sewing) | Small C API Multiplatform multithreaded fiber based job system

### Sound

Lib           | Title
------------- | -------------
[openal-soft](https://github.com/kcat/openal-soft) | software implementation of the OpenAL 3D audio API
[soloud](https://github.com/jarikomppa/soloud) | Free, easy, portable audio engine for games
[BareRose/atomix](https://github.com/BareRose/atomix) | Portable, single-file, wait-free atomic sound mixing library utilizing SSE-accelerated mixing

### Networking

Lib           | Title
------------- | -------------
[librg](https://github.com/librg/librg) | Pure C99 game networking library
[bkaradzic/bnet](https://github.com/bkaradzic/bnet#bnet---message-oriented-networking-library) | Message oriented networking library using TCP transport
[zeromq/libzmq](https://github.com/zeromq/libzmq) | ZeroMQ core engine in C++, implements ZMTP/3.1 http://www.zeromq.org
[rxi/dyad](https://github.com/rxi/dyad) | Asynchronous networking for C
[lsalzman/enet](https://github.com/lsalzman/enet) | ENet reliable UDP networking library
[jarikomppa/ipc](https://github.com/jarikomppa/ipc) | Public domain, cross platform, single header inter-process communication primitives. This is a "stb like" public domain header-only C/C++ library that provides inter process communication functionality, released under unlicense.
[ValveSoftware/GameNetworkingSockets](https://github.com/ValveSoftware/GameNetworkingSockets) | Reliable & unreliable messages over UDP. Robust message fragmentation & reassembly. Encryption. 

### SIMD

Lib           | Title
------------- | -------------
[p12tic/libsimdpp](https://github.com/p12tic/libsimdpp) | Portable header-only zero-overhead C++ low level SIMD library
[VcDevel/Vc](https://github.com/VcDevel/Vc) | SIMD Vector Classes for C++


## Engine Components

### Rendering

Lib           | Title
------------- | -------------
[bkaradzic/bgfx](https://github.com/bkaradzic/bgfx) | Cross-platform, graphics API agnostic, "Bring Your Own Engine/Framework" style rendering library.
[DiligentGraphics/DiligentEngine](https://github.com/DiligentGraphics/DiligentEngine) | A modern cross-platform low-level 3D graphics library that supports Direct3D11, Direct3D12, OpenGL/GLES, Vulkan and Metal
[Kode/Kore](https://github.com/Kode/Kore) | Modern low level game library and hardware abstraction
[floooh/sokol](https://github.com/floooh/sokol) | minimal cross-platform standalone C headers
[floooh/oryol](https://github.com/floooh/oryol) | A small, portable and extensible C++ 3D coding framework
[cofenberg/unrimp](https://github.com/cofenberg/unrimp) | Unified renderer implementation ("Un r imp") 
[doitsujin/dxvk](https://github.com/doitsujin/dxvk) | Vulkan-based D3D11 and D3D10 implementation for Linux / Wine 
[pplux/px](https://github.com/pplux/px) | Single header C++ Libraries for Thread Scheduling, Rendering
[google/filament](https://github.com/google/filament) | Filament is a real-time physically based rendering engine for Android, Windows, Linux and macOS
[intel/fastuidraw](https://github.com/intel/fastuidraw) | library that provides a higher performance Canvas interface
[mosra/magnum](https://github.com/mosra/magnum) | Lightweight and modular C++11/C++14 graphics middleware for games and data visualization
[GPUOpen-LibrariesAndSDKs/V-EZ](https://github.com/GPUOpen-LibrariesAndSDKs/V-EZ) | V-EZ is an open source, cross-platform (Windows and Linux) wrapper intended to alleviate the inherent complexity and application responsibility of using the Vulkan API.
[ssloy/tinyrenderer](https://github.com/ssloy/tinyrenderer) | A brief computer graphics / rendering course 
[nicebyte/nicegraf](https://github.com/nicebyte/nicegraf) | An abstraction layer for low-level platform-specific graphics APIs. 

### UI

Lib           | Title
------------- | -------------
[ocornut/imgui](https://github.com/ocornut/imgui) | Dear ImGui: Bloat-free Immediate Mode Graphical User interface for C++ with minimal dependencies
[vurtun/nuklear](https://github.com/vurtun/nuklear) | A single-header ANSI C gui library
[andlabs/libui](https://github.com/andlabs/libui) | Simple and portable (but not inflexible) GUI library in C that uses the native GUI technologies of each platform it supports
[rxi/microui](https://github.com/rxi/microui) | Tiny immediate-mode UI library
[julianeisel/bWidgets](https://github.com/julianeisel/bWidgets) | Basic UI widget toolkit designed for Blender 

### Scenegraph
Lib           | Title
------------- | -------------
[buserror/libc3](https://github.com/buserror/libc3) | Lightweight C Scene Graph Library

### ECS
Lib           | Title
------------- | -------------
[skypjack/entt](https://github.com/skypjack/entt) | A fast and reliable entity-component system (ECS) and much more
[redxdev/ECS](https://github.com/redxdev/ECS) | C++ single-header entity component system library
[alecthomas/entityx](https://github.com/alecthomas/entityx) | EntityX - A fast, type-safe C++ Entity-Component system
[discoloda/Diana](https://github.com/discoloda/Diana) | Entity Component system like Artemis implemented in C 
[SanderMertens/reflecs](https://github.com/SanderMertens/reflecs) | Multithreaded entity component system written in C99 

### Animation
Lib           | Title
------------- | -------------
[guillaumeblanc/ozz-animation](https://github.com/guillaumeblanc/ozz-animation) | Open source c++ skeletal animation library and toolset
[google/motive](https://github.com/google/motive) | A cross-platform, memory efficient, and performant animation system written in C++ http://google.github.io/motive/

### Physics
Lib           | Title
------------- | -------------
[NVIDIAGameWorks/PhysX](https://github.com/NVIDIAGameWorks/PhysX) | NVIDIA PhysX SDK 4
[bulletphysics/bullet3](https://github.com/bulletphysics/bullet3) | Bullet Physics SDK: real-time collision detection and multi-physics simulation for VR, games, visual effects, robotics, machine learning etc.
[MADEAPPS/newton-dynamics](https://github.com/MADEAPPS/newton-dynamics) | Newton Dynamics is an integrated solution for real time simulation of physics environments. http://www.newtondynamics.com
[erincatto/Box2D](https://github.com/erincatto/Box2D) | Box2D is a 2D physics engine for games http://box2d.org
[AvtechScientific/ASL](https://github.com/AvtechScientific/ASL) | Advanced Simulation Library - hardware accelerated multiphysics simulation platform. http://asl.org.il
[gjk.c](https://github.com/kroitor/gjk.c) | Gilbert-Johnson-Keerthi (GJK) collision detection algorithm
[nudge](https://github.com/rasmusbarr/nudge) | A small data-oriented and SIMD-optimized 3D rigid body physics library.
[gpu sph fluids](https://github.com/erwincoumans/fluids_v3) | GPU SPH fluids 
[phyx](https://github.com/zeux/phyx) | 2D physics engine with SoA/SIMD optimizations
[ParticleSolver](https://github.com/ebirenbaum/ParticleSolver) | CPU and GPU implementations of a particle-based physics
[PlayRho](https://github.com/louis-langholtz/PlayRho) | Real-time oriented physics engine and library that's currently best suited for 2D games
[Chipmunk2D](https://github.com/slembcke/Chipmunk2D) | A fast and lightweight 2D game physics library.
[PositionBasedDynamics](https://github.com/InteractiveComputerGraphics/PositionBasedDynamics) | PositionBasedDynamics is a library for the physically-based simulation of rigid bodies, deformable solids and fluids


### Pathfinding
Lib           | Title
------------- | -------------
[jps](https://github.com/fgenesis/jps) | Jump Point Search, public domain, single .h (Super fast pathfinding on uniform grids)
[astar-algorithm-cpp](https://github.com/justinhj/astar-algorithm-cpp) | Implementations of the A* algorithm in C++ and C#
[MicroPather](https://github.com/leethomason/MicroPather) | A* solver (astar or a-star) written in platform independent C++
[recastnavigation](https://github.com/recastnavigation/recastnavigation) | Navigation-mesh Toolset for Games


### Database
Lib           | Title
------------- | -------------
[symisc/unqlite](https://github.com/symisc/unqlite) | An Embedded NoSQL, Transactional Database Engine 

## Asset Management

### Meshes/Geometry

Lib           | Title
------------- | -------------
[libigl](https://github.com/libigl/libigl) | Simple C++ geometry processing library
[MathGeoLib](https://github.com/juj/MathGeoLib) | library for linear algebra and geometry manipulation for computer graphics
[sseculling](https://github.com/nsf/sseculling) | SSE Frustum Culling Demo
[Cullminator9000](https://github.com/Alan-FGR/Cullminator9000) | The fastest culler ever
[SeamAwareDecimater](https://github.com/songrun/SeamAwareDecimater) | Mesh simplification with UV's boundary preserved
[zeux/meshoptimizer](https://github.com/zeux/meshoptimizer) | Mesh optimization library that makes indexed meshes more GPU-friendly

### Importers/Exporters

Lib           | Title
------------- | -------------
[assimp](https://github.com/assimp/assimp) | Official Open Asset Import Library Repository. Loads 40+ 3D file formats into one unified and clean data structure
[nem0/OpenFBX](https://github.com/nem0/OpenFBX) | Lightweight open source FBX importer 
[syoyo/tinyobjloader](https://github.com/syoyo/tinyobjloader) | Tiny but powerful single file wavefront obj loader 
[syoyo/tinygltf](https://github.com/syoyo/tinygltf) | Header only C++ Tiny glTF 2.0 loader. 

### Texture Baking/Packing

Lib           | Title
------------- | -------------
[caosdoar/Fornos](https://github.com/caosdoar/Fornos) | GPU Texture Baking Tool. A fast and simple tool to bake your high-poly mesh details to textures.
[kmkolasinski/AwesomeBump](https://github.com/kmkolasinski/AwesomeBump) | AwesomeBump generate normal, height, specular or ambient occlusion textures from a single image
[dariomanesku/cmft](https://github.com/dariomanesku/cmft) | Cross-platform open-source command-line cubemap filtering tool
[Cheetah-Texture-Packer](https://github.com/scriptum/Cheetah-Texture-Packer) | High efficient and fast 2D bin packing tool
[thekla_atlas](https://github.com/Thekla/thekla_atlas) | Atlas Generation Tool
[libvips](https://github.com/libvips/libvips) | A fast image processing library with low memory needs

## Misc

Lib           | Title
------------- | -------------
[fungos/cr](https://github.com/fungos/cr) | cr.h: A Simple C Hot Reload Header-only Library 
[Manu343726/ctti](https://github.com/Manu343726/ctti)| Compile Time Type Information for C++
[easy_profiler](https://github.com/yse/easy_profiler) | Lightweight profiler library for c++
[spdlog](https://github.com/gabime/spdlog) | Fast C++ logging library.
[color](https://github.com/dmilos/color) | C++ library thats implemets class color
[libmorton](https://github.com/Forceflow/libmorton) | C++ header-only library with methods to efficiently encode/decode Morton codes
[pugixml](https://github.com/zeux/pugixml) | Light-weight, simple and fast XML parser for C++ with XPath support
[opengex](http://opengex.org/) | Scene format specification
[rxi/log.c](https://github.com/rxi/log.c) | A simple logging library implemented in C99













