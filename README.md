# Slicer.Chamfer3Dprinting.com

**Chamfer3D Slicer** is a desktop 3D printing slicer project maintained by [Chamfer3Dprinting](https://github.com/chamfer3dprinting), starting from [Bambu Studio](https://github.com/bambulab/BambuStudio).

The goal is a Chamfer3D printing workflow: prepare models, choose printer and filament settings, generate toolpaths, preview layers, and export a print file.

## Project status

The repository is initialized as a public Bambu Studio fork. Application code, interface, profiles, and build scripts currently come from upstream. Chamfer3D application branding, an independently verified build, and a Chamfer3D installer are planned.

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
