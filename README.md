# Optimizing Efficiency and Visual-Textual Alignment for LLM-Based Radiology Report Generation

## Introduction
![overview](https://github.com/zailongchen/R2Gen-EVA/blob/main/images/frame.png?raw=true)

## Getting Started
### Installation

**1. Prepare the code and the environment**

Git clone our repository and install the requirements.

```bash
https://github.com/zailongchen/R2Gen-EVA.git
cd R2Gen-EVA
pip install -r requirements.txt
```


**2. Prepare the training dataset**

IU-xray: download the dataset from [here](https://drive.google.com/file/d/1c0BXEuDy8Cmm2jfN0YYGkQxFZd2ZIoLg/view)

Mimic-cxr: you can download our preprocess annotation file from [here](https://drive.google.com/file/d/14689ztodTtrQJYs--ihB_hgsPMMNHX-H/view?usp=sharing) and download the images from [official website](https://physionet.org/content/mimic-cxr-jpg/2.0.0/)

After downloading the data, place it in the ./data folder.

### Training

For IU-Xray

```bash
bash scripts/iuxray/r2gen_eva_train.sh
```

For MIMIC-CXR

```bash
bash scripts/mimic/r2gen_eva_train.sh
```

### Testing 

```bash
bash scripts/iuxray/r2gen_eva_test.sh
```

For MIMIC-CXR

```bash
bash scripts/mimic/r2gen_eva_test.sh
```


## Acknowledgement

+ [R2GenGPT](https://github.com/wang-zhanyu/R2GenGPT) This repo is mainly built upon R2GenGPT.
+ [MiniGPT-4](https://github.com/Vision-CAIR/MiniGPT-4) Some codes of this repo are based on MiniGPT-4.
+ [Llama2](https://github.com/facebookresearch/llama) The fantastic language ability of Llama-2 with only 7B parameters is just amazing.


## License
This repository is under [BSD 3-Clause License](LICENSE.md).
