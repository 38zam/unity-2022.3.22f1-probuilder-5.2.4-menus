# Unity Window — ProBuilder (Text Mode)

This file indexes the structural hierarchy and active states of the standalone ProBuilder Window when rendered in Text Mode within Unity 2022.3.22f1 and ProBuilder 5.2.4.

---

## 🛠️ ProBuilder Window Hierarchy

* 🟠 **Create Shape**
    * **Shape Palette (Icons)**:
        * 1. **Sprite**:
            * **Shape Properties (New Shape)**:
                * **Shape**: Sprite (Dropdown: Sprite, Plane, Cone, Sphere, Door, Prism, Cube, Cylinder, Stairs, Torus, Arch, Pipe)
                * **Pivot**: [Center, First Corner]
                * **Size**: X, Y, Z
        * 2. **Plane**:
            * **Shape Properties (New Shape)**:
                * **Shape**: Plane (Dropdown: Sprite, Plane, Cone, Sphere, Door, Prism, Cube, Cylinder, Stairs, Torus, Arch, Pipe)
                * **Pivot**: [Center, First Corner]
                * **Size**: X, Y, Z
            * **Plane Settings**:
                * **Height Cuts**: Integer input
                * **Width Cuts**: Integer input
        * 3. **Cone**:
            * **Shape Properties (New Shape)**:
                * **Shape**: Cone (Dropdown: Sprite, Plane, Cone, Sphere, Door, Prism, Cube, Cylinder, Stairs, Torus, Arch, Pipe)
                * **Pivot**: [Center, First Corner]
                * **Size**: X, Y, Z
            * **Cone Settings**:
                * **Sides Count**: Slider / Integer input
                * **Smooth**: Checkbox
        * 4. **Sphere**:
            * **Shape Properties (New Shape)**:
                * **Shape**: Sphere (Dropdown: Sprite, Plane, Cone, Sphere, Door, Prism, Cube, Cylinder, Stairs, Torus, Arch, Pipe)
                * **Pivot**: [Center, First Corner]
                * **Size**: X, Y, Z
            * **Sphere Settings**:
                * **Subdivisions**: Slider / Integer input
                * **Smooth**: Checkbox
        * 5. **Door**:
            * **Shape Properties (New Shape)**:
                * **Shape**: Door (Dropdown: Sprite, Plane, Cone, Sphere, Door, Prism, Cube, Cylinder, Stairs, Torus, Arch, Pipe)
                * **Pivot**: [Center, First Corner]
                * **Size**: X, Y, Z
            * **Door Settings**:
                * **Pediment Height**: Float input
                * **Side Width**: Float input
        * 6. **Prism**:
            * **Shape Properties (New Shape)**:
                * **Shape**: Prism (Dropdown: Sprite, Plane, Cone, Sphere, Door, Prism, Cube, Cylinder, Stairs, Torus, Arch, Pipe)
                * **Pivot**: [Center, First Corner]
                * **Size**: X, Y, Z
            * *No unique settings.*
        * 7. **Cube**:
            * **Shape Properties (New Shape)**:
                * **Shape**: Cube (Dropdown: Sprite, Plane, Cone, Sphere, Door, Prism, Cube, Cylinder, Stairs, Torus, Arch, Pipe)
                * **Pivot**: [Center, First Corner]
                * **Size**: X, Y, Z
            * *No unique settings.*
        * 8. **Cylinder**:
            * **Shape Properties (New Shape)**:
                * **Shape**: Cylinder (Dropdown: Sprite, Plane, Cone, Sphere, Door, Prism, Cube, Cylinder, Stairs, Torus, Arch, Pipe)
                * **Pivot**: [Center, First Corner]
                * **Size**: X, Y, Z
            * **Cylinder Settings**:
                * **Sides Count**: Slider / Integer input
                * **Height Cuts**: Integer input
                * **Smooth**: Checkbox
        * 9. **Stairs**:
            * **Shape Properties (New Shape)**:
                * **Shape**: Stairs (Dropdown: Sprite, Plane, Cone, Sphere, Door, Prism, Cube, Cylinder, Stairs, Torus, Arch, Pipe)
                * **Pivot**: [Center, First Corner]
                * **Size**: X, Y, Z
            * **Stairs Settings**:
                * **Steps Generation**: Dropdown
                * **Steps Count**: Slider / Integer input
                * **Circumference**: Slider input
                * **Inner Radius**: Float/Integer input
                * **Sides**: Checkbox
        * 10. **Torus**:
            * **Shape Properties (New Shape)**:
                * **Shape**: Torus (Dropdown: Sprite, Plane, Cone, Sphere, Door, Prism, Cube, Cylinder, Stairs, Torus, Arch, Pipe)
                * **Pivot**: [Center, First Corner]
                * **Size**: X, Y, Z
            * **Torus Settings**:
                * **Tube Radius**: Float input
                * **Rows**: Slider / Integer input
                * **Columns**: Slider / Integer input
                * **Horizontal Circumference**: Slider / Integer input
                * **Vertical Circumference**: Slider / Integer input
                * **Smooth**: Checkbox
        * 11. **Arch**:
            * **Shape Properties (New Shape)**:
                * **Shape**: Arch (Dropdown: Sprite, Plane, Cone, Sphere, Door, Prism, Cube, Cylinder, Stairs, Torus, Arch, Pipe)
                * **Pivot**: [Center, First Corner]
                * **Size**: X, Y, Z
            * **Arch Settings**:
                * **Thickness**: Float input
                * **Sides Count**: Slider / Integer input
                * **Arch Circumference**: Slider / Integer input
                * **End Caps**: Checkbox
                * **Smooth**: Checkbox
        * 12. **Pipe**:
            * **Shape Properties (New Shape)**:
                * **Shape**: Pipe (Dropdown: Sprite, Plane, Cone, Sphere, Door, Prism, Cube, Cylinder, Stairs, Torus, Arch, Pipe)
                * **Pivot**: [Center, First Corner]
                * **Size**: X, Y, Z
            * **Pipe Settings**:
                * **Thickness**: Float input
                * **Sides Count**: Slider / Integer input
                * **Height Cuts**: Slider / Integer input
                * **Smooth**: Checkbox
    * **Note**: Click and drag in Scene view to place/scale. SHIFT+click to duplicate last settings.


