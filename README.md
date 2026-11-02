# Underwater 3D Reconstruction from Expedition Video

**Summer Internship Project · CSIR–National Institute of Oceanography, Goa · May–July 2022**

An exploration of photogrammetry for documenting underwater archaeological artifacts at Dwarka, India. I turned selected expedition footage into textured 3D models and compared reconstruction workflows.

## Reconstructed artifacts

Click a preview to open its full-resolution video.

<table>
  <tr>
    <td width="50%" align="center"><a href="assets/videos/artifact-1.mp4"><img src="assets/previews/artifact-1.gif" alt="Rotating textured reconstruction of artifact 1" width="480"></a><br><strong>Artifact 1</strong> · <a href="assets/videos/artifact-1.mp4">Full video</a></td>
    <td width="50%" align="center"><a href="assets/videos/artifact-3.mp4"><img src="assets/previews/artifact-3.gif" alt="Rotating textured reconstruction of artifact 3, with a central opening" width="480"></a><br><strong>Artifact 3</strong> · <a href="assets/videos/artifact-3.mp4">Full video</a></td>
  </tr>
  <tr>
    <td width="50%" align="center"><a href="assets/videos/artifact-5.mp4"><img src="assets/previews/artifact-5.gif" alt="Rotating textured reconstruction of the elongated artifact 5" width="480"></a><br><strong>Artifact 5</strong> · <a href="assets/videos/artifact-5.mp4">Full video</a></td>
    <td width="50%" align="center"><a href="assets/videos/artifact-6.mp4"><img src="assets/previews/artifact-6.gif" alt="Rotating textured reconstruction of artifact 6, a rectangular surface" width="480"></a><br><strong>Artifact 6</strong> · <a href="assets/videos/artifact-6.mp4">Full video</a></td>
  </tr>
</table>

*Final presentation models from the original project. Full-resolution MP4s are included unchanged. [Preview details and media provenance](docs/media-provenance.md).*

## From underwater imagery to a model

<table>
  <tr><th width="50%">Archived input frame · Artifact 3</th><th width="50%">Final presentation model · Artifact 3</th></tr>
  <tr>
    <td><img src="assets/images/artifact-3-input.jpg" alt="Underwater video frame showing artifact 3 and its central opening" width="480"></td>
    <td><img src="assets/images/artifact-3.jpg" alt="Still from the textured artifact 3 turntable" width="480"></td>
  </tr>
</table>

*An archived frame from the multiview input sequence, shown alongside the final presentation model.*

The existing still photographs did not provide enough usable coverage. I screened approximately **102 GB of imagery and video**, grouped the data around six artifacts, and selected footage for **four artifacts**. The NIO team had collected the expedition data before my project began.

**My work:** footage selection, color adjustment, frame extraction and filtering, focal-length metadata experiments, reconstruction with Meshroom and Autodesk ReCap, and mesh processing and presentation with MeshLab and Blender.

**Workflow:** select footage → prepare frames → assign metadata → reconstruct → inspect and process meshes.

## Comparing the reconstruction tools

<table>
  <tr><th width="50%">Meshroom · Artifact 3</th><th width="50%">Autodesk ReCap · Artifact 3</th></tr>
  <tr>
    <td><img src="assets/images/artifact-3-meshroom-report.jpg" alt="Artifact 3 Meshroom reconstruction reproduced from the 2022 report" width="480"></td>
    <td><img src="assets/images/artifact-3-recap-report.jpg" alt="Artifact 3 Autodesk ReCap reconstruction reproduced from the 2022 report" width="480"></td>
  </tr>
</table>

*Original report snapshots used for qualitative comparison of surface detail, texture, and unwanted geometry.*

<details>
<summary><strong>Focal-length metadata experiment</strong></summary>

The 2022 report compared the same frame set with and without a nominal **3 mm** focal-length EXIF tag.

<table>
  <tr><th width="50%">With focal-length metadata</th><th width="50%">Without focal-length metadata</th></tr>
  <tr>
    <td><img src="assets/images/focal-length-report-a.jpg" alt="Report Figure 5: reconstruction with a 3 mm focal-length tag" width="480"></td>
    <td><img src="assets/images/focal-length-report-b.jpg" alt="Report Figure 6: reconstruction without focal-length metadata" width="480"></td>
  </tr>
</table>

The report describes fewer floating mesh artifacts with metadata. This was a qualitative observation. The surviving project files do not establish calibrated camera intrinsics or fully reproduce the paired experiment. See the [project notes](docs/project-notes.md) for the recovered evidence and limitations.

</details>

## Project record

- [Technical notes and recovered reconstruction statistics](docs/project-notes.md)
- [Original project report · 2022](reports/NIO_Project_report_2022.pdf)
- [Original rendered videos on Google Drive](https://drive.google.com/drive/folders/1_581juqpWYv1QTdUgxJZUVrJMKO82Li8)

This repository presents the 2022 results. Evaluation was qualitative; no independent geometric accuracy measurement is reported. The reconstruction algorithms were supplied by the existing tools.

**Acknowledgments:** Expedition imagery from the NIO team. Project guidance from Mr. Sundaresh and Pramod Kumar Maurya at CSIR–NIO.
