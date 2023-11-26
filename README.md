# 2023_biomedical_exp13
2023 바이오메디컬 시스템 반도체 융합기초설계 13주차 실험 (마이크로프로세서 실험1)

## Requirements, installation
```
sudo apt-get install libatlas-base-dev
sudo apt-get install python3-scipy python3-matplotlib
pip install --upgrade numpy
pip install pandas pywavelets statistics wfdb

wget -r -N -c -np https://physionet.org/files/mitdb/1.0.0/
git clone https://github.com/hsw5781/2022_biomedical_exp14.git
```
**Note:** Please check Raspberry Pi setting manual provided in [this page](https://www.notion.so/seungwoo-hong/Raspberry-Pi-ver-221117-4af98121fb94487a8fa9df09bc6f6b91)

## How to Run
* FFT: `python fft_anaylsy.py`
* ECG sampling & QRS detection: `python qrs_detection.py -p <patient_number> -fs <sampling_freq>`
  * `<patient_number>`: patient id within MIT-BIH dataset
  * `<sampling_freq>`: sampling frequency of ECG signal (lead-II)
