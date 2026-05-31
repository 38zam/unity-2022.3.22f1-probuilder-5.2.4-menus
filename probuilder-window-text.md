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
* 🟠 **UV Editor**
* 🟠 **Vertex Colors**

* 🔵 **Orientation: Global**

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
