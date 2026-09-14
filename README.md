<a id="top"></a>
# Display Comfort Configurations

A database of display configurations, calibration data and measurements focused on long-term visual comfort, readability and stable image reproduction.

This repository contains display settings, ICC/ICM color profiles, verification reports, measurements and engineering documentation for monitors, laptops, smartphones, tablets and TVs.

[🇷🇺 Русская версия](README_ru.md)

[![Monitors](https://img.shields.io/github/directory-file-count/xdenb43/display-comfort-configurations/monitors?type=dir&label=Monitors&color=informational)](https://github.com/xdenb43/display-comfort-configurations/tree/main/monitors)
[![Laptops](https://img.shields.io/github/directory-file-count/xdenb43/display-comfort-configurations/laptops?type=dir&label=Laptops&color=informational)](https://github.com/xdenb43/display-comfort-configurations/tree/main/laptops)
[![Smartphones](https://img.shields.io/github/directory-file-count/xdenb43/display-comfort-configurations/smartphones?type=dir&label=Smartphones&color=informational)](https://github.com/xdenb43/display-comfort-configurations/tree/main/smartphones)
[![Tablets](https://img.shields.io/github/directory-file-count/xdenb43/display-comfort-configurations/tablets?type=dir&label=Tablets&color=informational)](https://github.com/xdenb43/display-comfort-configurations/tree/main/tablets)
[![TVs](https://img.shields.io/github/directory-file-count/xdenb43/display-comfort-configurations/tv?type=dir&label=TVs&color=informational)](https://github.com/xdenb43/display-comfort-configurations/tree/main/tv)
<a href=".meta/draft-pages/"><img align="right" src=".meta/draft-pages.svg" alt="Draft pages"></a>

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
Each device directory is self-contained and may include  
- documentation  
- display configuration  
- color profiles  
- calibration verification reports  
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
- Settings are selected based on the display's hardware characteristics and, where available, real measurements.
- Monitor calibration is performed through the display's hardware controls whenever possible.
- ICC/ICM profiles complement display calibration and color management; they do not change the physical properties of the display.
- Smartphone and tablet entries primarily document daily-use configurations optimized for long-term visual comfort, readability and appropriate luminance.
- Verification reports and measurements are provided whenever available to document the resulting display behavior.
- Changes to calibration or configuration parameters are made only after verification rather than by assumption.

## Disclaimer

Calibration and display configuration results are device-specific.

Even identical display models may differ due to manufacturing tolerances, panel revisions, aging, firmware, display modes and user settings. Published configurations and profiles should therefore be considered reference configurations and may not provide identical results on another unit. 

## License

Unless otherwise stated, all documentation is released under the MIT License.  

Calibration profiles, verification reports, measurements and configuration recommendations are provided for educational and research purposes.  

<p align="right">
  <a href="#top">⬆️ Top</a>
</p>