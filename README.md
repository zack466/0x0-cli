# A simple 0x0 CLI written in Python

## Introduction

This is a simple command-line interface to upload files to [0x0.st](https://0x0.st), with support for deleting files that you have uploaded.
To use, download the script `0x0` and then make it executable with `chmod +x 0x0`.
It may be helpful to then move this script into a folder in your PATH.

This script requires an installation of Python 3, accessible with `python3`.
Note that it will create an file to store 0x0 tokens in your home directory (default location `~/.local/share/0x0/entries.json`).
If you want to change where the entries file is stored or the 0x0 URL, modify the constants at the top of `0x0`.

## Usage

```
# upload a file
0x0 some_file.txt

# upload a file from a remote URL (must start with 'http://' or 'https://')
0x0 http://file_url

# upload a file that expires in 24 hours
0x0 -e 24 some_file.txt

# view all uploaded files
0x0 -l

# view info for a specific uploaded file
0x0 -l some_file.txt

# delete an uploaded file
0x0 -d some_file.txt
```
