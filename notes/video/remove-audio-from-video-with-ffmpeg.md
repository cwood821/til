# Remove audio from video with ffmpeg `-an` option

If you have a video that does not need sound, like a background video on a web page, you can remove the sound with ffmpeg and the `-an` flag. This will help reduce file size.

```bash
ffmpeg -i [input_file] -vcodec copy -an [output_file]
```

From the documentation: 
> The presence of -an disables audio stream selection

See on [Stackoverflow](https://superuser.com/questions/268985/remove-audio-from-video-file-with-ffmpeg#268986) and [official documentation](https://ffmpeg.org/ffmpeg.html#Audio-Options).

You can also output audio and video separately:

```
ffmpeg -i input.mp4 -map 0:0 -c:v copy only_video.mp4
ffmpeg -i input.mp4 -map 0:1 -c:a copy only_audio.mp4
```
This snippet from [Stack overflow](https://stackoverflow.com/questions/32703344/does-removing-audio-from-a-video-file-reduce-its-size#32703391)

