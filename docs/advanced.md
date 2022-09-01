# Advanced Settings
Let's dig into the Advanced settings! (they might sound scary, but they aren't)</br></br>

## Process Priority
I would just set this to something like `Above Normal` or `High`.

## Color Fornat
**NV12** => 8-bit, 4:2:0 (least accurate colors, fastest, usually default)</br>
**I420** => 8-bit, 4:2:0</br>
**I444** => 8-bit, 4:4:4 (most accurate colors, slowest)</br>
**P010** => 10-bit, 4:2:0</br>
**I010** => 10-bit, 4:2:0</br>
**RGB** => 8-bit (not hardware accelerated, usually not supported in consumer video formats)</br>
</br>
Choose accordingly.</br>

## Color Space (SDR / Standard)
For an SDR recording, use `sRGB`.

## Color Range
Set it to the `Full` value.
