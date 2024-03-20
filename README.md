# RVC-TTS-Pipeline

RVC를 이용한 voice-conversion pipeline 이다.

Retrieval-based-Voice-Conversion-WebUI
를 응용한
https://github.com/JarodMica/rvc-tts-pipeline
에서

API로 쓰기 좋게 변형하기 위해 만들었다.

## Installation

1. Install pytorch first here: https://pytorch.org/get-started/locally/

1.

```
pip install -e git+https://github.com/cksghkd123/rvc.git#egg=rvc
```

2.

```
pip install -e git+https://github.com/cksghkd123/rvc-tts-pipeline.git#egg=rvc_tts_pipe
```

3. `hubert_base.pt` 와 `rmvpe.pt` 모델을 따로 설치할 필요가 있다.

4. import `rvc_infer`

## Basic usage

```
from rvc_infer import rvc_convert

rvc_convert(model_path="your_model.pth", input_path=input_file_path, output_file_name=file_name)
```
