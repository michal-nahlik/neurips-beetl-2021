# NeurIPS 2021 BEETL Competition
## Benchmarks for EEG Transfer Learning
https://beetl.ai/

### Training and submission notebooks
Leaderboard testing phase<br>
Sleep: [src/leaderboard/beetl_sleep_mixup_vat.ipynb](/src/leaderboard/beetl_sleep_mixup_vat.ipynb)<br>

Final scoring phase<br>
Sleep: [src/final/beetl_sleep_mixup_vat_v3.ipynb](/src/final/beetl_sleep_mixup_vat_v3.ipynb)<br>
Motor imagery: [src/final/beetl_mi_mixup_vat.ipynb](/src/final/beetl_mi_mixup_vat.ipynb)<br>

### Report
Report: [doc/neurips-beetl-2021.pdf](/doc/neurips-beetl-2021.pdf)<br>

### Output from notebook runs
Leaderboard testing phase sleep: [output/leaderboard/2021-09-29-18-58-sleep-mixup_vat_v2.zip](/output/leaderboard/2021-09-29-18-58-sleep-mixup_vat_v2.zip)<br>
Final scoring phase sleep: [output/final/2021-10-01-17-09-sleep-mixup_vat_v3.zip](/output/final/2021-10-01-17-09-sleep-mixup_vat_v3.zip)<br>
Final scoring motor imagery: [output/final/2021-09-30-15-01-mi-mixup_vat.zip](/output/final/2021-09-30-15-01-mi-mixup_vat.zip)<br>

Output content:
- model states from different stages of training (best_model...pt)
- target and test outputs from different stages (...-target_output.npy, ...-test_output.npy)
- copy of notebook that generated the output (notebook_run.ipynb)
- submission (answer.txt)

### Reproducibility
Notebooks were run on Google Colab with Tesla K80 GPU, NVIDIA-SMI 470.63.01, Driver Version: 460.32.03, CUDA Version: 11.2 and PyTorch 1.9.0+cu102. <br>

To rerun the notebooks change:
- GDRIVE_DATA_FOLDER to folder where zipped competition data are located on your gdrive
- GDRIVE_OUTPUT_FOLDER to folder where the run output will be saved after it's done

Expected files for Sleep and Motor imagery:
- Sleep: SleepSource.zip, LeaderboardSleep.zip, finalSleep.zip
- Motor imagery: leaderboardMI.zip, finalMI.zip

### TODO
- fix readme
- clean up and add code of other approaches