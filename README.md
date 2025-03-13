# Alma 2930 Video Converter

This script converts a video for playback on the **Alma 2930** set-top box using `ffmpeg`.

## Features

Options tailored for **Alma 2930 compatibility**:

- 🎥 **Video Encoding**: Uses **H.264 (libx264)** with **Baseline profile & Level 3.0** for broad compatibility.
- 🔄 **Resolution Scaling**: Converts video to **1280x720 (HD)**.
- 🔧 **Bitrate Control**: Sets **video bitrate to 1500 kbps** with appropriate maxrate and buffer size.
- 🔊 **Audio Encoding**: Uses **AAC (Advanced Audio Codec)** at **128 kbps**.
- 🚀 **Progressive Streaming**: Uses `-movflags faststart` to optimize playback.

---

## 📌 Usage

```sh
./convertor [OPTIONS]
```

### Options:
| Option | Description |
|--------|-------------|
| `-i, --input FILE1 [FILE2 ...]` | Specify input file(s) for conversion. |
| `-o, --output FILE1 [FILE2 ...]` | Specify output file(s) or output folder. |
| `-v, --version` | Show version information. |
| `-h, --help` | Show this help screen. |

---

## 🛠 Examples

### Convert multiple files:
```sh
./convertor -i input1.avi input2.mp4 -o output1.mp4 output2.mp4
```

### Convert a single file to a folder:
```sh
./convertor -i input1.avi -o output_folder/
```

### Convert multiple files to a folder:
```sh
./convertor -i input1.avi input2.mp4 -o output_folder/
```

### Show version info:
```sh
./convertor -v
```

### Show help screen:
```sh
./convertor -h
```

---

📢 **Note:** Ensure `ffmpeg` is installed and accessible from your command line.

🚀 Happy converting!
