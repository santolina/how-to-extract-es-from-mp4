# how-to-extract-es-from-mp4
Describe how we can extract elemental streams from MP4 as follows:

## Step.1
- idenfity which es is included in mp4
- $ffmpeg -i input.mp4

## Step.2 
### extract video es
- $ffmpeg -i input.mp4 -vcodec copy cn:video.extn
- extn is like h265, h264 etc...

### extract audio es
- $ffmpeg -i input.mp4 -acodec copy vn:audio.extn
- extn is like aac etc...

## Referneces
- https://e2e.ti.com/support/embedded/linux/f/354/t/156646
