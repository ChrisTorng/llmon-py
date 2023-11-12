# llmon-:pie:

cli llm chat with speech-to-text and text-to-speech support


uses llama-cpp-python, coqui.ai and pywhispercpp

its dope, but a wip.

# Additional

Add `.gitignore`.

Modify `llmon.py`:
```
self.speech_tt_model = Model('small')
```
Make `voices` folder, move artbell.wav into it.

Make `models` directory, download any GGUF file into it.

[llama-cpp-python - Installation with Hardware Acceleration](https://github.com/abetlen/llama-cpp-python#installation-with-hardware-acceleration)

```
pip -m venv .venv
.venv\Scripts\activate
set CMAKE_ARGS=-DLLAMA_CUBLAS=on
pip install -r requirements.txt
```

Manual install:
```
pip install llama-cpp-python
# pip install llama-cpp-python --force-reinstall --upgrade --no-cache-dir
pip install numpy==1.24.3
```

Run:
```
python llmon.py
```