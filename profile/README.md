# DeployAI Environmental Services

DeployAI Environmental Services is a collection of deep learning models designed to process and analyze high-resolution and very high-resolution satellite images for various environmental applications, developed by ECMWF and NCSR. This repository includes models for object detection, leaf area index estimation, and interactive segmentation.

## Services Summary

| Service | Description | Link |
|---------|-------------|------|
| Object Detection | Detects various objects in high-resolution optical remote sensing images using YOLOv8 Oriented Bounding Box. | [Object Detection](https://github.com/DeployAI-Environmental-Services/depai-yolov8-obb) |
| Leaf Area Index Estimation | Estimates Leaf Area Index (LAI) from Sentinel-2 satellite images. | [Leaf Area Index Estimation](https://github.com/DeployAI-Environmental-Services/depai-lai) |
| Segment Anything for GeoTiff Images | Provides interactive prompt segmentation using the Segment Anything Model. | [Segment Anything](https://github.com/DeployAI-Environmental-Services/depai-sam-interactive) |

### 1. [Object Detection](https://github.com/DeployAI-Environmental-Services/depai-yolov8-obb)

This service uses the `YOLOv8 Oriented Bounding Box` model to detect objects in very high-resolution optical remote sensing images. The model is served using a web interface built with `Flask`.

#### Key Features

- Detects various objects such as planes, ships, storage tanks, and more.
- Provides a web UI for uploading and processing images.
- Outputs bounding boxes with class IDs and confidence scores.

### 2. [Leaf Area Index Estimation](https://github.com/DeployAI-Environmental-Services/depai-lai)

This service provides a deep learning model for estimating the Leaf Area Index (LAI) from Sentinel-2 satellite images. The model is exposed using a web application.

#### Key Features

- Processes Geotiff images with specific spectral bands.
- Outputs LAI estimations for the input images.
- Provides a web UI for uploading and processing images.

### 3. [Segment Anything for GeoTiff Images](https://github.com/DeployAI-Environmental-Services/depai-sam-interactive)

This service offers interactive prompt segmentation using the `Segment Anything Model`, built with Dash and Dash Leaflet.

#### Key Features

- Allows segmentation of objects with bounding boxes and points.
- Supports georeferenced RGB GeoTiff files.
- Provides options for drawing bounding boxes, uploading images, and automatic segmentation.

## Local Development

Each service repository includes detailed instructions for local development, including cloning the repository, building Docker images, and running the services in containers. Refer to the respective README files for more information.

## Container Registry

All services are available as Docker images in the GitHub Container Registry. Follow the instructions in the respective README files to pull and run the images.
