# Computer_Graphics
CTU Computer Graphics Course F1 Project


Project description
This project is an interactive OpenGL racing scene inspired by an F1 track environment. The scene features a procedurally generated oval track with kerbs, grass borders, and a clearly marked start / finish area. A drivable player car is rendered using an external 3D model (OBJ loaded via Assimp) and shaded using Phong lighting for a more realistic appearance. The track also includes texture-based decals and sponsor branding using a texture atlas, alongside additional props such as animated banners to enhance depth and scale.

Multiple camera modes are implemented to support different gameplay and viewing perspectives, including an bird's eye view , orbit view, free camera, and a car-follow camera. Camera transitions are designed to feel smooth between modes, and mouse-look is supported for both free and follow camera control. A HUD is displayed to provide driving feedback such as speed and boost status, rendered unlit so it remains readable regardless of scene lighting and fog.

Beyond the player vehicle, two NPC cars are rendered and continuously drive around the track along a never-ending Catmull-Rom spline path. Their motion can be paused and resumed using the N key, allowing the scene to shift between an active racing environment and a static showcase for viewing.

User interaction is central to the project. The player can drive and steer using standard controls, and a boost mechanic is available via left click, granting a short 3-second burst of speed followed by a 5-second cooldown while the boost bar replenishes. The scene also includes an interactive cone obstacle on the track: in the bird's eye view (1), free camera view (3), and car camera view (4), the user can pick up, drag, and drop the cone using left click. In the same camera modes, the NPC cars can also be frozen and unfrozen with left click, adding an extra layer of interactivity beyond driving.

The environment supports lighting and atmosphere controls for variety and presentation. The city/track scene includes realistic lighting, simple fog effects, and a “dark mode” style setup where headlights can be toggled on and off for a more dramatic, spooky look. As a quality-of-life feature, the player can also toggle the car’s colour styling (blue vs. blue/red livery) using the V key.

Control keys
Driving

W : Accelerate / move forward
S : Brake / reverse
A : Steer left
D : Steer right
Camera Modes

1 : Camera Mode 1 - Bird's Eye View
2 : Camera Mode 2 - Orbit View
3 : Camera mode 3 - Free Camera View With Mouse-Look
4 : Camera mode 4 - Car Chase View
Camera Controls

Mouse Movement : Rotate View
↑ ↓ ← → Keys : Move Camera Around In Free Camera
Q : Ascend Camera In Free Camera
E : Descend Camera In Free Camera
B : Toggle Cursor
+ / - : Zoom In/Out
Other Controls

Right Click : Interact with Cone/NPC Cars (in Camera Modes 1, 3, 4)
Left Click : Boost Car Speed
F : Adjust Fog Level
H : Toggle Headlights On/Off
N : Pause/Resume NPC Cars
V : Toggle Player Car Colour Style
M: Toggle Light/Dark Modes
P : Toggle shading model (Phong per-fragment ↔ Phong per-vertex)
C : Reset Car positions to the track start
