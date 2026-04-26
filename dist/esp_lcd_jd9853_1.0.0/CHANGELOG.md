# Changelog

All notable changes to **esp_lcd_jd9853** will be documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
versioning follows [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-04-26

### Added

- Initial public release.
- ESP-IDF v5.x `esp_lcd` panel driver for JD9853 (Jadard).
- 240×284 IPS panel support (BOE WV018LZQ-N80-3QP1, 1.83").
- 4-wire SPI interface, RGB565 (16-bit) and RGB666 (18-bit) color depth.
- Vendor config hook for custom initialization sequences (`jd9853_vendor_config_t`).
- Helper macros: `JD9853_PANEL_BUS_SPI_CONFIG`, `JD9853_PANEL_IO_SPI_CONFIG`.

### Notes

- Tested on ESP-IDF 5.0 / 5.3 / 5.4 / 5.5.
