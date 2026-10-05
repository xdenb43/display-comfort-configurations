<!-- PAGE_STATUS: DRAFT -->

# HP ProBook 450 G8    

15.6-inch 16:9 IPS display with a **BOE09D8** panel and standard White LED backlight.

Calibration optimized for visual comfort using Spyder X and DisplayCAL.

Official product page: <https://hp.it-shop.bg/uploaded/8/4/ProBook-450-G8-QS.pdf>

[![Page status](badges/status.svg)](#)
[![ICC profile](badges/icc.svg)](https://xdenb43.github.io/display-comfort-configurations/laptops/hp-probook-450-g8/badges/icc.html)
[![Verification report](badges/report.svg)](https://xdenb43.github.io/display-comfort-configurations/laptops/hp-probook-450-g8/badges/report.html)

## Table of contents

- [Specifications](#specifications)
  - [Color characteristics](#color-characteristics)
- [Calibration](#calibration)
  - [Environment and targets](#environment-and-targets)
  - [OSD settings](#osd-settings)
- [Downloads](#downloads)
  - [ICC/ICM profile](#iccicm-profile)
  - [Reports](#reports)
- [Brightness response curve](#brightness-response-curve)

## Specifications  

| Parameter           | Value                      |
| ------------------- | -------------------------- |
| Screen size         | 15.6"                      |
| Panel type          | IPS (ADS)                  |
| Aspect ratio        | 16:9                       |
| Resolution          | 1920 × 1080                |
| Backlight           | White LED (WLED), Edge-lit |
| Refresh rate        | 60 Hz                      |
| Typical brightness  | 250 nits                   |
| Contrast ratio      | 800:1                      |
| Viewing angle (H/V) | 85°/85°/85°/85° (typ.)     |
| Response time       | 20 ms (Tr+Td)              |

### Color characteristics  

**Gamut coverage**
|      Color gamut       | Declared/known<br>coverage | Calibrated and measured<br>coverage |
| :----------------------: | :--------------------------: | :-----------------------------------: |
| Wide color gamut (WDC) |             -              |                  -                  |
|          sRGB          |           ~ 63%            |               60.45%                |
|          NTSC          |           ~ 45%            |                  -                  |
|         DCI-P3         |             -              |               43.53%                |
|       Adobe-RGB        |             -              |               42.35%                |
   
**Color depth:** 6-bit + FRC / 262K native panel colors    

<p align="right">
  <a href="#table-of-contents">⬆ Toc</a>
</p>


## Calibration  

Calibration objective: **Visual comfort with reduced eye strain during prolonged use.**  

### Environment and targets

**Calibration environment**
| Parameter        | Value                                 |
| ---------------- | ------------------------------------- |
| Calibration date | 2026-09-28 (YYYY-MM-DD)               |
| Instrument       | Spyder X                              |
| Software         | DisplayCal 3.8.9.3<br>ArgyllCMS 3.5.0 |


**Calibration target**
| Parameter          | Value              |
| ------------------ | ------------------ |
| Target white point | D65 (6500 K)       |
| Target gamma       | 2.2                |

<p align="right">
  <a href="#table-of-contents">⬆ Toc</a>
</p>

## Downloads

### ICC/ICM profile
- [ICC profile](https://xdenb43.github.io/display-comfort-configurations/laptops/hp-probook-450-g8/BOE09D8_D6500_2.2_F-S_XYZLUT_MTX.icm)

### Reports  
- [Verification report (HTML)](https://xdenb43.github.io/display-comfort-configurations/laptops/hp-probook-450-g8/Measurement_Report_BOE09D8.html)
- [Verification report (PDF)](Measurement_Report_BOE09D8.pdf)

<p align="right">
  <a href="#table-of-contents">⬆ Toc</a>
</p>


## Brightness response curve

Post-calibration measurement with [ArgyllCMS/spotread](https://www.argyllcms.com/doc/spotread.html)

> [!NOTE]
> Recommended luminance levels:
>
> - Night: 80–100 cd/m²
> - Evening: 100–120 cd/m²
> - Daylight: 120–140 cd/m²
> - Bright daylight: 140–160 cd/m²

![Brightness vs. Luminance](brightness_vs_luminance_BOE0852.png) 

| OSD Brightness (%) | Luminance (cd/m²) |
| :----------------: | :---------------: |
|         0          |        13         |
|         10         |        19         |
|         20         |        27         |
|         30         |        38         |
|         40         |        55         |
|      -> 50 <-      |     -> 79 <-      |
|      -> 60 <-      |     -> 100 <-     |
|      -> 97 <-      |     -> 119 <-     |
|      -> 70 <-      |     -> 128 <-     |
|      -> 74 <-      |     -> 141 <-     |
|      -> 80 <-      |     -> 164 <-     |
|         90         |        209        |
|        100         |        268        |

<p align="right">
  <a href="#table-of-contents">⬆ Toc</a>
</p>