* 🟠 **New Poly Shape**
    * **Behavior Note**: Clicking this tool immediately instantiates a new GameObject named `PolyShape` in the Hierarchy and activates the editing mode in the Scene view.
    * **Scene View Overlay (Poly Shape Tool)**:
        * ℹ️ *Click To Add Points. Press 'Enter' or 'Space' to Set Height*
        * **Extrusion**: Numerical text input field (Default: `0`)
        * **Flip Normals**: Checkbox toggle (Default: Unchecked)
    * **Inspector Components (For PolyShape GameObject)**:
        * 1. **GameObject Header**:
            * **Name**: `PolyShape`
            * **Static**: Checkbox (Default: Unchecked)
            * **Tag**: `Untagged`
            * **Layer**: `Default`
        * 2. **Transform**:
            * **Position**: X, Y, Z
            * **Rotation**: X, Y, Z
            * **Scale**: X, Y, Z
        * 3. **ProBuilder MeshFilter**:
            * **Button**: `Open ProBuilder`
            * ℹ️ *Mesh property is driven by the ProBuilder component.*
            * **Mesh**: Asset field reference (e.g., `pb_Mesh-6526`)
            * **Object Size (read only)**: X, Y, Z (Default: `0, 0, 0` during editing)
            * **Lightmap Static**: Checkbox toggle (Default: Unchecked)
            * ℹ️ *Warning Icon: To enable generation of lightmap UVs for this Mesh, please enable the 'Lightmap Static' property.*
        * 4. **Poly Shape (Script)**:
            * ℹ️ *Click To Add Points. Press 'Enter' or 'Space' to Set Height*
            * **Extrusion**: Numerical text input field (Mirrors the Scene View Overlay)
            * **Flip Normals**: Checkbox toggle (Mirrors the Scene View Overlay)
        * 5. **Mesh Renderer**:
            * **Materials**: Size array field (Default: `1`)
                * **Element 0**: Material asset reference (Default: `ProBuilderDefault`)
            * ⚠️ *Warning Icon: This renderer has more materials than the Mesh has submeshes. Multiple materials will be applied to the same submesh, which costs performance. Consider using multiple shader passes.*
            * **Lighting**:
                * **Cast Shadows**: Dropdown (Default: `On`)
                * **Receive Shadows**: Checkbox toggle (Default: Checked)
                * **Contribute Global Illumination**: Checkbox toggle (Default: Unchecked)
                * **Receive Global Illumination**: Dropdown (Default: `Light Probes` - Greyed out)
            * **Probes**:
                * **Light Probes**: Dropdown (Default: `Blend Probes`)
                * **Reflection Probes**: Dropdown (Default: `Blend Probes`)
                * **Anchor Override**: Asset field reference (Default: `None (Transform)`)
            * **Additional Settings**:
                * **Motion Vectors**: Dropdown (Default: `Per Object Motion`)
                * **Dynamic Occlusion**: Checkbox toggle (Default: Checked)
        * 6. **Mesh Collider**:
            * **Convex**: Checkbox toggle (Default: Unchecked)
            * **Is Trigger**: Checkbox toggle (Default: Unchecked)
            * **Provides Contacts**: Checkbox toggle (Default: Unchecked)
            * **Cooking Options**: Dropdown (Default: `Everything`)
            * **Material**: Asset field reference (Default: `None (Physic Material)`)
            * **Mesh**: Asset field reference (Default: `None (Mesh)`)
            * **Layer Overrides**:
                * **Layer Override Priority**: Integer input field (Default: `0`)
                * **Include Layers**: Dropdown (Default: `Nothing`)
                * **Exclude Layers**: Dropdown (Default: `Nothing`)

