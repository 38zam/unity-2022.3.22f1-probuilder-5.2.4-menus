# Unity Top Menu Access — Tools > ProBuilder

This file indexes the complete structural hierarchy of the ProBuilder menu located in the Unity top menu bar within Unity 2022.3.22f1 and ProBuilder 5.2.4.

---

## 📂 Menu Path: Tools > ProBuilder >

* **ProBuilder Window** — Opens the main ProBuilder editing window and dynamic panel.
* **Editors >** — Sub-menu for external editing modules.
  * *New Bezier Shape* `[Disabled when no mesh selected]`
  * *New Poly Shape Toggle* `[Disabled when no mesh selected]`
  * *New Shape Toggle ( Ctrl+Shift+K )* `[Disabled when no mesh selected]`
  * **Open Lightmap UV Editor [Always Enabled]** — Opens the baking UV configuration window.
  * *Open Material Editor* `[Disabled when no mesh selected]`
  * *Open Smoothing Editor* `[Disabled when no mesh selected]`
  * *Open UV Editor* `[Disabled when no mesh selected]`
  * *Open Vertex Color Editor* `[Disabled when no mesh selected]`
  * *Open Vertex Position Editor* `[Disabled when no mesh selected]`
* **Dimensions Overlay >** — Sub-menu for grid and dimension overlay settings.
  * **Show Dimensions [Always Enabled]** — Toggles the measurement display for selected bounding boxes.

---

* **Selection >** — Sub-menu for advanced object/element selection actions.
  * *Select Loop* `[Disabled when no mesh selected]`
  * *Select Ring* `[Disabled when no mesh selected]`
  * *Grow Selection* `[Disabled when no mesh selected]`
  * *Shrink Selection* `[Disabled when no mesh selected]`
  * *Select Hole* `[Disabled when no mesh selected]`
  * *Select Vertex Color* `[Disabled when no mesh selected]`
* **Interaction >** — Sub-menu for interaction behaviors and tools.
  * **Toggle Edit Mode [Always Enabled]** — Switches between Object and Element editing modes.
  * **Backface Culling [Always Enabled]** — Toggles selection visibility of backward-facing polygons.
  * **Rect Select Mode >** — Bounding box selection strategy options.
    * **Complete [Always Enabled]** — Elements must be entirely inside the selection rectangle.
    * **Partial [Always Enabled]** — Elements are selected if the rectangle touches them.
* **Object >** — Sub-menu for object-level modifications.
  * **New Shape [Always Enabled]** — Opens the shape creation wizard panel.
  * *Subdivide Object* `[Disabled when no mesh selected]`
  * *Freeze Transform* `[Disabled when no mesh selected]`
* **Geometry >** — Sub-menu for structural and mesh geometry operations.
  * *Extrude* `[Disabled when no mesh selected]`
  * *Subdivide* `[Disabled when no mesh selected]`
  * *Merge Vertices* `[Disabled when no mesh selected]`
  * *Collapse Vertices* `[Disabled when no mesh selected]`
  * *Split Vertices* `[Disabled when no mesh selected]`
  * *Bevel* `[Disabled when no mesh selected]`
  * *Bridge Edges* `[Disabled when no mesh selected]`

---

* **Materials >** — Sub-menu for ProBuilder material assignment and vertex coloring shortcuts.
  * **Material Editor [Always Enabled]** — Opens the quick material palette window.
  * *Apply Material Palette* `[Disabled when no mesh selected]`
* **Vertex Colors >** — Sub-menu for vertex color editing and panels.
  * **Vertex Color Palette [Always Enabled]** — Opens the color swatch window for mesh painting.
  * *Set Selected Vertex Color* `[Disabled when no mesh selected]`

---

* **Repair >** — Sub-menu for mesh validation, rebuilding, and repair tools.
  * *Rebuild Mesh* `[Disabled when no mesh selected]`
  * *Remove Degenerate Triangles* `[Disabled when no mesh selected]`
  * **Upgrade Scene to ProBuilder 5 [Always Enabled]** — Standardizes older project data formats.

---

* **Export >** — Sub-menu for exporting ProBuilder meshes to external formats (OBJ, FBX, Asset, etc.).
  * *Export Asset* `[Disabled when no mesh selected]`
  * *Export OBJ* `[Disabled when no mesh selected]`
  * *Export FBX* `[Disabled when no mesh selected]`

---

* **Actions >** — Sub-menu for quick contextual actions.
  * *Strip ProBuilder Scripts* `[Disabled when no mesh selected]`
* **Debug >** — Sub-menu for technical logs, mesh data inspection, and debugging utilities.
  * **Force Refresh Objects [Always Enabled]** — Forces a hard update on all active scene instances.
  * **Show Vertex Markers [Always Enabled]** — Toggles structural handle rendering in the Editor view.
