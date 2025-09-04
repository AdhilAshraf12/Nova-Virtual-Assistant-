# Nova-Virtual-Assistant-
Nova is a personal assistant developed by me because I love Iron Man and wanted to make my own.


If youre on MacOS please use the following to setup Nova:

# 1) Python env
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt

# 2) Ollama (model host)
brew install --cask ollama
ollama pull llama3:8b

# 3) Piper + espeak-ng
brew install piper-tts espeak-ng

# 4) Voices (pick one; store in nova/voices/)
# Example: en-us-libritts-high
mkdir -p voices
# Download the .onnx voice from Piper releases and place under voices/


If youre on WindowsOS use this:

# 1) Python env
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt

# 2) Ollama
# Download & install from https://ollama.com/download
ollama pull llama3:8b

# 3) Piper
# Download piper_windows_x64.zip from Piper releases.
# Extract to nova\piper\ (so the exe is nova\piper\piper.exe)
# Put your voice .onnx into nova\voices\
