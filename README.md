# Llambada-v0.1 🐑 🎵
Welcome to the official implementation of Llambada version 0.1 repository! This project provides the tools and resources to use the Llambada model, an advanced system for music generation.

- Paper: [Arxiv](https://arxiv.org/pdf/2411.01661)

- Demo page: [Llambadad demo](https://songgen-ai.github.io/llambada-demo/)

This model is trained on totally 4.4k music hours dataset with 2xA100 GPUS. The training cost for this model is about 720 USD in 5 days for 2 stages: the semantic stage and the coarse stage.

⭐ Hopefully, we want open the a.i for everyone, so all of the source code of the model, the training script, and the hyperparameters will be released :)

Please note: At this time, the repository includes only the inference code and pre-trained model checkpoint. Training scripts will be added in a future update.

### ☑️ Release checklist

- [x] Model code
- [x] Inference script
- [ ] Checkpoint
- [ ] Training script
- [ ] Gradio inference
- [ ] Model serving
# 🛠️ Installation
Follow the steps below to set up your Python 3.10 environment using Conda and install the required dependencies.

Step 1: Create the environment
```bash
conda env create -f environment.yml
conda activate llambada
```
Step 2: Install dependencies
Install ffmpeg (for ubuntu, the script is here) and the dependencies.
``` bash
apt update && apt install ffmpeg
pip install -r requirements.txt
```
# 🚅 Training (Coming Soon)
Instructions and scripts for training will be provided in a future release.

# 🖥️ Inference
Utilize the pre-trained Llambada model to generate music easily.

## Checkpoint download

All of the checkpoints for semantic stage and the coarse stage can be downloaded in the [HuggingFace of SongGen](https://huggingface.co/songgen/Llambada)

## Running Inference
``` bash
CUDA_LAUNCH_BLOCKING=1 CUDA_VISIBLE_DEVICES=0 python infer.py
```
Create stunning music compositions with Llambada effortlessly!

### Contact

If you have any further questions or having new ideas for the model features, you can raise in the issue or you can contact us in songgen.ai and we can have support in our ability!

### License 

```
Copyright 2025 Songgen.ai

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
