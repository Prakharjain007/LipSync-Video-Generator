# Wav2Lip Lip Sync Code

This code allows you to synchronize an audio track with a video of a person speaking, creating a lip-synced video.

## Prerequisites

- Google Colab account (for running this code in a Colab environment)
- Python 3.x

## Setup

1. Clone the Wav2Lip repository and navigate to the appropriate directory:

   ```shell
   !git clone https://github.com/justinjohn0306/Wav2Lip

2. Download the pre-trained models:

   ```shell
   !wget 'https://github.com/justinjohn0306/Wav2Lip/releases/download/models/wav2lip.pth' -O 'checkpoints/wav2lip.pth'
   !wget 'https://github.com/justinjohn0306/Wav2Lip/releases/download/models/wav2lip_gan.pth' -O 'checkpoints/wav2lip_gan.pth'
   !wget 'https://github.com/justinjohn0306/Wav2Lip/releases/download/models/resnet50.pth' -O 'checkpoints/resnet50.pth'
   !wget 'https://github.com/justinjohn0306/Wav2Lip/releases/download/models/mobilenet.pth' -O 'checkpoints/mobilenet.pth'


3. Install required packages:

   ```shell
   !pip install https://raw.githubusercontent.com/AwaleSajil/ghc/master/ghc-1.0-py3-none-any.whl
   !pip install git+https://github.com/elliottzheng/batch-face.git@master
   !pip install ffmpeg-python mediapipe==0.8.11
   !pip install yt-dlp

## Usage

To use the Wav2Lip Lip Sync tool, follow these steps:

1. Provide the YouTube video URL from which you want to extract the audio.

2. Trim the video by specifying the start and end times to ensure there's a face in all frames.

3. Select your audio source (record, upload from a local drive, or Google Drive).

4. Configure optional parameters for video processing (e.g., padding, smoothing, model selection).

5. Run the code, and the lip-synced video will be generated.

## Example

Here's an example of how to use the Wav2Lip Lip Sync tool in a Colab notebook:

## Output

The lip-synced video will be saved as results/result_voice.mp4. You can download it from the Colab environment.
