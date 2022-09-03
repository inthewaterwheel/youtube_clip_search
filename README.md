### Youtube CLIP Search

These notebooks are messy and deserve some cleaning up, use at your own peril.

What it does:

- Use `pytube` to download all videos from a channel matching some conditions
- Use `FFMPEG` to capture a frame from the video every two seconds
- Use OpenAI CLIP to embed the images
- Use OpenAI CLIP to embed a text string, or also CLIP embed another image to search by.
- Find the closest 36 matches, and save them.

### Notes

- Runtime is dominated by the download, everything else is rather fast! You should be able to quite easily adapt this to searching other videos.

- I used a GPU to do this, and the code assumes that, but given how fast embedding was, maybe a CPU will suffice?
