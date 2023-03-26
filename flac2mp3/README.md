# flac2mp3 (FLAC to MP3)

## Overview

FLAC オーディオファイルを MP3 320kbps CBR に変換するスクリプトです。このスクリプトは変換前 FLAC ファイルのメタデータを保持した MP3 ファイルを生成します。また、変換前のディレクトリ構造も出力先に保持します。

## Requirements

| Tool                                        | Version |
| ------------------------------------------- | ------- |
| Python                                      | ^3.11.1 |
| [Click](https://click.palletsprojects.com/) | ^8.1.3  |
| FFmpeg                                      | ^5.1.2  |

## Installation

```sh
git clone git@github.com:haru52/utility_tools.git
cd utility_tools/flac2mp3
make
```

## Usage

```console
Usage: flac2mp3 [OPTIONS] INPUT_DIRECTORY_PATH [OUTPUT_DIRECTORY_PATH]

  Encode FLAC audio files into MP3 320kbps CBR files

Options:
  -h, --help  Show this message and exit.
```

`[OUTPUT_DIRECTORY_PATH]` を省略した場合、カレントディレクトリを出力先に設定

## Update

```sh
cd path/to/utility_tools
git pull
```

## Description

- 出力先に同名のファイルが既に存在する場合、エンコードしない
- FFmpeg は LAME ライブラリを用いて FLAC を MP3 にエンコード

## License

[MIT](LICENSE)

## Author

[haru](https://haru52.com/)
