![Logo](resources/AudioMerge.png)
# AudioMerge

AudioMerge is a tool for merging selected audio tracks from an MKV video file into MP4.

*Remove unwanted audio tracks from your clips.*

## Features

- Browse for an MKV file with multiple audio tracks
- Remove unwanted audio tracks from your video.
- Adjust the volume of each audio track
- Save and load presets for audio track configurations
- Set custom start time for the video
- Easy-to-use graphical interface

## Getting Started

### Prerequisites
Only required if you plan on building the program yourself or running the Python script manually.

- Python 3.x
- FFmpeg 

### Clone the Repository

```bash
git clone https://github.com/cwyptt/PyAudioMerge.git
cd AudioMergeMKV
```

### Install Dependencies

```bash
pip install tkinter
```

### Install FFmpeg

1. Download FFmpeg from the [official website](https://ffmpeg.org/download.html) suitable for your operating system.
2. Ensure that the `ffmpeg` executable is in your system's PATH.
3. Extract the FFmpeg archive.
4. Place the extracted `ffmpeg` folder in the root directory of the cloned repository. The structure should look like this:

```
PyAudioMerge/
├── ffmpeg/
│   ├── bin/
│   │   ├── ffmpeg.exe (or ffmpeg for Linux/Mac)
│   ├── other folders and files
├── PyAudioMerge.py
├── PyAudioMerge.spec
├── other files
```

### Run the Application

You can run the Python script directly if you want to look at and mess with the code:

```bash
python PyAudioMerge.py
```

Alternatively, if you just want to use PyAudioMerge without diving into the code, you can download the executable from the [Releases](https://github.com/cwyptt/AudioMerge/releases) page.

### Build the Executable with PyInstaller

If you prefer to build the executable yourself, you can use PyInstaller:

1. Install PyInstaller:

   ```bash
   pip install pyinstaller
   ```

2. Build the executable:

   ```bash
   pyinstaller PyAudioMerge.spec
   ```

   The executable will be created in the `dist` directory.

If you want to build the one-file executable, utilize the files in "PyAudioMerge (Only Executable)" which is found in the resources folder.

## Usage

1. Run the application and click "Browse" to select an MKV file.
2. Adjust the volume of each audio track using the sliders.
3. Optionally, set a custom start time for the video.
4. Click "Merge Audio Files With Video" to start the merging process.
5. Save and load presets as needed for easy configuration.

## Folders

- **Export Folder:** The folder where the merged video will be saved.
- **Preset Folder:** The folder where presets are saved and loaded from.

## Contributions

Contributions are welcome! Feel free to fork the repository and submit pull requests.

## License

This project is licensed under the MIT License.

## Acknowledgments

- Thanks to the [FFmpeg](https://ffmpeg.org/) project for providing the tools needed for audio and video processing.
- The graphical interface is built using [Tkinter](https://docs.python.org/3/library/tkinter.html).
