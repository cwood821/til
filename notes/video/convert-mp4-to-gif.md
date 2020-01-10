# Convert mp4 to gif to with `ffmpeg` 

With ffmpeg, convert an mp4 to gif with:

```
ffmpeg -i some.mp4 -vf "fps=30,scale=720:-1:flags=lanczos,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse" -loop 0 some.gif
```

See documentation on [flags](https://ffmpeg.org/ffmpeg.html).
