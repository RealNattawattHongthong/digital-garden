---
title: YouTube Downloader using Python
---
```py
from pytube import YouTube
import os

def download_video(url):
    try:
        yt = YouTube(url)
        # Filter streams for mp4 format
        stream = yt.streams.filter(file_extension='mp4').first()
        if stream:
            print("Downloading...")
            stream.download()
            print("Download complete!")
        else:
            print("No MP4 format available for this video.")
    except Exception as e:
        print("Error:", str(e))

if __name__ == "__main__":
    video_url = input("Enter the YouTube video URL: ")
    download_video(video_url)

```
This one work! Or should work [[knowledge]]