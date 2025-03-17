# Batch Rename CLI (brn)

A command-line utility for batch renaming files with powerful sorting and formatting options.

## Features

- Rename multiple files at once using patterns and numbering
- Sort files by name, size, or modification date
- Customizable numbering format with padding
- Preserve file extensions
- Simple and intuitive command-line interface

## Installation

### Quick Install/Update (Linux/macOS)
```
sudo curl -fsSL https://raw.githubusercontent.com/apapamarkou/batch-rename-cli/main/brn -o /usr/bin/brn && sudo chmod +x /usr/bin/brn
```

### Requirements

- Python 3.x
- Curl
- Linux/Unix-based system

#### Ubuntu/Debian
```
sudo apt update
sudo apt install python3 curl
```
#### Fedora
```
sudo dnf update
sudo dnf install python3 curl
```
#### OpenSUSE
```
sudo zypper refresh
sudo zypper install python3 curl
```
#### Arch Linux
```
sudo pacman -Syu
sudo pacman -S python curl
```
#### CentOS/RHEL
```
sudo yum update
sudo yum install python3 curl
```
#### Alpine Linux
```
sudo apk update
sudo apk add python3 curl
```

## Usage

Basic syntax: `brn [files] [options]`

## Examples

1. Rename all JPG files with sequential numbers:
```
brn *.jpg --count 001
```

2. Rename files sorted by size in descending order:
```
brn *.png --sort-size desc --count 001
```

3. Rename with custom prefix:
```
brn *.txt --prefix document_ --count 01
```

## Options
- --count <start>: Start numbering from specified value (e.g., 001, 01)
- --prefix <text>: Add prefix to filenames
- --sort-size: Sort files by size
- --sort-date: Sort files by modification date
- --sort-name: Sort files by name (default)
    - asc/desc: Specify sorting direction (e.g., --sort-size desc)
use brn --help to view more...

## Examples with Output

Before:
```
photo1.jpg
photo2.jpg
photo3.jpg
```

After `brn *.jpg --count 001`:
```
001.jpg
002.jpg
003.jpg
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch ( git checkout -b feature/AmazingFeature)
3. Commit your changes ( git commit -m 'Add some AmazingFeature')
4. Push to the branch ( git push origin feature/AmazingFeature)
5. Open a Pull Request

## License
This project is licensed under the GNU General Public License v3.0 - see the LICENSE file for details.

## Author
Andrianos Papamarkou

## Acknowledgments
- Thanks to all contributors who have helped with the development
- Inspired by the need for efficient batch file renaming in the command line

## Support
If you encounter any issues or have questions, please file an issue on the GitHub repository.

## Changelog
#### v1.0.0
- Initial release
- Basic renaming functionality
- Sorting options
- Customizable numbering
