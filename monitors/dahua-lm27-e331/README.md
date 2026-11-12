<!-- PAGE_STATUS: OK -->

# Dahua DHI-LM27-E331A   

27-inch QHD IPS gaming monitor featuring a **wide-gamut LED backlight**, 180 Hz refresh rate, Adaptive-Sync, and 1 ms MPRT response time.

Calibration objective: **comfortable everyday use with reduced eye strain during prolonged use, targeting the sRGB color space.**

Official product page:  <https://display.dahuasecurity.com/consumer/en/products/productDetail?product_id=139647>  

[![Page status](badges/status.svg)](#)
[![ICC profile](badges/icc.svg)](https://xdenb43.github.io/display-comfort-configurations/monitors/dahua-lm27-e331/badges/icc.html)
[![Verification report](badges/report.svg)](https://xdenb43.github.io/display-comfort-configurations/monitors/dahua-lm27-e331/badges/report.html)

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

| Parameter           | Value           |
| ------------------- | --------------- |
| Screen size         | 27"             |
| Panel type          | IPS             |
| Aspect ratio        | 16:9            |
| Resolution          | 2560 × 1440     |
| Backlight           | E-LED           |
| Refresh rate        | 180 Hz          |
| Brightness(typ)     | 300 cd/m² (max) |
| Contrast ratio      | 1000:1          |
| Viewing angle (H/V) | 178°(H)/178°(V) |
| Response time       | MPRT 1 ms       |


### Color characteristics  

**Gamut coverage**
|      Color gamut       | Declared/known<br>coverage | Calibrated and measured<br>coverage |
| :--------------------: | :------------------------: | :---------------------------------: |
| Wide color gamut (WDC) |     :heavy_check_mark:     |         :heavy_check_mark:          |
|          sRGB          |           ~ 99%            |               99.95%                |
|          NTSC          |           ~ 85%            |                  -                  |
|         DCI-P3         |             -              |               91.26%                |
|       Adobe-RGB        |             -              |               82.08%                |
   
**Color depth:** `8 bit`  

<p align="right">
  <a href="#table-of-contents">⬆ Toc</a>
</p>

## Calibration  

### Environment and targets

**Calibration environment**
| Parameter                        | Value                                 |
| -------------------------------- | ------------------------------------- |
| Calibration date                 | 2026-11-12 (YYYY-MM-DD)               |
| Instrument                       | Spyder X                              |
| White point setup software       | HCFR 2019 (Spyder X version)          |
| Calibration & profiling Software | DisplayCal 3.8.9.3<br>ArgyllCMS 3.5.0 |

**Calibration target**
| Parameter          | Value                         |
| ------------------ | ----------------------------- |
| Preset             | Office & Web (D65, Gamma 2.2) |
| Target white point | D65 (6500 K)                  |
| Target gamma       | 2.2                           |
| Target luminance   | 120 cd/m²                     |

### OSD settings  

The white point D65 is set using a 10% to 100% built-in HCFR 2019 grayscale

- Display menu:  
    - Brightness: 28  
    - Contrast: 50  
    - Black level: 50  
    - Sharpness: 50  
- Colors menu:  
    - Red: 50 (default)  
    - Green: 49 (1 click down from 50) [^1]    
    - Blue: 43 (1 click down from 44) [^1]    
- Gaming menu:  
    - FreeSync: OFF  
    - Overdrive: OFF  
    - DCR: OFF  
    - MPRT: OFF  
- Advanced menu:  
    - HDR: OFF  
- Refresh rate: 120 Hz fixed
  
[^1]: Colors have several clicks for one value  

<p align="right">
  <a href="#table-of-contents">⬆ Toc</a>
</p>

## Downloads

> [!IMPORTANT]  
> The ICC profile was created using the OSD settings listed above.  
> Different monitor settings (brightness, RGB gain, contrast, etc.) may reduce color accuracy.  

### ICC/ICM profile
- [ICC profile](https://xdenb43.github.io/display-comfort-configurations/monitors/dahua-lm27-e331/DHI-LM27-E331_120cdm2_2.2_M-S_XYZLUT_MTX.icm)

### Reports  
- [Verification report (HTML)](https://xdenb43.github.io/display-comfort-configurations/monitors/dahua-lm27-e331/Measurement_Report_DHI-LM27-E331.html)
- [Verification report (PDF)](Measurement_Report_DHI-LM27-E331.pdf)

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

![Brightness vs. Luminance](brightness_vs_luminance_dhi-lm27-e331.png) 

| OSD Brightness (%) | Luminance (cd/m²) |
| :----------------: | :---------------: |
|         0          |        27         |
|         10         |        59         |
|      -> 16 <-      |     -> 80 <-      |
|         20         |        93         |
|      -> 22 <-      |     -> 100 <-     |
|      -> 28 <-      |     -> 119 <-     |
|         30         |        127        |
|      -> 34 <-      |     -> 139 <-     |
|      -> 40 <-      |     -> 160 <-     |
|         50         |        193        |
|         60         |        223        |
|         70         |        254        |
|         80         |        284        |
|         90         |        314 [^2]   |
|        100         |        344 [^2]   |

[^2]: Measured luminance exceeds the manufacturer's specified
maximum SDR brightness of 300 cd/m². Values are retained as
experimental measurements and have not been independently verified.

<p align="right">
  <a href="#table-of-contents">⬆ Toc</a>
</p>
