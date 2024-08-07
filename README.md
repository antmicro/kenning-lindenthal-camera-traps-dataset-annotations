# Lindenthal Camera Traps Dataset - Instance Segmentation Annotations

Copyright (c) 2023-2024 [Antmicro](https://www.antmicro.com/)

This repository provides instance segmentation annotations in the [COCO JSON](https://cocodataset.org/#format-data) format for a subset of the [Lindenthal Camera Traps](https://lila.science/datasets/lindenthal-camera-traps/) dataset.

The Lindenthal Camera Traps Dataset comprises 775 video recordings captured at the [Lindenthal Wildlife Park](https://www.lindenthaler-tierpark.de/) in Cologne, Germany, using an *Intel RealSense D435* stereo camera.

![Example](img/example.gif)

### Annotations

The annotations were created by excluding the first 20 frames of each video to avoid any influence from the *Intel RealSense D435* stereo camera's automatic exposure adjustment.
From the remaining frames, every 10th frame was annotated.

Each annotation includes:

- **Instance Mask:** Pixel-level segmentation for precise shape definition of each animal.
- **Bounding Box:** Rectangular regions enclosing each detected animal, useful for object detection tasks.
- **Class Label:** Specific identification of the animal species.

## Licenses

The annotations are provided in the [annotations_lindenthal.json](annotations_lindenthal.json) file and are licensed under the [Apache-2.0 license](LICENSE).

The video recordings are available for download from the [LILA repository](https://lila.science/datasets/lindenthal-camera-traps/) and are subject to the licensing terms specified on the website.
