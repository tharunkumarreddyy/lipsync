# lipsync

## Objective

The objective of this project is to demonstrate my skills in creating or using an AI model that is proficient in lip-syncing, i.e. synchronizing an [audio](https://drive.google.com/file/d/1jhUOAeGw8lPjNf7Q1cIcBOvzE3CJ3gVz/view) file with a [video](https://www.youtube.com/watch?v=YMuuEv37s0o) file. My task is to ensure the model is accurately matching the lip movements of the characters in the given [video](https://www.youtube.com/watch?v=YMuuEv37s0o) file with the corresponding [audio](https://drive.google.com/file/d/1jhUOAeGw8lPjNf7Q1cIcBOvzE3CJ3gVz/view) file.

## Model

I will be using the [wav2lip](https://github.com/Rudrabha/Wav2Lip) pre-trained model. This is a deep learning model that has been trained on a large dataset of video and audio files. The model is able to learn the relationship between the lip movements of a person and the corresponding audio. This allows the model to accurately synchronize the audio with the video.

## Approach

At first the [video](https://www.youtube.com/watch?v=YMuuEv37s0o) in context was cropped so that it matches the length of the [audio](https://drive.google.com/file/d/1jhUOAeGw8lPjNf7Q1cIcBOvzE3CJ3gVz/view) provided. After that as the [wav2lip](https://github.com/Rudrabha/Wav2Lip) model works on videos having face in all of it's frames so the video was partitioned into segments of multiple videos some having face in all of it's frames and some having faces in none of it's frames. And accordingly the [audio](https://drive.google.com/file/d/1jhUOAeGw8lPjNf7Q1cIcBOvzE3CJ3gVz/view) was also partitioned in to segments corresponding the time frames of the vdeo segments.

And then [wav2lip](https://github.com/Rudrabha/Wav2Lip) pre-trained model was used to synchronize audio to those segments of videos having faces in all of it's frames and the in case of other segments the audio was replaced.

## Steps to Run

1. Open the [Google Colab](https://colab.research.google.com/drive/1RrJtagpguWYYUqo40KrIF_uzVJFJlzTI?usp=sharing) notebook in this repository.
2. Install all dependencies and pre-trained model by running the setupwav2 cell.
3. If you want to use the video youtube link [you tube](https://www.youtube.com/watch?v=YMuuEv37s0o) that I used, run the block of code named `Downloading the video file`. Otherwise, upload a video file into the sample_data of the repository and rename it to `input_vid.mp4`.
4. start:31
   end:60
   start1:69
   end1:84
   start2:127
   end2:135
   start3:488
   end3:508
5. Run the block of code named `select youtube video`.It will take some 40 minutes of time. Otherwise upload already provided video into the sample_data repository.
6. Run the 'select audio' code.Upload an audio file into the sample_data directory of the repository and rename it to `input_audio.wav`.
7. Run the block of code named `Start crunching and preview output`.
8. Download the result_voice.mp4 from wave2lip/results/


## Result

The resultant video of the project can be viewed [here](https://drive.google.com/file/d/1TYK4HLOFWzCXSMGgCie2i7O2nqh4u7aR/view?usp=sharing)

## Thank You

Thank you for taking the time to view my project. If you have any questions, please feel free to reach out to me at tharunkumarau01@gmail.com.