* 🟠 **Smoothing**
    * **Behavior Note**: Clicking this tool opens the standalone `Smooth Group Editor` window. The top bar contains three toggleable tab buttons (`Settings`, `Preview`, `Normals`) that can be turned ON/OFF independently. Multiple tabs can be active simultaneously, stacking their respective settings sections in the panel.
    * **Window Central State**:
        * ℹ️ *Select a ProBuilder Mesh* (Displayed when no valid ProBuilder geometry is active)
    * **Tab Toggles & Options**:
        * 1. **Settings** `[Toggleable Button]`
            * **Preview Opacity**: Horizontal slider accompanied by a numerical text input field (Default: `0.5`)
            * **Preview Dither**: Checkbox toggle (Default: Unchecked)
        * 2. **Preview** `[Toggleable Button]`
            * *No unique settings panel displayed inside the window.*
        * 3. **Normals** `[Toggleable Button]`
            * **Size/Length Slider**: A horizontal slider is exposed directly on the right side of the tab bar header to control normal lines visualization.

* 🟠 **Material Editor**
    * **Quick Material**:
        * **Material Slot**: Object field reference (Default: `None (Material)`)
        * **Apply (Ctrl+Shift+Click)**: Button `[Always Enabled]`
        * **Match Selection**: Button `[Disabled — Greyed out]`
        * **Texture Preview Box**: Displays `None (Texture)` to the right of the buttons.
    * **Material Palette**:
        * **Palette Selection**: Dropdown menu. Clicking it opens a context menu with:
            * `✓ Default Material Palette` (Active selection)
            * `New Material Palette...`
        * **Palette Profile Field**: Asset field reference (Default: `Default Material Palette (Material Palette)`)
        * **Shortcut List (Slots with Asset reference fields)**:
            * **Alt + 1**: `ProBuilderDefault`
            * **Alt + 2**: `None (Material)`
            * **Alt + 3**: `None (Material)`
            * **Alt + 4**: `None (Material)`
            * **Alt + 5**: `None (Material)`
            * **Alt + 6**: `None (Material)`
            * **Alt + 7**: `None (Material)`
            * **Alt + 8**: `None (Material)`
            * **Alt + 9**: `None (Material)`
            * **Alt + 0**: `None (Material)`
        * **Add**: Button at the bottom of the shortcut list.

