# Slide-Templates

3D-printable guides for marking the imageable areas of glass microscope slides used in spatial biology imaging platforms, and for visualizing imageable tissue regions in FFPE and fresh frozen (FF) tissue blocks.

The models were designed in [Tinkercad](https://www.tinkercad.com) between August and October 2026 and tested on a Formlabs Form 3B+.

---

## Purpose

Spatial imaging platforms only capture tissue within a defined region of the slide. These guides help with:

- **Slide marking:** Marking the imageable area on a standard glass microscope slide (25 × 75 × 1 mm) so tissue sections can be placed inside it during microtomy.
- **Block visualization:** Checking what, and how much, of the tissue in an FFPE or FF block will fit within the imageable area before sectioning.

### Guide Forms

Each platform's guide comes in two forms:

- **Recessed guide:** Slightly larger than a microscope slide, with a recess the slide slots into. The imageable area is cut out as a hole, so the slide is held in a fixed position while you mark through it.
- **Reference guide:** Matches the footprint of a standard microscope slide and is completely flat, with the imageable area cut out as a hole. It can be held over a tissue block to preview the imageable area, or held flush against a slide to mark it.

### Slide Orientation

Each guide is embossed with its platform's abbreviation (see the **Guide Label** column in [Contents](#contents)). The abbreviation marks the label end of the slide: **always position the slide's label under the abbreviation.** This keeps the imageable area in the correct position relative to the slide label for each platform.

### Visium HD Capture Area Hole

The Visium HD guides include a second, smaller hole sized to the Visium HD capture area (6.5 × 6.5 mm). On Visium HD, the capture area is selected from within the imageable area, so this hole lets you check whether a region of interest in a tissue block will fit inside a single capture area.

The capture area hole sits **outside** the imageable area on the guide and is **for previewing tissue blocks only.** Do not use it to mark slides; mark only the outline of the imageable area.

### Supported Platforms

- CosMx
- GeoMx
- Fusion
- CellScape
- Atera
- Xenium
- Visium HD

---

## Contents

| Platform | Guide Label | Recessed Guide | Reference Guide |
|----------|-------------|----------------|-----------------|
| CosMx | CMx | `CosMx_Slide_Marker_V2_Recessed.stl` | `CosMx_Slide_Reference.stl` |
| GeoMx | GMx | `GeoMx_Slide_Marker_V2_Recessed.stl` | `GeoMx_Slide_Reference.stl` |
| Fusion | F | `Fusion_Slide_Marker_V2_Recessed.stl` | `Fusion_Slide_Reference.stl` |
| CellScape | CSc | `CellScape_Slide_Marker_Recessed.stl` | `CellScape_Slide_Reference.stl` |
| Atera | A | `Atera_Slide_Marker_Recessed.stl` | `Atera_Slide_Reference.stl` |
| Xenium | X | `Xenium_Slide_Marker_Recessed.stl` | `Xenium_Slide_Reference.stl` |
| Visium HD | V | `Visium_Slide_Marker_Recessed.stl` | `Visium_Slide_Reference.stl` |

```
[project-name]/
├── README.md
├── LICENSE
├── stl/              STL model files
└── images/           (optional) Photos of guides in use
```

All models are in **millimeters (mm)** and sized for standard 25 × 75 × 1 mm glass microscope slides. When importing into a slicer, confirm the units are set to mm so parts load at the intended size.

> **Important:** Imageable area dimensions are based on platform specifications available at the time of design (August–October 2026). Vendors may change slide formats or imageable regions between instrument or chemistry versions. Always verify against the current manufacturer documentation before relying on these guides for experimental samples.

---

## Printing

These files were tested with the following setup:

| Setting | Value |
|---------|-------|
| Printer | Formlabs Form 3B+ |
| Technology | SLA (resin) |
| Material | Formlabs Black V4.1 |
| Layer thickness | 25 µm (fine detail) or 50 µm (faster) |
| Slicer | Formlabs PreForm |

### Layer Thickness

- **25 µm** gives the smoothest surfaces and the most accurate edges, which matters for guides where precise boundaries are the point.
- **50 µm** prints significantly faster and is suitable when slight edge variation is acceptable.

### Dimensional Accuracy

Because these guides depend on precise dimensions, check a printed guide against a slide before use. Resin parts can shrink or warp slightly depending on orientation, washing, and curing.

### Notes for Other Printers

These models should print on other SLA/MSLA resin printers, though accuracy may vary with different resins and exposure settings. They have not been tested on FDM (filament) printers.

### Post-Processing

Wash and post-cure parts according to Formlabs' recommendations for Black V4.1, then remove supports and sand support marks as needed, taking care not to sand surfaces that define the imageable boundary.

---

## Usage

### Printing a Guide

1. Download the recessed and/or reference STL file for your platform from the `stl/` folder.
2. Open it in PreForm (or your printer's slicer).
3. Select Black V4.1 and a layer thickness of 25 µm or 50 µm.
4. Orient the part, generate supports, and send it to the printer.
5. Wash, cure, and finish the printed part.
6. Confirm the fit and dimensions against a blank slide before use. A recessed guide should hold the slide snugly without forcing it.

### Marking a Slide (Recessed Guide)

1. Slot a clean slide into the recess with the slide's label under the platform abbreviation and the side that will receive the tissue section facing down.
2. Trace the outline of the imageable area onto the back of the slide through the hole, using a pen whose ink is soluble in ethanol or xylene (a fine point Sharpie has been tested and works well).
3. Remove the slide from the guide.
4. During microtomy, use the marked outline to place the section within the imageable area.
5. The markings are removed with ethanol before (FFPE or frozen) or during deparaffinization (FFPE).

### Marking a Slide (Reference Guide)

1. Hold the slide flush against the guide, with the slide's label under the platform abbreviation and its edges aligned with the guide's edges.
2. Mark the imageable area on the back of the slide through the hole, as with the recessed guide.

### Previewing a Tissue Block (Reference Guide)

1. Hold the reference guide over the cut face of an FFPE or FF tissue block, keeping in mind which end the slide label will be on (the abbreviation end).
2. Look through the hole to see what, and how much, of the tissue will fit within the imageable area.
3. Use this to decide on block orientation and trimming, or whether the region of interest will fit on a single slide.
4. **Visium HD only:** Look through the smaller capture area hole to check whether your region of interest fits within the 6.5 × 6.5 mm capture area, which will later be selected from within the imageable area.

> **Visium HD:** When marking a Visium HD slide, trace only the imageable area hole. The capture area hole is for block previewing and is not positioned over the imageable area.

> **Tip:** Always mark the back of the slide, never the side the section is placed on, so ink cannot contact the tissue. A fine point Sharpie was used during testing. If you use a different pen, confirm that its ink comes off fully in your protocol's solvents before using it on experimental slides.

---

## Contributing

Contributions are welcome, especially guides for additional platforms or updated dimensions for new slide formats:

1. Fork this repository.
2. Add or modify files, keeping the existing naming convention.
3. Update the **Contents** table in this README, including the platform and the source of the dimensions used.
4. Open a pull request describing your changes.

Please report dimension errors, platform specification changes, or failed prints by opening an [issue](../../issues).

---

## Disclaimer

This project is independent and is not affiliated with, endorsed by, or sponsored by the manufacturers of any of the platforms listed. All product names and trademarks are the property of their respective owners and are used only to identify compatibility.

These guides are provided as aids for sample preparation. They are not a substitute for manufacturer instructions, and the author accepts no responsibility for lost samples or failed runs.

---

## License

Copyright 2026 Lindsay Parmelee

Licensed under the Apache License, Version 2.0 (the "License");
you may not use these files except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

The full license text is in the [`LICENSE`](LICENSE) file.

---

## Author

All designs are original work by Lindsay Parmelee · [@Lindsayparm](https://github.com/Lindsayparm)
