---
hide:
  - toc
---

# El Niño & Central Texas Flood Risk — Sources & Methodology

*Supporting material for a Bexar County parish newsletter piece on the 2026–27 El Niño forecast and local flood risk. This page reflects independent, personal research conducted on my own time — it is not an official USGS product, publication, or position.*

## Forecast data

- NOAA Climate Prediction Center, [ENSO Diagnostic Discussion, Aug. 13, 2026](https://www.cpc.ncep.noaa.gov/products/analysis_monitoring/enso_advisory/ensodisc.shtml) (this is not a permalink, and contents may change over time)
- NOAA CPC monthly SST index table (`sstoi.indices`) — raw current-year monthly trajectory
- **Methodology note**: NOAA replaced its longstanding ONI (Oceanic Niño Index) with RONI (Relative Oceanic Niño Index) in February 2026, adjusting for a faster-moving climatological baseline. Figures here use NOAA's own published, RONI-aware numbers rather than an independent re-derivation from raw data, after an earlier pass through this analysis showed the two can diverge by several tenths of a degree.

## Extending the record back to 1870

- [HadISST1.1 Niño 3.4 monthly SST anomaly series](https://psl.noaa.gov/data/timeseries/month/), PSL Data Explorer
- Calibrated against NOAA's official ONI record (1950–present) before extending to pre-1950 winters; agreement within roughly 0.1–0.3°C

## San Antonio precipitation

- [NOAA/RCC Applied Climate Information System (ACIS)](https://data.rcc-acis.org), station KSAT (San Antonio airport, 1942–present)
- "SAN ANTONIO – COOP" downtown station (1885–1940), immediately preceding KSAT
- 1991–2020 normals computed from the full ACIS monthly record

## USGS river gage data

- [USGS Water Data OGC API](https://api.waterdata.usgs.gov/ogcapi/v0/) — `peaks`, `daily`, and `continuous` (15-minute instantaneous) collections
- Gages: Guadalupe River near Spring Branch (08167500), Colorado River at Austin (08158000), Nueces River near Tilden (08194500), Medina River at Bandera (08178880), Frio River at Concan (08195000), and Guadalupe River at FM474 near Bergheim (08167200)
- Daily-mean discharge alone understates flashy Hill Country flood behavior; where available (1996–present), instantaneous 15-minute discharge and stage are used in preference to daily means

## Bergheim, July 2026

The July 16, 2026 peak stage and discharge figures cited in the newsletter piece are drawn from my own field measurement, made as part of the USGS field crew on site that day. As of this writing, that peak had not yet completed USGS's official review process — treat the specific figures as a firsthand, provisional account rather than a finalized agency record.

## Raw data files

The derived datasets behind the newsletter's figures are available below:

- [nino34-hadisst-djf-1870-2026.csv](data/el-nino-2026/nino34-hadisst-djf-1870-2026.csv) — ranked DJF Niño 3.4 anomalies, 1870–2026
- [ksat-precip-sep-feb-by-year.csv](data/el-nino-2026/ksat-precip-sep-feb-by-year.csv) — San Antonio airport precipitation by strong El Niño year
- [sa-downtown-coop-precip-pre1950.csv](data/el-nino-2026/sa-downtown-coop-precip-pre1950.csv) — downtown station precipitation, pre-1950 years
- [usgs-annual-peaks-all-gages.csv](data/el-nino-2026/usgs-annual-peaks-all-gages.csv) — full annual peak-flow record, all gages
- [usgs-daily-max-in-window-summary.csv](data/el-nino-2026/usgs-daily-max-in-window-summary.csv) — max daily-mean discharge per gage per El Niño window
- [usgs-daily-discharge-el-nino-windows-full.csv](data/el-nino-2026/usgs-daily-discharge-el-nino-windows-full.csv) — full daily discharge series behind that summary
- [usgs-instantaneous-summary.csv](data/el-nino-2026/usgs-instantaneous-summary.csv) — max 15-minute discharge and stage, sub-daily era (1996–present)
- [usgs-instantaneous-top10.csv](data/el-nino-2026/usgs-instantaneous-top10.csv) — top 10 instantaneous readings per gage/window
- [usgs-peak-stage-top5-all-gages.csv](data/el-nino-2026/usgs-peak-stage-top5-all-gages.csv) — all-time top-5 peak gage height per site

---
