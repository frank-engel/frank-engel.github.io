# Machine Learning for Image Velocimetry

<!-- 🖼️ TODO: Need cover images for Auto-STIV and AIPIV (figures from papers) -->

Collaborative research applying deep learning to advance the state-of-the-art of image-based flow measurement — automating and improving the image velocimetry workflow with physics-guided deep learning.

---

## Auto-STIV

**Auto-STIV** is a deep learning framework for fully autonomous two-dimensional streamflow velocity vector field estimation. Developed in collaboration with Pennsylvania State University (Dr. Xiaofeng Liu, Dr. Roberto Fernández, and Dr. Xiaofeng Liu).

### Key Innovation

Auto-STIV eliminates the need for manual parameter tuning in space-time image velocimetry by using deep learning to automatically detect and extract velocity information from video sequences. This represents a step toward fully autonomous, real-time discharge measurement from camera imagery.

### Publication

Tenorio, A., Umarova, A., Fernández, R., **Engel, F.L.**, and Liu, X., *in review*, Auto-STIV — A deep learning framework for fully autonomous two-dimensional streamflow velocity vector field estimation: *Water Resources Research*.

---

## AIPIV

**AIPIV** (Entropy-guided deep feature particle image velocimetry) applies entropy-guided deep learning for robust river surface velocity estimation. Developed in collaboration with the Stevens Institute of Technology (Dr. Mahmoud Ayyad).

### Key Innovation

AIPIV integrates information-theory principles (entropy) with deep feature extraction to produce more robust velocity estimates under challenging field conditions — low contrast, variable lighting, and sparse surface tracers.

### Publication

Ayyad, M., **Engel, F.L.**, Temimi, M., and Henein, M.M.R., *in review*, AIPIV — Entropy-guided deep feature particle image velocimetry for robust river surface velocity estimation: *Water Resources Research*.

---

## My Role

I serve as co-PI and domain expert on both collaborations, providing:

- Operational image velocimetry expertise and validation datasets
- USGS field data and camera imagery
- Integration requirements for operational deployment
- Advising graduate students conducting the ML research

## Collaborators

- **Pennsylvania State University** — Dr. Xiaofeng Liu, Dr. Roberto Fernández, Alejandro. Tenorio (Ph.D. student)
- **Stevens Institute of Technology** — Dr. Mahmoud Ayyad, Dr. Marouane Temimi 
- **University of Arizona** — Dr. Jennifer Duan

## Related

- [IVy Tools](ivy-tools.md) — the operational framework these methods aim to enhance
- [ECHO AI Skunkworks](echo.md) — evaluating ML approaches for production readiness
