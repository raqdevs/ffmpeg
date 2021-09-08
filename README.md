# ffmpeg
Estudos e casos de uso ffmpeg

## extract audio wav.bat
Extrair arquivo de audio .wav de um video no formato .mp4, funciona em outros formatos de videos (importante ler a documentação do ffmpeg para ver os formatos suportados)
```
ffmpeg -i input.mp4 -vn -acodec pcm_s16le -ar 44100 -ac 2 output.wav
pause
```

## weba to wav.bat
Converter arquivos.weba para wav (serve também para outros formatos de exportação em vez de .wav pode-se utilizar .mp3), nesse caso foi utilizado o audio de videos do YouTube
_
```
ffmpeg -i videoplayback.weba -vn -acodec pcm_s16le -ar 44100 -ac 2 output.wav
pause
```

Para acessar o audio do video do youtube em exemplo rápido seria:
1. Abra o video no youtube no navegador em um computador
2. Aperte f12 no teclado ou botão direito e inspecionar 
3. Cole o código abaixo na aba Console, aperte Enter
```
ytplayer.config.args.raw_player_response.streamingData.adaptiveFormats.pop().url
```
