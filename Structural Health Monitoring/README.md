The project uses Dataset available on kaggle 

https://www.kaggle.com/datasets/programmer3/aging-bridge-shm-time-series-dataset

📌 Project Overview

This project applies Machine Learning techniques for Structural Health Monitoring by analyzing acceleration data from structures like bdridges. The main goal is to detect whether a structure is in a Normal or Not Normal (Damaged/Abnormal) state using statistical features and classification models.

Key highlights:

Computed Root Mean Square (RMS) of acceleration signals over short and long windows.

Used Z-score analysis for feature standardization and anomaly detection.

Designed a fuzzy membership system to handle ambiguous cases.

Trained an SVM classifier with fuzzy membership weights to classify structural states.

⚙️ Features Extracted

Acceleration Magnitude (acc_mag)

Short-term RMS (rms_short) – captures local vibration patterns

Long-term RMS (rms_long) – captures global structural behavior

Z-score normalization – to identify abnormal deviations

🧮 Methodology

Preprocessing:

Computed acceleration magnitude from sensor signals.

Applied rolling windows (8 samples for short RMS, larger for long RMS).

Feature Engineering:

Extracted RMS and z-scores.

Designed fuzzy membership rules:

Normal (close to 0 deviation).

Not Normal (large deviations).

Ambiguous states (between thresholds).

Classification:

Trained SVM (Support Vector Machine) model.

Applied fuzzy membership weights during training.

