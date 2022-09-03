# AMD Optimal Settings
First of all, for output we're gonna use the `Advanced` Output Mode.</br>

# Streaming
[TL;DR Jump](#tldr-streaming)</br>
In the streaming tab, select the `AMD HW H.264` encoder.
Change the `Rate Control` to `CBR`, set `Keyframe Interval` to `2s`, change the `Preset` to `Quality` or `Balanced` (if your hardware cannot keep up with these presets, choose the `Speed` preset), change `Profile` to `High` and set B-frames to `2`.</br>

## Bitrate
Bitrate is dependent on your streaming service and on your internet, here's a link to the [YouTube](https://support.google.com/youtube/answer/1722171?hl=en) and the [Twitch](https://stream.twitch.tv/encoding/) bitrate guides.

## AMF Options
**====(RX 6000 USERS ONLY)====** </br>
Final options: `BReferenceEnable=1 BPicturesPattern=1 MaxConsecutiveBPictures=1 HighMotionQualityBoostEnable=1` (options are separated by spaces).

## TL;DR (Streaming)
<img src="https://github.com/TorniX0/optimal-obs-settings/raw/main/docs/AMD_STR1.PNG"> 

</br>

# Recording (H.264)
[TL;DR Jump](#h264-tldr-recording)</br>
In the recording tab, select the `AMD HW H.264` encoder.
Change the `Rate Control` to `CQP`, set keyframe interval to `1s`, change the `Preset` to `Speed` and change `Profile` to `High`.

## CQ Level
CQ Level determines the overall quality and file-size of the video, it can range from 1 (the best quality, and the highest file-size) to 51 (the worst quality, and the smallest file-size).</br></br>
I would recommend the following values:</br></br>
**Near Lossless** => 1-5;</br>
**Indistinguishable** => 6-13;</br>
**High Quality** => 14-16;</br>
**Tolerable Quality** => 17-23;</br>

# H.264 TL;DR (Recording)
<img src="https://github.com/TorniX0/optimal-obs-settings/raw/main/docs/AMD_REC1.PNG">

</br>

# Recording (HEVC)
[TL;DR Jump](#hevc-tldr-recording)</br>
In the recording tab, select the `AMD HW H.265` encoder.
Change the `Rate Control` to `CQP`, set keyframe interval to `1s` and change the `Preset` to `Speed`.

## HEVC TL;DR (Recording)
<img src="https://github.com/TorniX0/optimal-obs-settings/raw/main/docs/AMD_REC2.PNG"> 

</br>
