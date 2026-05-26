# CohesiveAR

**Cohesive AR Content via Concurrent Extraction and Mapping of Real-World Textures**  
*Completed at UCSB, Fall 2022*

---

## 💡 Overview
Objects in AR can often appear disconnected from the real world. What if you could use textures from your immediate surroundings to create new virtual objects?

CohesiveAR allows developers to extract real-world textures and apply them dynamically onto virtual scene objects.
*   **Seamless Transitions:** Blend virtual and physical objects smoothly within a single scene.
*   **Immersive Experience:** Provide users with a highly cohesive, realistic AR environment.

## 📽️ Project Demo

[![CohesiveAR Demo Video](animation.webp)](https://www.youtube.com/watch?v=eUzmJmamqFk)

🔗 **[Watch the Full App Demo Video on YouTube](https://www.youtube.com/watch?v=eUzmJmamqFk)**

---

## 🖼️ Screenshots

![Surface Scanning Results](Capture.PNG)

*Figure 1 (a, b, c): Results of scanning a variety of surface textures in outdoor and indoor environments located in San Clemente Villages, UCSB (November 25th, 2022).*

## 🛠️ Tech Stack
*   **Engine & Languages:** Unity, C#, C++, ShaderLab
*   **Frameworks:** Google ARCore, OpenCV

## 📦 Project Components
*   **[Cohesive-AR-ARCore](https://github.com/CohesiveAR/Cohesive-AR-ARCore):** Main ARCore integration pipeline.
*   **[Texture-Scan](https://github.com/CohesiveAR/Texture-Scan):** Marker-based texture scanning scripts.
*   **[OpenCv-Editing-for-Image](https://github.com/CohesiveAR/OpenCv-Editting-for-Image-):** Image processing scenes and custom Shaders.
*   **[Manipulate-Scene-Object](https://github.com/CohesiveAR/Manipulate-Scene-Object):** C++ engine logic for object scaling, rotation, and texture mapping.
