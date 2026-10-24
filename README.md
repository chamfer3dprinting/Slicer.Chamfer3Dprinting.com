# Slicer.Chamfer3Dprinting.com

**Chamfer3D Slicer** is a desktop 3D printing slicer project maintained by [Chamfer3Dprinting](https://github.com/chamfer3dprinting), starting from [Bambu Studio](https://github.com/bambulab/BambuStudio).

The goal is a Chamfer3D printing workflow: prepare models, choose printer and filament settings, generate toolpaths, preview layers, and export a print file.

## Project status

This public Bambu Studio fork now has the Chamfer3D application name, a separate settings key, a Windows executable named `chamfer3d-slicer.exe`, and a Windows preview build workflow. Much of the interface, artwork, profiles, and functionality still comes from upstream. GUI and printer workflow verification, further branding, and an installer remain planned.

## Windows preview download

Published previews will appear on the [Releases page](https://github.com/chamfer3dprinting/Slicer.Chamfer3Dprinting.com/releases). A successful [Windows preview build](https://github.com/chamfer3dprinting/Slicer.Chamfer3Dprinting.com/actions/workflows/build_all.yml) also provides the `Chamfer3D-Slicer-Windows-x64-preview` artifact. Failed or running builds do not provide a ready app.

Download the portable ZIP, extract the entire contents, and open `install-dir/chamfer3d-slicer.exe`. Keep the executable, DLLs, and resources together. The build checks CLI startup; the preview still needs GUI and printer workflow testing.

The repository name is the intended project identity. A website at that address has not been deployed.

## Start here

- [Development guide](DEVELOPMENT.md): source checkout, build references, and verification.
- [Roadmap](ROADMAP.md): milestones for the first Chamfer3D release.
- [Issues](https://github.com/chamfer3dprinting/Slicer.Chamfer3Dprinting.com/issues): development tasks and feedback.
- [Original upstream README](README.upstream.md): Bambu Studio documentation and acknowledgements.

## Foundation

The inherited Bambu Studio codebase includes model preparation, slicing, G-code preview, multiple plates, supports, and printer/filament/process profiles. It uses native C++ and CMake, with upstream build guides for Windows, macOS, and Linux.

The first development milestone targets Windows. Printer support and networking behavior must be verified for Chamfer3D releases; repository creation alone does not establish compatibility.

## License and credits

This fork retains the [GNU Affero General Public License, version 3](LICENSE), and upstream copyright and attribution notices.

Bambu Studio is based on [PrusaSlicer](https://github.com/prusa3d/PrusaSlicer), which derives from [Slic3r](https://github.com/Slic3r/Slic3r). Their authors and contributors provide the foundation for this project.

The optional Bambu networking plugin is described separately in the [upstream README](README.upstream.md#license); it is not a Chamfer3D-owned component.

Chamfer3D Slicer is an independent project and is not an official Bambu Lab product.
