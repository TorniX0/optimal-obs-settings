# Video Settings
If you want to record at the **native resolution** of your monitor, set both boxes to the biggest dropdown value.</br>
`Base (Canvas) Resolution` represents the "scene" resolution.</br>
`Output (Scaled) Resolution` represents the final video resolution (must be lower or equal to the `Base Resolution`).

## Downscale Filter
Filter | Samples | Details
:---: | :---: | :---:
`Billinear` | 1 | Fastest, but blurry if scaling
`Area` | 4/6/9 | Fast, but has decent scaling
`Bicubic` | 16 | Slow, but has good scaling
`Lanczos` | 36 | Slowest, but has the best scaling

*Choose depending on your needs*.</br>

## FPS
Use `Common FPS Values`, and choose `60 FPS` (if your computer **cannot** handle `60 FPS`, find a sweet spot that works for you, or decrease the encoding quality).
