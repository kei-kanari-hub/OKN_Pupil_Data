README for the dataset associated with:

Dataset Version  
Created on: 2025-02-27

Title:
OKN and Pupillary Response Modulation by Gaze and Attention Shifts

Authors:
Kei Kanari & Moe Kikuchi

DOI:
https://doi.org/10.3390/jemr18020011

---

Dataset Overview:

This dataset includes measurements of optokinetic nystagmus (OKN) and pupil responses collected under two conditions:
1. Gaze shift condition (overt attention)
2. Attention shift condition (covert attention)

The dataset is organized into the following structure:

- OKN/
  ├── att/
  │   ├── att_LL.csv
  │   ├── att_LR.csv
  │   ├── att_RL.csv
  │   └── att_RR.csv
  └── gaze/
      ├── gaze_LL.csv
      ├── gaze_LR.csv
      ├── gaze_RL.csv
      └── gaze_RR.csv

- Pupil/
  ├── att/
  │   ├── att_BB.csv
  │   ├── att_BW.csv
  │   ├── att_WB.csv
  │   └── att_WW.csv
  └── gaze/
      ├── gaze_BB.csv
      ├── gaze_BW.csv
      ├── gaze_WB.csv
      └── gaze_WW.csv

- latency.csv

---

File Naming Convention:

- For OKN data:
  Each file is named as either `gaze_XX.csv` or `att_XX.csv`, where:
    - The prefix `gaze_` indicates the overt gaze shift condition.
    - The prefix `att_` indicates the covert attention shift condition.
    - `LL`: left-to-left motion
    - `LR`: left-to-right motion
    - `RL`: right-to-left motion
    - `RR`: right-to-right motion

- For Pupil data:
  Each file is named similarly, with:
    - `BB`: black-to-black shift
    - `BW`: black-to-white shift
    - `WB`: white-to-black shift
    - `WW`: white-to-white shift

Each CSV file contains time-series data for individual trials, with rows corresponding to time points and columns to participants or trials.

---

latency.csv:

- This file contains the average response latencies (in milliseconds) for each participant under four conditions:
    - OKN attention
    - Pupil attention
    - OKN gaze
    - Pupil gaze

- The first row of `latency.csv` is the header:
  `OKN attention, Pupil attention, OKN gaze, Pupil gaze`

- Each subsequent row corresponds to one participant.

---

Please cite the original publication when using this dataset:

Kanari, K., & Kikuchi, M. (2025). OKN and Pupillary Response Modulation by Gaze and Attention Shifts. Journal of Eye Movement Research, 18(2), Article 11. https://doi.org/10.3390/jemr18020011
