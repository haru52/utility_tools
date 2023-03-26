# flac2mp3.py

## Overview

FLACオーディオファイルをMP3 320kbps CBRに変換するスクリプトです．  
変換前FLACファイルのメタデータを保持したMP3ファイルを生成します．  
また，変換前のディレクトリ構造を出力先に保持します．

## Description

- 出力先に同名のファイルが既に存在する場合，エンコードしない
- FFmpegはLAMEライブラリを用いてFLACをMP3にエンコード

## Requirements

- Python 3.6.2 or later
  - Click (Python library) 6.7 or later（pipやcondaでインストール可能）
- FFmpeg 4.0.1 or later

## Usage

```console
Usage: flac2mp3 [OPTIONS] INPUT_DIRECTORY_PATH [OUTPUT_DIRECTORY_PATH]

  Encode FLAC audio files into MP3 320kbps CBR files

Options:
  -h, --help  Show this message and exit.
```

[OUTPUT_DIRECTORY_PATH]を省略した場合，カレントディレクトリを出力先に設定

## License

[MIT License](LICENSE)

## Author

[haru](https://haru52.com/)
