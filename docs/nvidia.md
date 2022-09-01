# NVIDIA Optimal Settings
First of all, for output we're gonna use the `Advanced` Output Mode.</br>

# Streaming
[TL;DR Jump](#tldr-streaming)</br>
In the streaming tab, select the `NVIDIA NVENC H.264` encoder.
Change the `Rate Control` to `CBR`, set `Keyframe Interval` to `2`, change the `Preset` to `Quality` or `Max Quality` (if your hardware cannot keep up with these presets, choose the `Performance` or the `Max Performance` preset), change `Profile` to `High`, tick `Look-ahead`, tick `Psycho Visual Tuning` (PVT).</br>

## Bitrate
Bitrate is dependent on your streaming service and on your internet, here's a link to the [YouTube](https://support.google.com/youtube/answer/1722171?hl=en) and the [Twitch](https://stream.twitch.tv/encoding/) bitrate guides.

## Max B-Frames
I recommend setting it to 2-4 depending on what type of game you are playing. If you are playing fast-paced games with a lot of motion, use `2`.

## Explanation
> Why should I use Look-ahead or Psycho Visual Tuning?

First of all, let's define what Look-ahead and Psycho Visual Tuning are.</br>
Psycho Visual Tuning is a function that allows the encoder to optimize the use of bitrate, and increase perceived visual quality, **especially** in situations with **high motion**, at the cost of increased encoding usage.</br>
Look-ahead is a function that indicates the encoder to **analyze a few frames in the future** of the **currently** encoded frame, *(higher values meaning more frames)*, and to allow the encoder to take frame data into account during rate control logic.


Both can be beneficial, especially with streaming.

## TL;DR (Streaming)
<img src="https://github.com/TorniX0/optimal-obs-settings/raw/main/docs/NVIDIA_STR1.PNG"> 

</br>

# Recording (H.264)
[TL;DR Jump](#h264-tldr-recording)</br>
In the recording tab, select the `NVIDIA NVENC H.264` encoder.
Change the `Rate Control` to `CQP`, set keyframe interval to `1s`, change `Preset` to `Max Performance`, change `Profile` to `High`, leave `Look-ahead` and `Psycho Visual Tuning` unticked.

## CQ Level
CQ Level determines the overall quality and file-size of the video, it can range from 1 (the best quality, and the highest file-size) to 51 (the worst quality, and the smallest file-size).</br></br>
I would recommend the following values:</br></br>
**Near Lossless** => 1-5;</br>
**Indistinguishable** => 6-13;</br>
**High Quality** => 14-16;</br>
**Tolerable Quality** => 17-23;</br>

# H.264 TL;DR (Recording)
<img src="https://github.com/TorniX0/optimal-obs-settings/raw/main/docs/NVIDIA_REC1.PNG">

</br>

# Recording (HEVC)
[TL;DR Jump](#hevc-tldr-recording)</br>
In the recording tab, select the `NVIDIA NVENC HEVC` encoder.
The settings are the same on `HEVC` except the `Profile` which should be set to `Main`.

## HEVC TL;DR (Recording)
<img src="https://github.com/TorniX0/optimal-obs-settings/raw/main/docs/NVIDIA_REC2.PNG"> 

</br>
