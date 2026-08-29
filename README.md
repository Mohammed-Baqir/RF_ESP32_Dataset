# RF_ESP32_Dataset
Self-collected ESP32 WiFi CSI dataset (2.4 GHz, 64 subcarriers) with 192 RF sessions across 8 indoor environments: 71 human-activity, 63 metal/object, and 58 environment-with-metal recordings. Includes CSI, AGC, FFT data, event labels, and metadata. Supports cross-environment RF sensing research. Anonymized identifiers.


Dataset Structure:

01 = Human Activity
02 = Metal and objects
03 = Environment with metals (share with 01 & 02)

Example: session_20250313_142305/

data/
└── 01/
    └── session_20250313_142305/
        ├── metadata.json
        ├── events.csv
        ├── csi_data.npy
        ├── agc_data.npy
        ├── fft_data.npy
        ├── session_info.json
        └── rf_summary.json
    02/
    └── session_20250313_142305/
        ├── metadata.json
        ├── events.csv
        ├── csi_data.npy
        ├── agc_data.npy
        ├── fft_data.npy
        ├── session_info.json
        └── rf_summary.json
    03/
    └── session_20250313_142305/
        ├── metadata.json
        ├── events.csv
        ├── csi_data.npy
        ├── agc_data.npy
        ├── fft_data.npy
        ├── session_info.json
        └── rf_summary.json



-----
The below points are shared and should be considered by all the environments, HAR, metal objects and distances.
Where:

1. object_type (related with HAR and type of metal)
2. activity (related with HAR only)
3. distance (related with HAR, Metal and Environments)
4. environment (related with all)
5. person_id (related with one person, no other)
