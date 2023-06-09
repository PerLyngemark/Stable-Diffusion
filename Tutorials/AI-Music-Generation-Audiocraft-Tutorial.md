# Tutorial Video Link > coming soon

[![image](https://img.shields.io/discord/772774097734074388?label=Discord&logo=discord)](https://discord.com/servers/software-engineering-courses-secourses-772774097734074388) [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FFurkanGozukara%2FStable-Diffusion%2Fedit%2Fmain%2FTutorials%2FAI-Music-Generation-Audiocraft-Tutorial.md&count_bg=%2379C83D&title_bg=%239E0F0F&icon=apachespark.svg&icon_color=%23E7E7E7&title=views&edge_flat=false)](https://hits.seeyoufarm.com) [![Twitter Follow](https://img.shields.io/twitter/follow/GozukaraFurkan?label=Follow&style=social)](https://twitter.com/GozukaraFurkan) [![YouTube Channel](https://img.shields.io/badge/YouTube-Channel-red?style=for-the-badge&logo=youtube)](https://www.youtube.com/SECourses) [![Patreon](https://img.shields.io/badge/Patreon-Support%20Me-f96854?style=for-the-badge&logo=patreon)](https://www.patreon.com/your_patreon_page)

## Colab
Google Colab Link Works with GPU for free : https://colab.research.google.com/drive/1fxGqfg96RBUvGxZ1XXN07s3DthrKUl4-?usp=sharing

## Example Resources and More Help
**Auto install and run scripts : https://www.patreon.com/posts/ai-music-auto-84334460**

Stable Diffusion tutorials : https://github.com/FurkanGozukara/Stable-Diffusion

## Prerequisites

### Step 1 : Python

**Full tutorial for python and git installation with venv**

https://youtu.be/B5U7LJOvH6g

**Download and install Python 3.10.x and git**

https://www.python.org/ftp/python/3.10.9/python-3.10.9-amd64.exe

https://git-scm.com/downloads

## Installation

Repo url : https://github.com/facebookresearch/audiocraft

Enter inside the drive or folder where you want to install

Open cmd type 
```
git clone https://github.com/facebookresearch/audiocraft
```

Move into cloned folder

```
cd audiocraft
```

Lets say you wan't to use the same version that I have used in the tutorial video at this moment execute below commit checkout

```
git checkout 0c75a46321e6e4b15b1e6c751d9c69ff9cbdda69
```

Make a new venv with the below command

```
python -m venv venv
```

Enter incide venv - scripts and activate

```
cd venv
cd scripts
activate
```

Install Torch 2 and gradio with below command

```
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```

Return back into main folder with below command and execute install requirements

```
cd..
cd..
pip install -e .
```

Then we reinstall xformers and we install gradio
```
pip uninstall -y xformers
pip install xformers
pip install gradio
```

Then we are ready to start the application. Whenever you start the application you need to activate venv. For activating venv open a new cmd window in cloned repo, execute below command and it will work
```
call .\venv\Scripts\activate.bat
python app.py
```

My venv installed libraries full list. obtained via ```pip freeze```

My python is 3.10.9

```
aiofiles==23.1.0
aiohttp==3.8.4
aiosignal==1.3.1
altair==5.0.1
antlr4-python3-runtime==4.9.3
anyio==3.7.0
appdirs==1.4.4
async-timeout==4.0.2
attrs==23.1.0
-e git+https://github.com/facebookresearch/audiocraft@0c75a46321e6e4b15b1e6c751d9c69ff9cbdda69#egg=audiocraft
audioread==3.0.0
av==10.0.0
blis==0.7.9
catalogue==2.0.8
certifi==2022.12.7
cffi==1.15.1
charset-normalizer==2.1.1
click==8.1.3
cloudpickle==2.2.1
colorama==0.4.6
colorlog==6.7.0
confection==0.0.4
contourpy==1.0.7
cycler==0.11.0
cymem==2.0.7
Cython==0.29.35
decorator==5.1.1
demucs==4.0.0
diffq==0.2.4
docopt==0.6.2
dora-search==0.1.12
einops==0.6.1
exceptiongroup==1.1.1
fastapi==0.96.0
ffmpy==0.3.0
filelock==3.9.0
flashy==0.0.2
fonttools==4.39.4
frozenlist==1.3.3
fsspec==2023.6.0
gradio==3.34.0
gradio_client==0.2.6
h11==0.14.0
httpcore==0.17.2
httpx==0.24.1
huggingface-hub==0.15.1
hydra-colorlog==1.2.0
hydra-core==1.3.2
idna==3.4
Jinja2==3.1.2
joblib==1.2.0
jsonschema==4.17.3
julius==0.2.7
kiwisolver==1.4.4
lameenc==1.4.2
langcodes==3.3.0
lazy_loader==0.2
librosa==0.10.0.post2
linkify-it-py==2.0.2
llvmlite==0.40.1rc1
markdown-it-py==2.2.0
MarkupSafe==2.1.2
matplotlib==3.7.1
mdit-py-plugins==0.3.3
mdurl==0.1.2
mpmath==1.2.1
msgpack==1.0.5
multidict==6.0.4
murmurhash==1.0.9
mypy-extensions==1.0.0
networkx==3.0
num2words==0.5.12
numba==0.57.0
numpy==1.24.1
omegaconf==2.3.0
openunmix==1.2.1
orjson==3.9.1
packaging==23.1
pandas==2.0.2
pathy==0.10.1
Pillow==9.3.0
pooch==1.6.0
preshed==3.0.8
pycparser==2.21
pydantic==1.10.9
pydub==0.25.1
Pygments==2.15.1
pyparsing==3.0.9
pyre-extensions==0.0.29
pyrsistent==0.19.3
python-dateutil==2.8.2
python-multipart==0.0.6
pytz==2023.3
PyYAML==6.0
regex==2023.6.3
requests==2.28.1
retrying==1.3.4
safetensors==0.3.1
scikit-learn==1.2.2
scipy==1.10.1
semantic-version==2.10.0
sentencepiece==0.1.99
six==1.16.0
smart-open==6.3.0
sniffio==1.3.0
soundfile==0.12.1
soxr==0.3.5
spacy==3.5.2
spacy-legacy==3.0.12
spacy-loggers==1.0.4
srsly==2.4.6
starlette==0.27.0
submitit==1.4.5
sympy==1.11.1
thinc==8.1.10
threadpoolctl==3.1.0
tokenizers==0.13.3
toolz==0.12.0
torch==2.0.1+cu118
torchaudio==2.0.2+cu118
torchvision==0.15.2+cu118
tqdm==4.65.0
transformers==4.30.1
treetable==0.2.5
typer==0.7.0
typing-inspect==0.9.0
typing_extensions==4.4.0
tzdata==2023.3
uc-micro-py==1.0.2
urllib3==1.26.13
uvicorn==0.22.0
wasabi==1.1.2
websockets==11.0.3
xformers==0.0.20
yarl==1.9.2
```