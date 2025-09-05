# pck3r : C++ Package Manager for Windows

Pck3r is a modern package manager for Windows 10 x64, implemented in C++ for performance and modularity. It helps users manage software installations with MSI/EXE installers on Windows. Pck3r makes installing, downloading, and managing software easier with a clear interface and straightforward commands.

## Requirements

- Windows 10 x64
- g++ compiler (MinGW or similar)

## Setup

1. Compile the project using g++:

```
g++ -Iinclude -o pck3r.exe main.cpp -lurlmon -lshell32 -lwininet
```

2. Run the executable with desired commands:

```
.\pck3r.exe [command] [options]
```

## Commands

- **install**: Install a package

```
.\pck3r.exe install [package_name]
```

Supported packages include:

- nodejs
- google-chrome
- firefox
- winrar
- vlc
- 7zip
- notepadpp
- adobereader
- java
- python

- **cls**: Clear the terminal (just for fun)

```
.\pck3r.exe cls
```

- **version**: Show the current version

```
.\pck3r.exe version
```

- **help**: Show help information

```
.\pck3r.exe /help
```

## Development

The project is modularized for easier maintenance and extension. The main executable handles command parsing and delegates to modules for specific functionality.

## License

Pck3r uses the license in the [LICENSE](./LICENSE) file.
