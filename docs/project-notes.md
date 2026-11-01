# Project notes

**Context.** Completed at CSIR–National Institute of Oceanography, Goa, from May to July 2022 during my mechanical engineering undergraduate studies, this project explored photogrammetry for documenting underwater archaeological artefacts at Dwarka.

**My contribution.** The NIO team collected the expedition imagery in February 2022; data acquisition was outside my project. I manually screened approximately 102 GB, grouped material around six artefacts, and selected four with usable footage. Available still photographs were insufficient for these reconstructions, so I used video frames.

The workflow combined manual decisions, graphical tools, and an ExifTool shell script:

1. Select stable footage with object coverage, overlapping views, and consistent zoom.
2. Adjust color in Adobe Premiere Pro, trim footage, and extract frames with VLC.
3. Reject poor frames; prepare image sets with and without focal-length EXIF metadata.
4. Reconstruct with Meshroom and Autodesk ReCap; process meshes in MeshLab and Blender.

These tools provided the reconstruction algorithms. My work focused on imagery preparation, workflow configuration, output comparison, and presentation.

**Findings and limits.** The report describes fewer floating mesh artefacts with focal-length metadata, more pronounced boundaries in Meshroom outputs, and smoother surfaces and textures in ReCap outputs. These were qualitative observations, without reported ground-truth geometry or quantitative accuracy measurements.

The metadata experiment used a nominal focal length of **3 mm**; it did not establish calibrated underwater camera intrinsics. The findings do not establish universal preferences between still images and video or between software packages.

**Recovered archive evidence.** Surviving Meshroom graphs use draft meshing directly from Structure-from-Motion, without depth-map stages. Historical cache statistics record:

| Archived run | Registered / input frames | Sparse points |
|---|---:|---:|
| Artefact 3 | 181 / 181 | 124,570 |
| Artefact 6 | 79 / 79 | 79,744 |
| Artefact 5, `noFL` | 92 / 92 | 71,626 |
| Artefact 4, test 1 | 36 / 145 | 17,091 |
| Artefact 4, test 2, video 1 | 32 / 81 | 35,597 |

These are run diagnostics, not accuracy measurements or controlled EXIF comparisons. See [archive sources and caveats](../evidence/archive-summary.json).

**About the visuals.** Turntables show final presentation models. Each render's reconstruction engine and edit history remain unverified. The example source image is an archived input frame; its color-editing history is unknown.

The [original report](../reports/NIO_Project_report_2022.pdf) is preserved as a historical 2022 document.
