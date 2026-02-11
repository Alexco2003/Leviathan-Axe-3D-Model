# 🪓 Leviathan Axe - Game Ready 3D Asset

> A high-fidelity, game-ready recreation of Kratos' **Leviathan Axe** from *God of War*. Modeled in Blender, textured in Adobe Substance 3D Painter, and optimized for modern game engines.

![Render Preview](renders/render1.png)

## 📥 Download (Game Ready)
For the final, usable asset (FBX + Textures) ready to be dropped into your preferred game engine, please check the **Releases** section.
* **[🔗 Download Latest Release](https://github.com/Alexco2003/Leviathan-Axe-3D-Model/releases)**
    * *Includes: `CA_Leviathan_Axe.fbx` and 4K PBR Textures.*

---

### ✅ Project Requirements & Implementation
The project was developed to meet the official exam criteria, which are documented in the `requirements/` folder in both `requirementsRo.txt` and `requirementsEn.txt`.

#### 1. 3D Modeling
* **High Poly (Mandatory):** Created a high-resolution sculpt (`axe_hp`) to capture fine surface details and runes.
* **Procedural Modeling (Optional):** Implemented a non-destructive workflow using a modifier stack (Mirror, Bevel, Subdivision) to ensure procedural flexibility.
* **Low Poly (Optional):** Optimized the final mesh (`axe_lp`) for game engine performance, achieving approximately 4,000 triangles.

#### 2. UV Mapping
* **UV Unwrapping:** Developed clean and coherent UV maps to ensure professional texture density and zero overlapping.

#### 3. Texturing
* **PBR Workflow:** Applied professional texturing in Adobe Substance 3D Painter using a Metal/Roughness PBR workflow.
* **Detail Baking:** Baked high-poly data (Normal, AO, Curvature) onto the low-poly mesh to simulate complex geometry with high performance efficiency.
* **Source Project:** The complete texturing process, including layers, masks, and bakes, is available for review in the `CA_Leviathan_Axe.spp` file.

#### 4. Final Presentation
* **Scene Setup:** Configured a dedicated presentation scene with PBR materials and custom lighting.
* **Rendering:** Generated high-quality final presentation renders using the **Cycles** engine.

---

## 🛠️ Blender Project Structure (`.blend`)
The main project file `CA_Leviathan_Axe.blend` is organized with a clear hierarchy to distinguish between high-poly data and game-ready assets.

**⚠️ Important:** By default, the viewport may open in *Solid Mode*. To view the final materials and lighting, press `Z` and switch to **Rendered View**.

### Scene Hierarchy Breakdown:

#### Collections (Folders):
* **📁 `backup`**: Stores iterative saves and non-destructive versions of the model used during the procedural phase.
* **📁 `lights`**: Contains the lighting setup (Point Lights) created for the presentation scene.
* **📁 `camera`**: Houses the active camera used for generating the final renders.

#### Objects (Meshes):
* **🔸 `axe_hp`**: The **High Poly** version of the blade. This object contains the full sculpted detail and runes required by the project criteria.
* **🔸 `axe_lp`**: The **Low Poly** game-ready blade. This is the optimized version used for the final PBR texturing.
* **🔸 `handle`**: The separate mesh for the wooden handle, allowing for independent UV mapping and material application.

---

## 📂 Repository Structure
Here is an overview of the files included in this repository:

```text
root/
├── 📂 assets/
│   ├── 📂 meshMaps/        # Baked maps (AO, Curvature, Normal from High Poly)
│   ├── 📂 ornaments/       # Alphas and stencils used for the runes
│   └── 📂 textures/        # Final exported PBR textures (BaseColor, Normal, Roughness, Metallic)
│
├── 📂 renders/             # High-quality PNG renders of the final object
│
├── 📂 requirements/        # Project assignment documentation
│
├── 📄 CA_Leviathan_Axe.blend # MAIN PROJECT FILE (Blender 5.0.1)
│                             # Contains scenes, materials, and modeling stages.
│
├── 📄 CA_Leviathan_Axe.spp   # TEXTURING SOURCE FILE (Substance 3D Painter)
│                             # Contains the full layer stack and materials.
│
├── 📄 .gitattributes         # Git LFS configuration for large file handling
└── 📄 README.md              # Project documentation
```
---

## 🚀 Tech Stack

The development of this asset involved a professional industry-standard pipeline to ensure high visual quality and technical optimization:

* **Blender 5.0.1:** Primary tool used for **High Poly** sculpting, **Low Poly** modeling, UV unwrapping, and final **Cycles** rendering.
* **Adobe Substance 3D Painter:** Used for professional **PBR texturing**, detail baking (Normal, AO, Curvature), and material authoring.
* **Git LFS (Large File Storage):** Utilized for efficient version control of large binary files like `.blend` and `.spp` projects.

---
