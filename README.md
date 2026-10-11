# VideoStreamLab

A Google Colab notebook with practical utilities for inspecting,
downloading, organizing, extracting, and processing video files. It
brings common media workflows together in one place using tools such as
FFmpeg, FFprobe, MediaInfo, MKVToolNix, and yt-dlp.

## Features

-   **Video metadata:** Inspect media information with FFmpeg and
    MediaInfo, including video, audio, and subtitle streams.
-   **Batch duration checks:** Read durations for a video file, a list
    of files, or files in a folder.
-   **Sample generation:** Generate video samples using the notebook's
    sample-generation workflow.
-   **Screenshot extraction:** Extract still images from videos at
    selected timestamps.
-   **Download utilities:** Download files from supported direct links
    and selected file-hosting services.
-   **YouTube downloads:** Download video or audio using `yt-dlp`, with
    options for format, output name, folder, and cookies.
-   **Archive extraction:** Extract ZIP, RAR, 7Z, and TAR archives,
    including password-protected archives where supported by the
    installed utility.
-   **File and folder operations:** Create, copy, move, inspect size,
    and delete files or folders.
-   **Video compression:** Compress or re-encode videos with codecs such
    as H.264, H.265/HEVC, VP9, or AV1 where supported by the installed
    FFmpeg build.
-   **Multi-function media workflows:** Combine stream inspection and
    selection with media processing options provided by the notebook.

## Getting Started

### Run in Google Colab

1.  upload `Videofunc.ipynb` to Colab.
2.  Run the relevant cell.
3.  Enter the requested file path, URL, format, or output folder in the
    cell's input fields.
4.  Review the output and confirm that the generated files are saved to
    the intended location.
5.  Use the notebook's download cell when you need to download output
    files from the Colab runtime.

### Requirements

The notebook is designed for a Google Colab/Linux-style environment and
uses a combination of:

-   Python
-   FFmpeg / FFprobe
-   MediaInfo
-   MKVToolNix (`mkvmerge`)
-   `yt-dlp`
-   System archive utilities such as `unzip`, `unrar`, and `7z`
-   Other Python packages imported by individual cells

Some cells attempt to install missing system tools. Installation may
require appropriate runtime permissions and an internet connection.

## Notebook Sections

  -----------------------------------------------------------------------
  Section                             Purpose
  ----------------------------------- -----------------------------------
  Metadata                            Display media information using
                                      FFmpeg

  MediaInfo                           Summarize video, audio, and
                                      subtitle streams

  Multiple Files Duration             Check duration for multiple video
                                      files

  Generate Sample                     Create samples using the notebook's
                                      sample workflow

  Screenshot                          Extract screenshots from video

  Save Colab Files                    Download files from the Colab
                                      runtime

  Download (Standard)                 Download files using supported link
                                      types

  Extract Archives                    Extract supported archive formats

  Folder (Standard)                   Perform file and folder operations

  Web Download                        Browser-assisted web download
                                      workflow

  YouTube                             Download video or audio with yt-dlp

  Compress                            Re-encode or compress video

  Multi Functions                     Use combined media stream and
                                      processing utilities
  -----------------------------------------------------------------------

## Notes and Limitations

-   Run the notebook in a compatible runtime; local environments may
    require manual installation and configuration of system tools.
-   Supported download services and URLs can change over time.
-   Large downloads and video encodes may take significant time and
    runtime storage.
-   Review commands and file paths before running operations that move
    or delete files.
-   Only download content that you own or are authorized to access, and
    follow the terms of the relevant websites and services.
-   The exact options available depend on the installed tool versions
    and the FFmpeg build.

