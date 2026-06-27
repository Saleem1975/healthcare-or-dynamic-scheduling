# Data Notes

This repository does not include raw laparoscopic videos or patient-level clinical data.

The original study used laparoscopic cholecystectomy videos to train and evaluate a CNN-based model for detecting the end of Gallbladder Dissection Phase 4 and supporting dynamic operating room scheduling.

## Included sample files

### `sample_schedule_data.csv`
A small schedule-comparison dataset recreated from the reported schedule tables in the paper. It includes:

- Operation number
- Actual operation time
- Patient waiting time under traditional static scheduling
- Patient waiting time under CNN-based dynamic scheduling
- Operating room idle time under traditional static scheduling
- Operating room idle time under CNN-based dynamic scheduling

This file is intended for GitHub demonstration, chart reproduction, and portfolio documentation.

### `sample_phase4_prediction_results.csv`
A small summary of the reported Phase 4 prediction results across the ten test surgeries, including actual Phase 4 ending time, predicted Phase 4 ending time, absolute error in seconds, and absolute error percentage.

## Privacy and data-sharing statement

Raw laparoscopic videos are not included due to clinical, privacy, and data-sharing restrictions. The repository is prepared for educational, research, and portfolio demonstration purposes only.
