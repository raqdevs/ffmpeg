# ffmpeg
Estudos e casos de uso ffmpeg

## Salve como .bat 

* ## extract audio wav.bat
```
ffmpeg -i input.mp4 -vn -acodec pcm_s16le -ar 44100 -ac 2 output.wav
pause
```
