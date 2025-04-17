

# [Deletor](https://pashkov256.github.io/deletor-doc) - Utility for Deleting Files by Extension and Size
[![Go Reference](https://pkg.go.dev/badge/github.com/pashkov256/deletor/v1.svg)](https://pkg.go.dev/github.com/pashkov256/deletor)
![code helpers](https://www.codetriage.com/pashkov256/tcache/badges/users.svg)

**Deletor** is a command-line utility for deleting files based on their extension and size. It allows you to find and delete files in a specified directory that match the given criteria (file extension and minimum size).

## Web docs
 [https://pashkov256.github.io/deletor-doc](https://pashkov256.github.io/deletor-doc)


## Features
- 🗑️ **Delete by Extension**: Deletes files with specified extensions (e.g., .mp4, .zip).

- 📏 **Size Filter**: Deletes only files larger than the specified size (e.g., 10mb, 1gb).

- 📂 **Recursive Search**: Scans the directory and all its subdirectories.

- 🛠️ **Confirmation Prompt**: Asks for confirmation before deleting files.

- 📊 **Table Output**: Displays files in a clean, formatted table with sizes aligned for readability.
## 📦 Installation
```bash
go install github.com/pashkov256/deletor
```

## 🛠 Usage

```bash
deletor -e mp4,zip -d ~/Downloads/ -s 10mb
```

### Arguments:
- `-e, --extensions` - list of file extensions separated by commas (e.g., `mp4,zip,jpg`).
- `-d, --directory` - path to the directory to search for files.
- `-s, --size` - maximum file size (e.g., `10b`,`10kb`,`10mb`,`10gb`).

## 🔥 Example
```bash
deletor -e mp4,zip -d ~/Downloads/ -s 18kb
```
Output:
```bash
2.96 MB    /home/user/Downloads/sample.zip
155.14 KB  /home/user/Downloads/image.jpg
370.86 KB  /home/user/Downloads/document.png

7.48 MB  will be cleared.

Delete these files? [y/n]: y
✓ Deleted: 2.52 MB
```

## 📜 License
This project is distributed under the MIT license.


## 🛠 Contribute
[CONTRIBUTING.md](https://github.com/pashkov256/deletor/blob/main/CONTRIBUTING.md)