* 🟠 **UV Editor**
    * **Behavior Note**: Opening this tool brings up a dedicated graphical grid workspace window with an integrated top toolbar, a floating Actions panel, and a coordinate grid display. Crucially, the selection mode buttons in this window dynamically toggle the global ProBuilder selection modes, filtering the available actions in the main ProBuilder panel.
    * **Top Toolbar Icons (From Left to Right)**:
        * 🛠️ **Navigation & Transform Tools**:
            * `Pan Tool` (Icon: Open Hand)
            * `Move Tool` (Icon: 4-Way Arrow | Tooltip: `Move Tool` — Active/Blue highlighted by default)
            * `Rotate Tool` (Icon: Circular arrow | Tooltip: `Rotate Tool`)
            * `Scale Tool` (Icon: Square box with expanding arrow)
        * 📐 **Selection Mode Toggles (Changes Global ProBuilder Mode)**:
            * `Object Selection` (Icon: Cube with highlighted corners | Tooltip: `Object Selection`) — *Sets ProBuilder panel to Object commands*.
            * `Vertex Selection` (Icon: Cube with 4 separate dots | Tooltip: `Vertex Selection`) — *Appends blue selection tools and red vertex actions*.
            * `Edge Selection` (Icon: Cube with highlighted wireframe edges | Tooltip: `Edge Selection`) — *Appends blue edge modifiers and red edge actions*.
            * `Face Selection` (Icon: Cube with a highlighted side face | Tooltip: `Face Selection`) — *Appends blue face modifiers and red face actions*.
        * 🎛️ **UV Command Toggles (Independent On/Off & Modals)**:
            * `Lock SceneView Handles` (Icon: 3-Way Colored Gizmo Arrows | Tooltip: `Lock the SceneView handle tools to UV manipulation mode. This allows you to move UV coordinates directly on your 3d object.`) — *Independent toggle button*.
            * `UV Viewer / Texture Preview` (Icon: Layered grid | Visual States: Orange when enabled, Gray/White grid lines when disabled) — *Independent toggle button to draw texture patterns behind UV layout*.
            * `Render UV Template` (Icon: Camera) — *Opens a modal settings overlay menu labeled "Render UVs" containing*:
                * **Image Size**: Dropdown selection menu featuring resolution presets: `256`, `512`, `1024` (Default), `2048`, and `4096`.
                * **Hide Grid**: Checkbox toggle.
                * **Line Color**: Color picker field (Default: Vibrant Green).
                * **Include Texture**: Checkbox toggle.
                * **Transparent Background**: Checkbox toggle.
                * **Background Color**: Color picker field (Default: Black).
                * **Action Button**: `Save UV Template` button located at the bottom of the modal parameters.
        * 📋 **UV Channel Dropdown**:
            * **Channel Selection**: Dropdown menu tracking current active editing layer. Options include:
                * `UV 1` (Active editable channel)
                * `UV 2 (read-only)`
                * `UV 3 (read-only)`
                * `UV 4 (read-only)`
    * **Floating Actions Panel**:
        * **Header**: `Actions`
        * **Central State Status**: 
            * ℹ️ *No UVs Selected* (Displayed when no active UV components are chosen).
    * **Grid Workspace**:
        * **Visual Boundaries**: Features a thick bright blue square outline representing the 0-1 UV space.
        * **Origin Coordinates**: Displays a faint gray `0, 0` text indicator at the bottom-left vertex corner of the blue outline boundary.
        * **Background Layout**: Dark gray grid matrix canvas background.

* 🎨 **Vertex Colors Window**
    * **Header Controls**:
        * `Reset` button: Positioned at the top right of the window header context line.
    * **Color Palette Section**:
        * **Active Palette Selector**: A dropdown selection row labeled `Color Palette` tracking the active palette asset (Default: `📦 Default Color Palette (...)` with a target asset selector icon on the far right).
        * **Palette Matrix Rows**: Contains exactly 16 parallel color assignment rows. Each row is structured with:
            * `Apply` action button on the left to paint the selected mesh elements.
            * A wide horizontal interactive color field bar showing the current color sample.
            * An eyedropper / color sampler icon on the far right of the field bar.
        * **Default Color Palette Spectrum (Top to Bottom Rows)**:
            1. Dark Navy Blue
            2. Mid Blue
            3. Light Sky Blue
            4. Cyan / Turquoise
            5. Teal / Sea Green
            6. Bright Green
            7. Neon Mint Green
            8. Yellow
            9. Orange
            10. Red
            11. Maroon / Burgundy
            12. Magenta / Hot Pink
            13. Purple
            14. Black
            15. Medium Gray
            16. Off-White / Light Gray

