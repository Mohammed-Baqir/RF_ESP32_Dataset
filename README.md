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

## Notes
- Person identifiers are anonymized (P01, P02, ...). The original-to-anonymized mapping is NOT included in this archive.
- The human-activity subset (group 01) is the labeled HAR subset used in the paper;
  groups 02 and 03 support metadata/domain analysis and auxiliary experiments.

## License
Creative Commons Attribution 4.0 International (CC BY 4.0).
