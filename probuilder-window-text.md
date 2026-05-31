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
* 🟠 **Smoothing**
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
