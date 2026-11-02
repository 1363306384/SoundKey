SoundKey packaging note: FFmpeg for macOS arm64

This note describes the FFmpeg executable bundled with SoundKey for Apple Silicon.
It is maintained locally for SoundKey and is not an upstream FFmpeg README.

The executable identifies itself as:
ffmpeg 9.0.2-https://www.martin-riedl.de

Recorded binary source and build recipes:
https://ffmpeg.martin-riedl.de/info/detail/macos/arm64/1789931890_9.0.2
https://github.com/Martin-Riedl/ffmpeg-builds

FFmpeg source release and source code:
https://ffmpeg.org/releases/ffmpeg-9.0.2.tar.xz
https://github.com/FFmpeg/FFmpeg/tree/n9.0.2

The actual bundled build's configuration, library versions and copyright notice
are recorded in ffmpeg-build-versions.txt. Its build enables GPL and version 3;
the accompanying GPLv3 license text is included in this directory.
See components-manifest.json for the recorded upstream file hash and
packaged-SHA256.txt for the executable hash after local code signing.

The previously copied Windows/Gyan README did not describe this Mac binary and
has been replaced by this platform-specific packaging note. The FFmpeg executable
and its behavior have not changed as part of this documentation correction.
