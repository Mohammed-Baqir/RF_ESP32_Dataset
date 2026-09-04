# RF_ESP32_Dataset
Self-collected ESP32 WiFi CSI dataset (2.4 GHz, 64 subcarriers) with 192 RF sessions across 8 indoor environments: 71 human-activity, 63 metal/object, and 58 environment-with-metal recordings. Includes CSI, AGC, FFT data, event labels, and metadata. Supports cross-environment RF sensing research.


# RF HAR Dataset

Self-collected ESP32-based WiFi CSI dataset (2.4 GHz, 20 MHz, 64 subcarriers) used in our paper


## Session counts
| Subset                    | Sessions |
|---------------------------|---------:|
| 01_human_activity         |       71 |
| 02_metal_object           |       63 |
| 03_environment_with_metal |       58 |
| Total                     |      192 |

## Per-session files
metadata.json, events.csv, csi_data.npy, agc_data.npy, fft_data.npy, session_info.json, rf_summary.json


## 🛠️ Companion Software (CSI Tools)

This dataset exported using the companion open-source toolkit:

👉 **[RF_ESP32_CSI_Tools — Unified Wi-Fi CSI Viewer & Spatial Diversity Analyzer](https://github.com/Mohammed-Baqir/RF_ESP32_CSI_Tools)**

> The toolkit (`GUI_CSI-Dataset_Collection.py`) is the **host-side analyzer** that generated this archive.

### Hardware Setup Used for This Dataset

| Role             | Device                                                                 |
|------------------|------------------------------------------------------------------------|
| Transmitter (TX) | TP-Link Wi-Fi AP, 3 antennas, 2.4 GHz                                  |
| Receiver    (RX) | ESP32 (`esp-csi` firmware), 1 antenna, 2.4 GHz, 20 MHz, 64 subcarriers |

> Firmware flashing follows the official [Espressif esp-csi guide](https://github.com/espressif/esp-csi); the toolkit runs on the host PC after setup.

**License note:** the software is released under **Apache-2.0** (derivative of Espressif `esp-csi`), while this dataset is released under **CC BY 4.0**.


## Notes
- Person identifiers are anonymized (P01, P02, ...). The original-to-anonymized mapping is NOT included in this archive.
- The human-activity subset (group 01) is the labeled HAR subset used in the paper;
  groups 02 and 03 support metadata/domain analysis and auxiliary experiments.

## License
Creative Commons Attribution 4.0 International (CC BY 4.0).
