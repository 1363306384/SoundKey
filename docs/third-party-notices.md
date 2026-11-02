# Third-party notices

[Back to home](../README.md) · [返回中文首页](../README.zh-CN.md)

SoundKey's installers include third-party command-line tools and their runtime dependencies for online import and audio conversion. These components retain their own licenses and notices. This repository provides application documentation and release downloads; it does not publish SoundKey application source code.

| Component | Version bundled in 1.0.0 | Project and notices |
| --- | --- | --- |
| yt-dlp | 2026.10.26 | [Project](https://github.com/yt-dlp/yt-dlp) · Unlicense, with additional terms for bundled dependencies |
| Deno | 2.9.8 | [Project](https://github.com/denoland/deno) · MIT |
| FFmpeg | 9.0.2 | [Project](https://ffmpeg.org/) · The bundled builds declare GPLv3 |

The current packages invoke FFmpeg for conversion and probing; they do not include a separate `ffprobe` executable. Original upstream manifests may also describe FFprobe or files from a larger upstream archive.

## License texts and provenance

| Document | Mac | Windows |
| --- | --- | --- |
| yt-dlp license | [Text](licenses/macos/yt-dlp-LICENSE.txt) | [Text](licenses/windows/yt-dlp-LICENSE.txt) |
| yt-dlp bundled dependency notices | [Text](licenses/macos/yt-dlp-THIRD_PARTY_LICENSES.txt) | [Text](licenses/windows/yt-dlp-THIRD_PARTY_LICENSES.txt) |
| Deno license | [Text](licenses/macos/deno-LICENSE.txt) | [Text](licenses/windows/deno-LICENSE.txt) |
| FFmpeg GPLv3 license | [Text](licenses/macos/ffmpeg-GPLv3-LICENSE.txt) | [Text](licenses/windows/ffmpeg-GPLv3-LICENSE.txt) |
| Recorded download/source URLs | [Text](licenses/macos/SOURCE-URLS.txt) | [Text](licenses/windows/SOURCE-URLS.txt) |
| FFmpeg build/source information | [Text](licenses/macos/ffmpeg-UPSTREAM-README.txt) | [Text](licenses/windows/ffmpeg-UPSTREAM-README.txt) |
| Mac FFmpeg build configuration | [Text](licenses/macos/ffmpeg-build-versions.txt) | — |

Mac FFmpeg binaries come from the Martin Riedl build distribution; Windows FFmpeg binaries come from Gyan's essentials build. The linked platform notices record their respective source and build references. Licenses and additional dependency notices are also included with the installed tools.

YouTube is a trademark of Google LLC. SoundKey is an independent application and is not affiliated with or endorsed by YouTube or Google.

---

安装包内含用于在线导入与音频转换的第三方工具及依赖，各自保留原许可。上表提供对应许可和来源记录。当前安装包不单独附带 `ffprobe` 可执行文件；原上游清单可能仍提到它。此仓库用于介绍、使用文档与安装包发布，不包含 SoundKey 应用源码。
