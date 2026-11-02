# Media provenance

The visuals show results of the 2022 undergraduate project. This repository was assembled in November 2026 from the original report, retained project files, and rendered videos.

## Turntables

The four original MP4 files are included unchanged under `assets/videos/`. They were retrieved from the author's [rendered-video folder](https://drive.google.com/drive/folders/1_581juqpWYv1QTdUgxJZUVrJMKO82Li8).

| Artifact | Original filename | Source |
|---|---|---|
| 1 | `Video_artefact1.mp4` | [Drive video](https://drive.google.com/file/d/1wysPdyqLNCbbHDofwEatiL5aSMu3jwKH/view) |
| 3 | `Video_artefact3.mp4` | [Drive video](https://drive.google.com/file/d/1GadCV6noyzxi2q-g1qBZwYJmab2BBNJf/view) |
| 5 | `Video_artefact5.mp4` | [Drive video](https://drive.google.com/file/d/1m4vMa5X-vXrbKe8tPgAhosLAodsC6DV6/view) |
| 6 | `video_artefact6.mp4` | [Drive video](https://drive.google.com/file/d/1YxJelQM3_-oc7QE2NeLJiUN2soCibzgr/view) |

GIF previews preserve the full video duration and camera motion at 12 frames per second. Each uses a fixed crop around the model across the sequence, proportional resizing, neutral padding, and GIF color quantization. JPEG stills use the first frame of the same presentation crop. No geometry was repaired or generated to make these previews. The original MP4s retain their original framing and resolution.

These are final presentation models. The precise reconstruction engine and full manual edit history of each render have not been verified from the retained files. Do not use them as unedited algorithm outputs or as a controlled software comparison.

## Input and comparison images

- `artifact-1-source-collage.jpg`, `artifact-3-source-collage.jpg`, `artifact-5-source-collage.jpg`, and `artifact-6-source-collage.jpg`: four visually selected frames per artifact, sampled from widely separated positions in the archived input sequences. Each complete frame is proportionally resized and arranged with its original frame number. No additional color correction or cropping was applied. The labels for artifact 5 distinguish its two source videos. These collages illustrate selected viewpoints from the larger sequences; see the [frame selections and source hashes](../evidence/source-frame-selections.json) for exact provenance.
- `artifact-3-input.jpg`: resized from the archived input `artefact3/artefact3_frames00181.jpg`. Its prior color-adjustment history is unknown.
- `artifact-3-meshroom-report.jpg` and `artifact-3-recap-report.jpg`: original embedded images from printed page 15 of the report, preserving the report's software labels.
- `focal-length-report-a.jpg` and `focal-length-report-b.jpg`: original embedded Figures 5 and 6 from printed page 14 of the report, preserving its experimental labels. These snapshots alone do not validate the reported mechanism or quantify accuracy.

The [2022 report](../reports/NIO_Project_report_2022.pdf) is unchanged. Its broad novelty and generalization claims should be read in their historical context; the current [project notes](project-notes.md) state the narrower conclusions supported by the retained evidence.
