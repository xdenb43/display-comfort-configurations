<!-- PAGE_STATUS: DRAFT -->

# [Device Name]

[Short description of the device and display $PANEL.]

Official product page: [URL]

[![Page status](badges/status.svg)](#)
[![ICC profile](badges/icc.svg)](https://xdenb43.github.io/display-configuration-database/laptops/$DEVICE/badges/icc.html)
[![Verification report](badges/report.svg)](https://xdenb43.github.io/display-configuration-database/laptops/$DEVICE/badges/report.html)

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

| Parameter           | Value |
| ------------------- | ----- |
| Screen size         |       |
| Panel type          |       |
| Aspect ratio        |       |
| Resolution          |       |
| Backlight           |       |
| Refresh rate        |       |
| Typical brightness  |       |
| Contrast ratio      |       |
| Viewing angle (H/V) |       |
| Response time       |       |


### Color characteristics

**Gamut coverage**
|      Color gamut       | Declared/known<br>coverage | Calibrated and measured<br>coverage |
| :--------------------: | :------------------------: | :---------------------------------: |
| Wide color gamut (WDC) |     :heavy_check_mark:     |             :question:              |
|          sRGB          |         ~ 97-100%          |             :question:              |
|          NTSC          |             -              |             :question:              |
|         DCI-P3         |          ~ 66-70%          |             :question:              |
|       Adobe-RGB        |             -              |             :question:              |

**Color depth**: X bit    

<p align="right">
  <a href="#table-of-contents">⬆ Toc</a>
</p>

## Calibration  

Calibration objective: **Visual comfort with reduced eye strain during prolonged use.**  

### Environment and targets

**Calibration environment**
| Parameter        | Value                                 |
| ---------------- | ------------------------------------- |
| Calibration date | YYYY-MM-DD                            |
| Instrument       | Spyder X                              |
| Software         | DisplayCal 3.8.9.3<br>ArgyllCMS 3.5.0 |


**Calibration target**
| Parameter          | Value        |
| ------------------ | ------------ |
| Target white point | D65 (6500 K) |
| Target gamma       | 2.2          |
| Target luminance   | 120 cd/m²    |

### OSD settings  

- Display menu:  
    - Brightness: 22  
    - Contrast: 50  
    - Black level: 50  
    - Sharpness: 50  
- Colors menu:  
    - Red: 50  
    - Green: 49  
    - Blue: 43  
- Gaming menu:  
    - FreeSync: OFF  
    - Overdrive: OFF  
    - DCR: OFF  
    - MPRT: OFF  
- Advanced menu:  
    - HDR: OFF  
- Refresh rate: 120 Hz fixed

<p align="right">
  <a href="#table-of-contents">⬆ Toc</a>
</p>

## Downloads

> [!IMPORTANT]  
> The ICC profile was created using the OSD settings listed above.  
> Different monitor settings (brightness, RGB gain, contrast, etc.) may reduce color accuracy.  

### ICC/ICM profile
- [ICC profile](https://xdenb43.github.io/display-configuration-database/laptops/$DEVICE/$PANEL_120cdm2_D6500_2.2_M-S_XYZLUT_MTX.icm)

### Reports  
- [Verification report (HTML)](https://xdenb43.github.io/display-configuration-database/laptops/$DEVICE/Measurement_Report_$PANEL.html)
- [Verification report (PDF)](Measurement_Report_$PANEL.pdf)

<p align="right">
  <a href="#table-of-contents">⬆ Toc</a>
</p>

## Brightness response curve  

Pre-calibration measurement with [DisplayCal interactive mode](https://displaycal.net/#settings_calibration)

> [!NOTE]
> Recommended luminance levels:
>
> - Night: 80–100 cd/m²
> - Evening: 100–120 cd/m²
> - Daylight: 120–140 cd/m²
> - Bright daylight: 140–160 cd/m²

![Brightness vs. Luminance](brightness_vs_luminance_$DEVICE.png) 

| OSD Brightness (%) | Luminance (cd/m²) |
| :----------------: | :---------------: |
|         0          |        28         |
|         4          |        40         |
|         10         |        60         |
|         13         |        70         |
|      -> 16 <-      |     -> 80 <-      |
|         17         |        85         |
|         19         |        90         |
|      -> 22 <-      |     -> 100 <-     |
|      -> 27 <-      |     -> 120 <-     |
|      -> 33 <-      |     -> 140 <-     |
|         36         |        150        |
|         50         |        197        |
|         75         |        276        |
|        100         |        351        |

<p align="right">
  <a href="#table-of-contents">⬆ Toс</a>
</p>