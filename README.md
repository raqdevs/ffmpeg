# ffmpeg
Estudos e casos de uso ffmpeg

* extract audio wav.bat, extrair arquivo de audio .wav de um video no formato .mp4, funciona em outros formatos de videos (importante ler a documentação do ffmpeg para ver os formatos suportados)
```
ffmpeg -i input.mp4 -vn -acodec pcm_s16le -ar 44100 -ac 2 output.wav
pause
```
