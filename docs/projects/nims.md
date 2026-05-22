# National Imagery Management System (NIMS)

<!-- 🖼️ TODO: Updated HIVIS screenshot showing 1000+ cameras on map -->

![NIMS](../img/project-4-cover.png){ align=right width="300" }

**NIMS** is a scalable cloud infrastructure for hydrologic imagery data that ingests, archives, and delivers imagery from more than 1,000 camera installations at USGS streamgages across the United States. It is the agency-wide standard platform for USGS hydrologic imagery.

[:material-api: Public API](https://api.waterdata.usgs.gov/docs/nims/){ .md-button }
[:material-web: HIVIS App](https://apps.usgs.gov/hivis/){ .md-button .md-button--primary }

---

## Overview

Prior to NIMS, no centralized infrastructure existed to ingest, archive, or deliver hydrologic imagery at national scale. Individual camera installations operated in isolation with no interoperability, no public access pathway, and no scalable operational model. NIMS resolved this through a serverless AWS architecture achieving radical cost efficiency.

## Architecture

- **Serverless AWS** — Lambda, S3, API Gateway
- **Public-facing API** — first open programmatic access to USGS hydrologic imagery
- **Interoperability** — mandatory integration with National Water Dashboard and Water Data for the Nation
- **Cost architecture** — $2/camera/month operating costs (order of magnitude below alternatives)
- **Multi-source ingestion** — CameraDCP, FTP, bulk upload, and third-party camera systems

## Impact & Scale

| Metric | Value |
|--------|-------|
| Cameras served | 1,000+ (994 publicly accessible) |
| Archived images | 110+ million |
| Growth rate | ~1 million images/week |
| API requests | 350,000–400,000/day |
| Operating cost | ~$2/camera/month |

## HIVIS

The **Hydrologic Imagery Visualization and Information System** (HIVIS) is the public-facing web application that displays NIMS imagery and derived products. I serve as Product Owner for HIVIS.

## Downstream Applications

NIMS has enabled applications beyond its original scope:

- **RIce-Net** — ML-based river ice detection (94% accuracy)
- **Image velocimetry** — real-time discharge during flood events (work in progress)
- **Water level detection** — automated ML models
- **National Water Dashboard** — public imagery integration
- Press coverage: [*New York Times*](https://www.nytimes.com/2025/08/13/climate/alaska-juneau-flood-glacier.html), [ABC News](https://abcnews.com/US/glacier-lake-outburst-alaskas-mendenhall-glacier-causes-record/story?id=124610857), [CBS News](https://www.cbsnews.com/news/juneau-alaska-flooding-mendenhall-glacier-suicide-basin-evacuation-warnings-intensify/), [GovTech](https://www.govtech.com/em/preparedness/usgs-makes-700-cameras-available-to-emergency-managers)

## Recognition

- Unit Award for Excellence of Service (2023) — "outstanding contributions advancing cameras in water monitoring"
- Led creation of the **Imagery Dataflows Function** — a new USGS enterprise organizational unit
- NEON (National Ecological Observatory Network) evaluating CameraDCP for adoption

## Technology

`AWS Lambda` · `S3` · `API Gateway` · `JavaScript` · `React` · `Node.js`
