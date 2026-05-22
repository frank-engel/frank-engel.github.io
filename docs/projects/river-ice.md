# River Ice Detection (RIce-Net)

<!-- 🖼️ TODO: Need updated cover image showing ice detection results -->

![River Ice](../img/project-6-cover.png){ align=right width="300" }

**RIce-Net** is a machine learning framework that identifies the presence of river ice using imagery captured by the National Imagery Management System (NIMS) and available through HIVIS. Developed in collaboration with the Stevens Institute of Technology.

---

## Overview

River ice affects streamflow measurement accuracy, infrastructure safety, and flood risk. Traditional ice detection relies on manual observation or in-situ sensors with limited spatial coverage. RIce-Net leverages the national-scale imagery archive provided by NIMS to automate ice detection using deep learning.

## Results

- **94% accuracy** in automated river ice detection
- Trained on USGS HIVIS camera imagery from diverse geographic locations
- Operates on standard ground-based camera imagery (no specialized sensors required)

## My Role

I contributed the data infrastructure (NIMS/HIVIS imagery), provided domain expertise on camera deployment and image quality, and collaborated on model design and validation. My contribution focused on data production (60%) and ensuring the ML pipeline was compatible with operational USGS imagery workflows.

## Collaboration

This project is a collaboration with:

- **Stevens Institute of Technology** — ML model development (Dr. Marouane Temimi)
- **USGS Hydrologic Remote Sensing Branch** — imagery infrastructure and domain expertise

## Publication

Ayyad, M., Temimi, M., Abdelkader, M., Henein, M., **Engel, F.L.**, Lotspeich, R.R., and Eggleston, J.R., 2025, RIce-Net — Integrating ground-based USGS HIVIS cameras and machine learning for automated river ice detection. *Engineering Applications of Artificial Intelligence*, [doi:10.1016/j.envsoft.2025.106454](https://doi.org/10.1016/j.envsoft.2025.106454).

## Related

- [NIMS](nims.md) — provides the imagery data
- [ECHO AI Skunkworks](echo.md) — exploring additional ML applications on NIMS data
