## Introduction
DiffSynth Studio is a diffusion engine. We have restructured architectures, including Text Encoder, UNet, and VAE, among others, maintaining compatibility with models from the open-source community while enhancing computational performance. We offer many interesting features. Enjoy the magic of diffusion models!

## Installation
```
git clone https://github.com/Agoooy/AI-Video/
cd DiffSynth-Studio
pip install -e .
```

## Usage (in Python code)
The Python examples are in [`examples`](./examples/). We provide an overview here.

### Long Video Synthesis
We trained an extended video synthesis model, which can generate 128 frames. [`examples/ExVideo`](./examples/ExVideo/)

https://github.com/modelscope/DiffSynth-Studio/assets/35051019/d97f6aa9-8064-4b5b-9d49-ed6001bb9acc

### Image Synthesis
Generate high-resolution images, by breaking the limitation of diffusion models! [`examples/image_synthesis`](./examples/image_synthesis/)

|512*512|1024*1024|2048*2048|4096*4096|
|-|-|-|-|
|![512](https://github.com/Artiprocher/DiffSynth-Studio/assets/35051019/55f679e9-7445-4605-9315-302e93d11370)|![1024](https://github.com/Artiprocher/DiffSynth-Studio/assets/35051019/6fc84611-8da6-4a1f-8fee-9a34eba3b4a5)|![2048](https://github.com/Artiprocher/DiffSynth-Studio/assets/35051019/9087a73c-9164-4c58-b2a0-effc694143fb)|![4096](https://github.com/Artiprocher/DiffSynth-Studio/assets/35051019/edee9e71-fc39-4d1c-9ca9-fa52002c67ac)|

|1024*1024|2048*2048|
|-|-|
|![1024](https://github.com/Artiprocher/DiffSynth-Studio/assets/35051019/67687748-e738-438c-aee5-96096f09ac90)|![2048](https://github.com/Artiprocher/DiffSynth-Studio/assets/35051019/584186bc-9855-4140-878e-99541f9a757f)|

### Toon Shading
Render realistic videos in a flatten style and enable video editing features. [`examples/Diffutoon`](./examples/Diffutoon/)

https://github.com/Artiprocher/DiffSynth-Studio/assets/35051019/b54c05c5-d747-4709-be5e-b39af82404dd

https://github.com/Artiprocher/DiffSynth-Studio/assets/35051019/20528af5-5100-474a-8cdc-440b9efdd86c

### Video Stylization
Video stylization without video models. [`examples/diffsynth`](./examples/diffsynth/)

https://github.com/Artiprocher/DiffSynth-Studio/assets/35051019/59fb2f7b-8de0-4481-b79f-0c3a7361a1ea

### Chinese Models
Use Hunyuan-DiT to generate images with Chinese prompts. We also support LoRA fine-tuning of this model. [`examples/hunyuan_dit`](./examples/hunyuan_dit/)

Prompt: 少女手捧鲜花，坐在公园的长椅上，夕阳的余晖洒在少女的脸庞，整个画面充满诗意的美感

|1024x1024|2048x2048 (highres-fix)|
|-|-|
|![image_1024](https://github.com/Artiprocher/DiffSynth-Studio/assets/35051019/2b6528cf-a229-46e9-b7dd-4a9475b07308)|![image_2048](https://github.com/Artiprocher/DiffSynth-Studio/assets/35051019/11d264ec-966b-45c9-9804-74b60428b866)|

Prompt: 一只小狗蹦蹦跳跳，周围是姹紫嫣红的鲜花，远处是山脉

|Without LoRA|With LoRA|
|-|-|
|![image_without_lora](https://github.com/Artiprocher/DiffSynth-Studio/assets/35051019/1aa21de5-a992-4b66-b14f-caa44e08876e)|![image_with_lora](https://github.com/Artiprocher/DiffSynth-Studio/assets/35051019/83a0a41a-691f-4610-8e7b-d8e17c50a282)|

## Usage (in WebUI)
```
python -m streamlit run DiffSynth_Studio.py
```

https://github.com/Artiprocher/DiffSynth-Studio/assets/35051019/93085557-73f3-4eee-a205-9829591ef954
