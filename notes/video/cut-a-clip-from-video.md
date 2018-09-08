# Cut a clip from a video with ffmpeg

To trim a video with ffmpeg without re-encoding (and affecting quality), use the this snippet:

```
ffmpeg -i in-file.mp4 -t 00:00:05 -c copy out-file.mp4
```

The `-c copy` flag will copy data without re-encoding.


See this [Stack Overflow post](https://superuser.com/questions/377343/cut-part-from-video-file-from-start-position-to-end-position-with-ffmpeg) for other variations, including re-encoding. Also, see the [official documentation](https://ffmpeg.org/ffmpeg.html#Main-options).

