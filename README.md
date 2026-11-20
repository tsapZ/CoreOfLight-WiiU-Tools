# Core of Light: Wii U converter package

The package [Skylanders: Core of Light](https://github.com/tsapZ/SkylandersCoreOfLight) downloads for its
"Wii U figures" setting (tsapZ/SkylandersCoreOfLight#56). It holds
[SkyP4tcher](https://github.com/SkyP4tcher)'s two converters, which turn your own extracted Wii U copy of
Skylanders SuperChargers or Imaginators into the Xbox 360 format, with everything they need to run, so you
don't have to install Python:

| Part | Version | Licence |
| --- | --- | --- |
| [superpatcher](https://github.com/SkyP4tcher/superpatcher) | v0.2.0 | LGPL-2.1-or-later |
| [imagipatcher](https://github.com/SkyP4tcher/imagipatcher) | v0.2.0-pre | LGPL-2.1-or-later |
| Python, the embeddable build from python.org | 3.14.10 | PSF |
| numpy (PyPI wheel) | 2.5.5 | BSD-3-Clause |
| scipy (PyPI wheel) | 1.18.1 | BSD-3-Clause |
| ffmpeg, [BtbN's LGPL build](https://github.com/BtbN/FFmpeg-Builds) (source: [FFmpeg](https://github.com/FFmpeg/FFmpeg)) | n8.1 | LGPL-2.1-or-later |

The tools' source is in the package unchanged. `manifest.json` lists where every part came from and its
SHA-256, and `LICENSES` has every licence. The package is built by `maintainer/tools/wiiu_tools_package.py` in
Core of Light's repository (it arrives there with the button), and Core of Light checks the download against the
SHA-256 it was built with. The ffmpeg source for this build: the FFmpeg commit named on BtbN's release page.

The package contains no game files. The converters only read the files you give them, and they don't
decrypt or download anything.

Questions about the conversion itself go to SkyP4tcher's repositories; questions about the button go to
Core of Light.
