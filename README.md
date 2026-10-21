# hierarchical-cow-behavior-monitoring
# Precision Dairy Cow Behavior Monitoring Pipeline
This repository contains the source code, dataset configuration, and Jupyter notebooks accompanying our published research on non-contact, automated individual monitoring of dairy cow behaviors in obstrcuted free-stall barn environments. The notebooks implement Computer Vision (CV) pipelines using Object Detection via YOLO [You only looks once], and RT-DETR-L (Real-Time Detection Transformer, large variant] using YOLO txt dataset containing 214,187 annotated images.
## Three-Stage Analytical Pipeline
The codebase is organized around a robust three-stage computer vision and tracking framework:
## 1.	Object Detection Stage
o	Models: YOLOv11m and RT-DETR-L
o	Objective: Bounding-box detection of dairy cows.
## 2.	Segmentation Stage
o	Models: YOLOv11m-SAM2 and RT-DETR-L-SAM2
### o	Objective: Instance segmentation refinement using the Segment Anything Model 2 (SAM2) architecture. Tracking & Evaluation Stage
o	Configurations Evaluated:
	YOLOv11m-SAM2 (Day and Night conditions)
	RT-DETR-L-SAM2 (Day and Night conditions)
	YOLOv11m-ByteTrack (Day and Night conditions)
	RT-DETR-L-ByteTrack (Day and Night conditions)
o	Objective: Multi-object tracking (MOT) performance, identity maintenance, and continuous behavioral classification using high-crowding videos under varied illumination conditions.
## Target Behavioral Classes (n = 5)
Drinking; Feeding; Resting; Standing; and Walking.
# Related Publication
A Hierarchical Computer Vision Framework for Continuous Dairy Cow Behavior Monitoring in an Obstructed Free-Stall Barns. Smart Agricultural Technology. 10.1016/j.atech.2026.102622.
