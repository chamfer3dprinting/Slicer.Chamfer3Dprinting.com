# Chamfer3D Slicer roadmap

This is the initial development plan. Unchecked items are planned work.

## 1. Establish the project

- [x] Create `chamfer3dprinting/Slicer.Chamfer3Dprinting.com` as a public Bambu Studio fork.
- [x] Add Chamfer3D project documentation and preserve upstream documentation and license.
- [x] Enable the project's issue tracker.
- [ ] Record a successful Windows baseline build and its toolchain versions.
- [ ] Compare the current upstream development snapshot with an upstream stable release before choosing a release baseline.

**Done when:** a documented local build launches, imports a sample model, slices it, and exports a file.

## 2. Create the Chamfer3D application identity

- [ ] Set the displayed application name to Chamfer3D Slicer.
- [ ] Add original Chamfer3D icons, splash artwork, and theme colors.
- [ ] Update About, help, project links, and installer metadata.
- [ ] Give Chamfer3D its own application identifiers and settings/profile directories.
- [ ] Review inherited update, account, telemetry, and networking integrations before a branded release.
- [ ] Preserve upstream attribution and license notices.

**Done when:** the branded application installs and runs alongside Bambu Studio with separate settings.

## 3. Verify the printing workflow

- [ ] Choose the first printer models and filament profiles to validate.
- [ ] Verify import, movement, rotation, scaling, and plate arrangement with STL and 3MF fixtures.
- [ ] Verify layer height, walls, infill, supports, and adhesion settings.
- [ ] Check layer preview and export using a documented reference model.
- [ ] Compare output with the selected upstream baseline.
- [ ] Validate printer-specific start/end G-code and thermal, motion, and build-volume limits.

**Done when:** a documented printer/profile combination passes the full preparation, slicing, preview, and export workflow.

## 4. Package the first preview

- [ ] Produce a Windows preview installer with a distinct Chamfer3D identity.
- [ ] Publish reproducible build instructions, source revision, and release notes.
- [ ] Document verified printers, remaining limitations, and the feedback process.
- [ ] Test installation, upgrade, and removal on a clean Windows environment.

**Done when:** a versioned preview is available with matching source and recorded verification.

## Later candidates

- Additional printer and material profiles.
- macOS and Linux builds.
- Workflow improvements driven by print testing.
- A project/download website at the intended domain.
- Printer connection features after their dependencies and supported interfaces are evaluated.
