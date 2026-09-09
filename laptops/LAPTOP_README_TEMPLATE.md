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

| Parameter          | Value |
| ------------------ | ----- |
| Screen size        |       |
| Panel type         |       |
| Aspect ratio       |       |
| Resolution         |       |
| Backlight          |       |
| Refresh rate       |       |
| Typical brightness |       |
| Contrast ratio     |       |
| Viewing angle(H/V) |       |
| Response time      |       |

### Color characteristics

**Gamut coverage**
|      Color gamut       | Declared/known<br>coverage | Calibrated and measured<br>coverage |
| :--------------------: | :------------------------: | :---------------------------------: |
| Wide color gamut (WDC) |     :heavy_check_mark:     |             :question:              |
|          sRGB          |         ~ 97-100%          |             :question:              |
|          NTSC          |             -              |             :question:              |
|         DCI-P3         |          ~ 66-70%          |             :question:              |
|       Adobe-RGB        |             -              |             :question:              |

**Color depth:** X bit    

<p align="right">
  <a href="#table-of-contents">⬆ Toc</a>
</p>

## Calibration  

Calibration objective: **Visual comfort with reduced eye strain during prolonged use.**  

### Environment and targets

**Calibration environment**
| Parameter        | Value                                 |
| ---------------- | ------------------------------------- |
| Calibration date | 2026-09-03                            |
| Instrument       | Spyder X                              |
| Software         | DisplayCal 3.8.9.3<br>ArgyllCMS 3.5.0 |


**Calibration target**
| Parameter          | Value        |
| ------------------ | ------------ |
| Target white point | D65 (6500 K) |
| Target gamma       | 2.2          |

### OSD settings  

- Display Manager -> Color Temperature: Default

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

Post-calibration measurement with [ArgyllCMS/spotread](https://www.argyllcms.com/doc/spotread.html)

> [!NOTE]
> Recommended luminance levels:
>
> - Night: 80–100 cd/m²
> - Evening: 100–120 cd/m²
> - Daylight: 120–140 cd/m²
> - Bright daylight: 140–160 cd/m²

![Brightness vs. Luminance](brightness_vs_luminance_$PANEL.png) 

| OSD Brightness (%) | Luminance (cd/m²) |
| :----------------: | :---------------: |
|         0          |        7          |
|         10         |        21         |
|         20         |        41         |
|         30         |        75         |
|      -> 40 <-      |     -> 118 <-     |
|         50         |        176        |
|         60         |        244        |
|         70         |        317        |
|         80         |        400        |
|         90         |        488        |
|         100        |        584        |

<p align="right">
  <a href="#table-of-contents">⬆ Toс</a>
</p>