# Remove Hiss from Videos

## Introduction
Have you ever found a Youtube video that is really good but has horrible background hiss?

Once you have downloaded the video using youtube-dl or the downloader of your choice

This script listens to the first 0.5 seconds of the clip and build a noise profile which will then be used to generate a video file with clean audio.

I made this script for myself as I found some great Python tutorial but had bad audio hiss in them.

## Requirements

- Linux system with the following packages installed

    - ```ffmpeg```
    - ```sox```

    For Ubuntu based distro's run ``` sudo apt install ffmpeg sox```

    vacleanup (Video Audio Cleanup) needs to be executeable (```sudo chmod +x vacleanup```)

## Usage

With your video downloaded, run ```./vacleanup FILENAME.webm```

The cleaned up version will be saved into a folder called ```cleaned``` with the original filename.