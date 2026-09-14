<!-- PAGE_STATUS: OK -->

# Huawei Matebook X Pro 2020 (MACHC-WAX9)   

13.9-inch 3:2 LTPS display with a **JDI LPM139M422A** panel and wide-gamut LED backlight.

Calibration optimized for visual comfort using Spyder X and DisplayCAL.

Official product page:  <https://consumer.huawei.com/ie/laptops/matebook-x-pro-2020/specs/>  

[![Page status](badges/status.svg)](#)
[![ICC profile](badges/icc.svg)](https://xdenb43.github.io/display-comfort-configurations/laptops/huawei-matebook-x-pro-2020/badges/icc.html)
[![Verification report](badges/report.svg)](https://xdenb43.github.io/display-comfort-configurations/laptops/huawei-matebook-x-pro-2020/badges/report.html)

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

| Parameter          | Value           |
| ------------------ | --------------- |
| Screen size        | 13.9"           |
| Panel type         | LTPS            |
| Aspect ratio       | 3:2             |
| Resolution         | 3000 × 2000     |
| Backlight          | LED             |
| Refresh rate       | 60 Hz           |
| Typical brightness | 450 nits        |
| Contrast ratio     | 1500:1          |
| Viewing angle(H/V) | 178°(H)/178°(V) |
| Response time      | ~31 ms          |

### Color characteristics  

**Gamut coverage**
|      Color gamut       | Declared/known<br>coverage | Calibrated and measured<br>coverage |
| :--------------------: | :------------------------: | :---------------------------------: |
| Wide color gamut (WDC) |     :heavy_check_mark:     |         :heavy_check_mark:          |
|          sRGB          |         ~ 97-100%          |                96.9%                |
|          NTSC          |             -              |                  -                  |
|         DCI-P3         |          ~ 66-70%          |                70.8%                |
|       Adobe-RGB        |             -              |               67.37%                |

**Color depth:** 8 bit    

<p align="right">
  <a href="#table-of-contents">⬆ Toc</a>
</p>

## Calibration  

Calibration objective: **Visual comfort with reduced eye strain during prolonged use.**  

### Environment and targets

**Calibration environment**
| Parameter        | Value                                 |
| ---------------- | ------------------------------------- |
| Calibration date | 2026-09-04                            |
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
- [ICC profile](https://xdenb43.github.io/display-comfort-configurations/laptops/huawei-matebook-x-pro-2020/LPM139M422A_120cdm2_D6500_2.2_M-S_XYZLUT_MTX.icm)

### Reports  
- [Verification report (HTML)](https://xdenb43.github.io/display-comfort-configurations/laptops/huawei-matebook-x-pro-2020/Measurement_Report_LPM139M422A.html)
- [Verification report (PDF)](Measurement_Report_LPM139M422A.pdf)

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

![Brightness vs. Luminance](brightness_vs_luminance_LPM139M422A.png) 

| OSD Brightness (%) | Luminance (cd/m²) |
| :----------------: | :---------------: |
|         0          |         7         |
|         10         |        21         |
|         20         |        40         |
|         30         |        73         |
|      -> 32 <-      |     -> 80 <-      |
|      -> 37 <-      |     -> 101 <-     |
|      -> 40 <-      |     -> 116 <-     |
|      -> 41 <-      |     -> 120 <-     |
|      -> 45 <-      |     -> 144 <-     |
|         50         |        173        |
|         60         |        239        |
|         70         |        310        |
|         80         |        391        |
|         90         |        478        |
|        100         |        572        |

<p align="right">
  <a href="#table-of-contents">⬆ Toc</a>
</p>