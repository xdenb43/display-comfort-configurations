<a id="top"></a>
# Display Comfort Configurations

A database of display configurations, calibration data and measurements focused on long-term visual comfort, readability and stable image reproduction.

This repository contains display settings, ICC/ICM color profiles, verification reports, measurements and engineering documentation for monitors, laptops, smartphones, tablets and TVs.  

[![Monitors](https://img.shields.io/github/directory-file-count/xdenb43/display-comfort-configurations/monitors?type=dir&label=Monitors&color=informational)](https://github.com/xdenb43/display-comfort-configurations/tree/main/monitors)
[![Laptops](https://img.shields.io/github/directory-file-count/xdenb43/display-comfort-configurations/laptops?type=dir&label=Laptops&color=informational)](https://github.com/xdenb43/display-comfort-configurations/tree/main/laptops)
[![Smartphones](https://img.shields.io/github/directory-file-count/xdenb43/display-comfort-configurations/smartphones?type=dir&label=Smartphones&color=informational)](https://github.com/xdenb43/display-comfort-configurations/tree/main/smartphones)
[![Tablets](https://img.shields.io/github/directory-file-count/xdenb43/display-comfort-configurations/tablets?type=dir&label=Tablets&color=informational)](https://github.com/xdenb43/display-comfort-configurations/tree/main/tablets)
[![TVs](https://img.shields.io/github/directory-file-count/xdenb43/display-comfort-configurations/tv?type=dir&label=TVs&color=informational)](https://github.com/xdenb43/display-comfort-configurations/tree/main/tv)
<a href=".meta/draft-pages/"><img align="right" src=".meta/draft-pages.svg" alt="Draft pages"></a>

<p align="center">
  ❤️ <a href="https://pay.cloudtips.ru/p/88930546">Support the project</a> ❤️
</p>

<p align="center">
  <strong>English</strong> · <a href="README_RU.md">Русский</a>
</p>

## Table of contents

- [Repository structure](#repository-structure)
- [Device categories](#device-categories)
- [Configuration and calibration philosophy](#configuration-and-calibration-philosophy)
- [Disclaimer](#disclaimer)
- [License](#license)

## Repository structure

```text
display-comfort-configurations/
├── monitors/
│   └── device-name/
│       ├── README.md
│       ├── profile.icm
│       └── verification-report.html
│
├── laptops/
├── smartphones/
├── tablets/
├── tv/
└── .meta/
```
Each device directory is ***self-contained*** and may include:  
- documentation  
- display configuration for a **specific use case** 
- ICC/ICM color profiles  
- verification reports  
- additional measurements or notes  

## Device categories

| Category       | Description                              |
| -------------- | ---------------------------------------- |
| 🖥️ Monitors    | External LCD, Mini LED and OLED displays |
| 💻 Laptops     | Built-in notebook displays               |
| 📱 Smartphones | Mobile device displays                   |
| 📱 Tablets     | Tablet displays                          |
| 📺 TVs         | Television displays                      |


## Configuration and calibration philosophy

The repository follows a physics-first and verification-first approach.  
- Display behavior is determined primarily by the physical characteristics of the display.
- Display settings are selected based on the display's hardware characteristics and, where available, real measurements.
- Monitors and laptops:
  - Display calibration is performed primarily using the display's own hardware controls whenever possible.
  - ICC/ICM color profiles complement display calibration; they do not change the physical properties of the display.
  - Calibration verification reports and measurements are provided whenever available.
- Smartphones and tablets:
  - Priority is given to display settings for everyday use, optimized for long-term visual comfort and text readability.
- TVs:
  - Priority is given to display settings and color correction for entertainment content such as movies and TV shows.

## Disclaimer

Calibration and display configuration results are ***device-specific***.

Even identical display models may differ due to manufacturing tolerances, panel revisions, aging, firmware, display modes and user settings. Published configurations and profiles should therefore be considered reference configurations and may not provide identical results on another unit. 

## License

Unless otherwise stated, all documentation is released under the [MIT License](LICENSE).  

Calibration profiles, verification reports, measurements and configuration recommendations are provided for educational and research purposes.  

<p align="right">
  <a href="#top">⬆️ Top</a>
</p>
