# Advanced Settings

## Color Fornat
Format | Hardware-accelerated | Bit-depth | Chroma Subsampling | Details
:---: | :---: | :---: | :---: | :---:
`NV12` | Yes | 8-bit | 4:2:0 | Same as `I420`, but stored differently in memory in order to provide better performance for GPU(s)
`I420` | Yes | 8-bit | 4:2:0 | Decent color quality, easiest to process
`I444` | Yes | 8-bit | 4:4:4 | Good color quality, but harder to process
`P010` | Yes | 10-bit | 4:2:0  | Same as `NV12` but more bit depth
`I010` | Yes | 10-bit | 4:2:0  | Same as `I420` but more bit depth
`BGRA` | No | 8-bit | - | Best color quality, hardest to process (not usually supported in consumer video formats)

*Choose based on your personal needs*.</br>

----
## Color Space

If you want to record your computer screen (games, desktop, etc..) use `sRGB`, otherwise use `Rec. 709`.

If you want to use HDR and record your computer screen (games, desktop, etc..) use `Rec. 2100 (HLG)` (way more support than `PQ`)

----
## Color Range
Set it to `Full`, though if you have any issues with your editing software displaying out weird colors while the video seems fine when playing it back, use `Partial`.
