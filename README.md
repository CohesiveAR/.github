# CohesiveAR

### **Cohesive Augmented Reality Content via Concurrent Extraction and Mapping of Real-World Textures** 
*Four Eyes Lab, University of California, Santa Barbara (UCSB) | Fall 2022*

>  **Repository Architecture:** The complete modular source code, dependencies, and evaluation pipelines are hosted across distinct repositories within the main organization profile.
>  **[Access the CohesiveAR Organization Profile](https://github.com/CohesiveAR)**

---

## System Overview & Abstract
CohesiveAR presents a real-time pipeline designed to bridge the visual discrepancy between synthetic assets and real-world environments in Augmented Reality (AR). By introducing a concurrent texture extraction and dynamic mapping framework, the system captures real-world surface materials and maps them programmatically onto virtual 3D meshes. This approach preserves local environmental context, ensuring high visual fidelity and texture cohesion across physical-virtual boundary layers.

## System Demonstration

[![CohesiveAR Evaluation Profile](profile/animation.webp)](https://www.youtube.com/watch?v=eUzmJmamqFk)

*Click the graphic above or follow the link to view the comprehensive **[System Evaluation and Real-Time Application Demo on YouTube](https://www.youtube.com/watch?v=eUzmJmamqFk)**.*

##  Technical Framework & Core Capabilities

*   **Concurrent Texture Extraction:** Real-time spatial tracking loops capture physical environmental surfaces, extracting localized pixel matrices under dynamic illumination conditions.
*   **Homography & Geometric Rectification:** Utilizes edge-side image processing pipelines to execute perspective transformation, lens distortion correction, and surface normalization.
*   **Context-Aware Mesh Mapping:** Coordinates low-latency vertex-to-pixel projection to wrap recovered material textures onto arbitrary, constraint-bound virtual geometries.
*   **Low-Level Render Pipeline Optimization:** Deploys custom rasterization shaders to achieve fluid frame rates on mobile hardware targets.

##  Core Infrastructure & Tooling
*   **Graphics & Runtime Engines:** Unity, C#, C++ Engine Core
*   **Spatial Computing Frameworks:** Google ARCore Spatial Mapping SDK
*   **Computer Vision Libraries:** OpenCV (Real-Time Image Processing & Matrix Manipulations)

##  Modular Subsystem Repositories

The architecture is fully decoupled to isolate the tracking, processing, and rendering layers:

*   **`Cohesive-AR-ARCore`** — *[Access Link](https://github.com/CohesiveAR/Cohesive-AR-ARCore)*  
The central Unity application runtime serving as the main orchestration engine; integrates the spatial state estimation, device tracking lifecycle, and all downstream subsystem components.
*   **`Texture-Scan`** — *[Access Link](https://github.com/CohesiveAR/Texture-Scan)*  
    Marker-based initialization arrays, surface boundary isolation scripts, and texture region-of-interest (ROI) segmentation.
*   **`OpenCv-Editing-for-Image`** — *[Access Link](https://github.com/CohesiveAR/OpenCv-Editting-for-Image-)*  
    Computer vision preprocessing scenes, matrix transforms, filters, and custom rendering shaders for photometric normalization.
*   **`Manipulate-Scene-Object`** — *[Access Link](https://github.com/CohesiveAR/Manipulate-Scene-Object)*  
    Low-level C++ rendering engine logic managing affine transformations (scaling, rotation), runtime memory allocations, and dynamic UV mapping matrices.
