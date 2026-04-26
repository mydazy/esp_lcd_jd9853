# Changelog

All notable changes to **esp_lcd_jd9853** will be documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
versioning follows [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.0.0] - 2026-04-26

### Notes

- **No API or behavior change.** Driver was already pure C since v1.0.0.
- Version aligned with the **mydazy/esp_lcd_touch_axs5106l** and **mydazy/esp_sc7a20h** v2.0.0 release, which underwent a full C rewrite. Bumping all three together lets integrators pin a single major version (`^2.0.0`).
- Source-compatible drop-in for v1.0.1.

## [1.0.1] - 2026-04-26

### Changed

- In-source comments translated from Chinese to English for global readability.
- Default vendor init sequence: clarifying source attribution comment added.

### Added

- `.clang-format` — Google C++ based style with ESP-IDF conventions.
- GitHub Actions multi-IDF-version build matrix (5.3 / 5.4 / 5.5).

### Notes

- No API changes. Source-compatible drop-in for v1.0.0.

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
