This script converts a video for playback on
the Alma 2930 set-top box using ffmpeg.

Options tailored for Alma 2930 compatibility:

- Use H.264 codec (libx264) with baseline profile and level 3.0 for broad compatibility.
- Scale video to 1280x720 resolution.
- Set video bitrate to 1500 kbps with corresponding maxrate and buffer size.
- Encode audio with AAC at 128 kbps.
- Use faststart to optimize the file for progressive streaming.


Usage:
  ./convertor [OPTIONS]
Options:
  -i, --input FILE1 [FILE2 ...]  Specify input file(s) for conversion.
  -o, --output FILE1 [FILE2 ...] Specify output file(s) or folder.
  -v, --version                  Show version information.
  -h, --help                     Show this help screen.
Examples:
  ./convertor -i input1.avi input2.mp4 -o output1.mp4 output2.mp4
  ./convertor -i input1.avi -o output_folder/
  ./convertor -i input1.avi input2.mp4 -o output_folder/
  ./convertor -v
  ./convertor -h