* 🔵 **Selection Modifiers (Blue Section)**
    * `Rect: Intersect` / `Rect: Complete` Toggle:
        * **Behavior**: Clicking this option toggles the bounding box selection behavior between two modes:
            * `Rect: Intersect` (Default): Selects mesh elements if any part of them is touched or intersected by the drag rectangle.
            * `Rect: Complete`: Selects mesh elements only if they are completely encompassed by the drag rectangle.
        * **Official Tooltip**: 
            > Sets whether or not a mesh element (edge or face) needs to be completely encompassed by a drag to be selected.
            > 
            > The default value is Intersect, meaning if any part of the elemnent is touched by the drag rectangle it will be selected.

* 🔵 **Selection Modifiers (Blue Section)**
    * `Rect` Toggle:
        * **Behavior**: Controls bounding box selection encapsulation. Switches between:
            * `Rect: Intersect` (Default): Selects elements if any part is touched by the drag rectangle.
            * `Rect: Complete`: Selects elements only if completely enclosed inside the drag rectangle.
    * `Shift` Cycle Toggle:
        * **Behavior**: Changes how the `Shift` key modifies active drag selections. Cycles through:
            * `Shift: Difference` (Default): Inverts the selection state of the targeted elements.
            * `Shift: Add`: Always adds newly dragged elements to the current selection.
            * `Shift: Subtract`: Always removes dragged elements from the current selection.
        * **Official Tooltip**:
            > When drag selecting elements, does the shift key
            > 
            > - [Add] Always add to the selection
            > - [Subtract] Always subtract from the selection
            > - [Difference] Invert the selection by the selected faces (Default)
    * `Orientation` Cycle Toggle:
        * **Behavior**: Toggles the alignment reference of the transform gizmo handles. Cycles through:
            * `Orientation: Global`: Aligns handles to world axis space.
            * `Orientation: Local`: Aligns handles to the active object's rotation coordinates.
            * `Orientation: Normal`: Aligns handles directly with the active element selection's normal vector.
        * **Official Tooltips**:
            * *Local State*: `The transform handle is aligned with the active object rotation.`
            * *Normal State*: `The transform handle is aligned with the active element selection.`
    * `Select Hidden` Toggle:
        * **Behavior**: Controls backface and occlusion culling during component selection. Toggles between:
            * `Select Hidden: On` (Default): Allows selection of obscured or camera-facing backfaces.
            * `Select Hidden: Off`: Limits selection exclusively to elements directly visible to the camera view.
        * **Official Tooltip**:
            > Setting Hidden Element Selection to On allows you to select faces that are either obscured by geometry or facing away from the scene camera (backfaces).
            > 
            > The default value is On.
    * `Select Face Loop` / `Select Face Ring`: Action items without sub-menus.
    * `Select by Material` `[+]` / `Select by Colors` `[+]`: 
        * **UI Indicator**: Features a small blue `+` square icon on the far right. 
        * **Human/AI Note**: This indicator signals that a secondary option window/overlay can be opened to configure parameters before running the selection tool.
    * `Shrink Selection` / `Grow Selection`: Direct component selection scaling actions.

* 🟢 *Conform Normals* `[Disabled — Greyed out]`
* 🟢 *Export* `[Disabled — Greyed out]` `[ + ]`
* 🟢 **Lightmap UVs** `[Always Enabled]` `[ + ]`
* 🟢 *Triangulate* `[Disabled — Greyed out]`
* 🟢 *Center Pivot* `[Disabled — Greyed out]`
* 🟢 *ProBuilderize* `[Disabled — Greyed out]` `[ + ]`
* 🟢 *Subdivide Object* `[Disabled — Greyed out]`
* 🟢 *Flip Normals* `[Disabled — Greyed out]`
* 🟢 *Mirror Objects* `[Disabled — Greyed out]` `[ + ]`
* 🟢 *Merge Objects* `[Disabled — Greyed out]`
* 🟢 *Freeze Transform* `[Disabled — Greyed out]`
* 🟢 *Set Trigger* `[Disabled — Greyed out]`
* 🟢 *Set Collider* `[Disabled when no mesh selected]`
