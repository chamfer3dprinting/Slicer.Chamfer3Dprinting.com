# Developing Chamfer3D Slicer

## Source baseline

- Fork: https://github.com/chamfer3dprinting/Slicer.Chamfer3Dprinting.com
- Upstream: https://github.com/bambulab/BambuStudio
- Initial branch: `master`
- Initial upstream commit: [`79df7ae309be398ed30c9f397c13c9911c2edc57`](https://github.com/bambulab/BambuStudio/commit/79df7ae309be398ed30c9f397c13c9911c2edc57)
- Initial upstream commit subject: FIX: 2.8.3 Beta Build Fixes (#12596)
- Repository established: October 24, 2026.

The initial commit subject identifies this as an upstream beta development snapshot. A stable release baseline has not yet been selected for Chamfer3D.

## Get the source

```sh
git clone https://github.com/chamfer3dprinting/Slicer.Chamfer3Dprinting.com.git
cd Slicer.Chamfer3Dprinting.com
git remote add upstream https://github.com/bambulab/BambuStudio.git
git switch -c chamfer/first-build
```

Keep the upstream remote available so fixes can be reviewed and brought into this fork.

## Build references

Use the build guide matching the chosen upstream source revision:

- [Windows compile guide](https://github.com/bambulab/BambuStudio/wiki/Windows-Compile-Guide)
- [macOS compile guide](https://github.com/bambulab/BambuStudio/wiki/Mac-Compile-Guide)
- [Linux compile guide](https://github.com/bambulab/BambuStudio/wiki/Linux-Compile-Guide)

The upstream Windows guide lists Visual Studio 2022 with C++ tools, CMake, Git, Perl, and pkg-config. Follow the guide's toolset constraints and dependency-build steps. The inherited `build_win.bat`, `CMakeLists.txt`, and `deps/` are the starting points for inspecting the current build.

No Chamfer3D build has been compiled or verified as part of repository initialization.

## First build verification

Record the source SHA, OS, compiler/toolset version, dependency versions, build command, and result.

1. Build and launch the inherited application.
2. Import a small, known STL model.
3. Select a documented printer and filament profile.
4. Slice the model and inspect the layer preview.
5. Export a print file and check its dimensions, temperature settings, and printer-specific commands.
6. Record the outcome before starting the application branding changes.

Use a separate test configuration for development. Before distributing Chamfer3D builds, give the application independent settings directories and application identifiers so it can run alongside Bambu Studio.

## Project layout

| Path | Purpose |
| --- | --- |
| `src/` | Application and slicing source |
| `resources/` | Application resources and profiles |
| `deps/` | Dependency build definitions |
| `cmake/` | CMake helpers |
| `tests/`, `t/` | Inherited test code and fixtures |
| `build_win.bat` | Inherited Windows build script |
| `version.inc` | Inherited version definitions |

## Change workflow

Make focused changes on a branch, document verification in the pull request, and preserve upstream copyright and license notices. Start with a reproducible baseline build, then application identity, then verified printer workflows.

See [ROADMAP.md](ROADMAP.md) for acceptance criteria for the first preview.
