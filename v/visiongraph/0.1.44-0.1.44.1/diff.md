# Comparing `tmp/visiongraph-0.1.44-py3-none-any.whl.zip` & `tmp/visiongraph-0.1.44.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,267 +1,264 @@
-Zip file size: 241823 bytes, number of entries: 265
--rw-r--r--  2.0 unx     4275 b- defN 23-Apr-14 15:29 tools/CameraCalibratorTool.py
--rw-r--r--  2.0 unx     1018 b- defN 23-Apr-14 15:29 tools/OpenVinoModelRenamer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 tools/__init__.py
--rw-r--r--  2.0 unx      221 b- defN 23-Apr-14 15:29 tools/utils.py
--rw-r--r--  2.0 unx     1758 b- defN 23-Apr-14 15:29 visiongraph/AsyncGraphNode.py
--rw-r--r--  2.0 unx     2806 b- defN 23-Apr-14 15:29 visiongraph/BaseGraph.py
--rw-r--r--  2.0 unx      678 b- defN 23-Apr-14 15:29 visiongraph/GraphNode.py
--rw-r--r--  2.0 unx      276 b- defN 23-Apr-14 15:29 visiongraph/Processable.py
--rw-r--r--  2.0 unx     2094 b- defN 23-Apr-14 15:29 visiongraph/VisionGraph.py
--rw-r--r--  2.0 unx     1898 b- defN 23-Apr-14 15:29 visiongraph/VisionGraphBuilder.py
--rw-r--r--  2.0 unx    23501 b- defN 23-Apr-14 15:29 visiongraph/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/cache/__init__.py
--rw-r--r--  2.0 unx      368 b- defN 23-Apr-14 15:29 visiongraph/data/Asset.py
--rw-r--r--  2.0 unx      376 b- defN 23-Apr-14 15:29 visiongraph/data/LocalAsset.py
--rw-r--r--  2.0 unx     1099 b- defN 23-Apr-14 15:29 visiongraph/data/RepositoryAsset.py
--rw-r--r--  2.0 unx      324 b- defN 23-Apr-14 15:29 visiongraph/data/__init__.py
--rw-r--r--  2.0 unx     2568 b- defN 23-Apr-14 15:29 visiongraph/data/labels/COCO.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/data/labels/__init__.py
--rw-r--r--  2.0 unx      172 b- defN 23-Apr-14 15:29 visiongraph/dsp/BaseFilterNumpy.py
--rw-r--r--  2.0 unx     2421 b- defN 23-Apr-14 15:29 visiongraph/dsp/LandmarkSmoothFilter.py
--rw-r--r--  2.0 unx     1487 b- defN 23-Apr-14 15:29 visiongraph/dsp/OneEuroFilter.py
--rw-r--r--  2.0 unx     1651 b- defN 23-Apr-14 15:29 visiongraph/dsp/OneEuroFilterNumba.py
--rw-r--r--  2.0 unx     2642 b- defN 23-Apr-14 15:29 visiongraph/dsp/OneEuroFilterNumpy.py
--rw-r--r--  2.0 unx     1037 b- defN 23-Apr-14 15:29 visiongraph/dsp/VectorNumpySmoothFilter.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/dsp/__init__.py
--rw-r--r--  2.0 unx      619 b- defN 23-Apr-14 15:29 visiongraph/estimator/BaseClassifier.py
--rw-r--r--  2.0 unx      397 b- defN 23-Apr-14 15:29 visiongraph/estimator/BaseEstimator.py
--rw-r--r--  2.0 unx     4091 b- defN 23-Apr-14 15:29 visiongraph/estimator/BaseVisionEngine.py
--rw-r--r--  2.0 unx     1100 b- defN 23-Apr-14 15:29 visiongraph/estimator/ChainEstimator.py
--rw-r--r--  2.0 unx      403 b- defN 23-Apr-14 15:29 visiongraph/estimator/ScoreThresholdEstimator.py
--rw-r--r--  2.0 unx      868 b- defN 23-Apr-14 15:29 visiongraph/estimator/VisionClassifier.py
--rw-r--r--  2.0 unx      410 b- defN 23-Apr-14 15:29 visiongraph/estimator/VisionEstimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/__init__.py
--rw-r--r--  2.0 unx     2448 b- defN 23-Apr-14 15:29 visiongraph/estimator/calculator/UndistortionCalculator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/calculator/__init__.py
--rw-r--r--  2.0 unx     1231 b- defN 23-Apr-14 15:29 visiongraph/estimator/engine/InferenceEngineFactory.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/engine/__init__.py
--rw-r--r--  2.0 unx      529 b- defN 23-Apr-14 15:29 visiongraph/estimator/inpaint/BaseInpainter.py
--rw-r--r--  2.0 unx     2161 b- defN 23-Apr-14 15:29 visiongraph/estimator/inpaint/GMCNNInpainter.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/inpaint/__init__.py
--rw-r--r--  2.0 unx     2077 b- defN 23-Apr-14 15:29 visiongraph/estimator/onnx/ONNXVisionEngine.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/onnx/__init__.py
--rw-r--r--  2.0 unx     2220 b- defN 23-Apr-14 15:29 visiongraph/estimator/openvino/OpenVinoEngine.py
--rw-r--r--  2.0 unx     2516 b- defN 23-Apr-14 15:29 visiongraph/estimator/openvino/OpenVinoObjectDetector.py
--rw-r--r--  2.0 unx     2967 b- defN 23-Apr-14 15:29 visiongraph/estimator/openvino/OpenVinoPoseEstimator.py
--rw-r--r--  2.0 unx      726 b- defN 23-Apr-14 15:29 visiongraph/estimator/openvino/SyncInferencePipeline.py
--rw-r--r--  2.0 unx     1703 b- defN 23-Apr-14 15:29 visiongraph/estimator/openvino/VisionInferenceEngine.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/openvino/__init__.py
--rw-r--r--  2.0 unx     1750 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/CenterNetDetector.py
--rw-r--r--  2.0 unx     3270 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/CrowdHumanDetector.py
--rw-r--r--  2.0 unx     1781 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/DETRDetector.py
--rw-r--r--  2.0 unx      544 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/InstanceSegmentationEstimator.py
--rw-r--r--  2.0 unx      523 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/LandmarkEstimator.py
--rw-r--r--  2.0 unx      524 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/ObjectDetector.py
--rw-r--r--  2.0 unx     1279 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/RoiEstimator.py
--rw-r--r--  2.0 unx     3147 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/SSDDetector.py
--rw-r--r--  2.0 unx     2082 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/SlidingWindowEstimator.py
--rw-r--r--  2.0 unx     1436 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/SpatialCascadeEstimator.py
--rw-r--r--  2.0 unx     3173 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/YOLODetector.py
--rw-r--r--  2.0 unx     3594 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/YOLOv5Detector.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/__init__.py
--rw-r--r--  2.0 unx     3441 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/camera/ArUcoCameraPoseEstimator.py
--rw-r--r--  2.0 unx      850 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/camera/BoardCameraCalibrator.py
--rw-r--r--  2.0 unx     4276 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/camera/ChArUcoCalibrator.py
--rw-r--r--  2.0 unx     3145 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/camera/ChessboardCalibrator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/camera/__init__.py
--rw-r--r--  2.0 unx     1127 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/AdasFaceDetector.py
--rw-r--r--  2.0 unx      512 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/FaceDetector.py
--rw-r--r--  2.0 unx     3805 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/OpenVinoFaceDetector.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/__init__.py
--rw-r--r--  2.0 unx     1781 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/emotion/AffectNetEmotionClassifier.py
--rw-r--r--  2.0 unx      450 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/emotion/FaceEmotionEstimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/emotion/__init__.py
--rw-r--r--  2.0 unx      609 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/landmark/FaceLandmarkEstimator.py
--rw-r--r--  2.0 unx     2646 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/landmark/IrisDistanceCalculator.py
--rw-r--r--  2.0 unx     2204 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/landmark/MediaPipeFaceDetector.py
--rw-r--r--  2.0 unx     2324 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/landmark/MediaPipeFaceMeshEstimator.py
--rw-r--r--  2.0 unx     1832 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/landmark/RegressionLandmarkEstimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/landmark/__init__.py
--rw-r--r--  2.0 unx     1301 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/pose/AdasHeadPoseEstimator.py
--rw-r--r--  2.0 unx      315 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/pose/HeadPoseEstimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/pose/__init__.py
--rw-r--r--  2.0 unx     4265 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/recognition/FaceRecognitionEstimator.py
--rw-r--r--  2.0 unx     2842 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/recognition/FaceReidentificationEstimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/recognition/__init__.py
--rw-r--r--  2.0 unx      517 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/hand/HandDetector.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/hand/__init__.py
--rw-r--r--  2.0 unx      608 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/hand/landmark/HandLandmarkEstimator.py
--rw-r--r--  2.0 unx     2778 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/hand/landmark/MediaPipeHandEstimator.py
--rw-r--r--  2.0 unx     2330 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/hand/landmark/OpenPoseHandEstimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/hand/landmark/__init__.py
--rw-r--r--  2.0 unx     2086 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/AEPoseEstimator.py
--rw-r--r--  2.0 unx     5139 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/EfficientPoseEstimator.py
--rw-r--r--  2.0 unx     3890 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/LiteHRNetEstimator.py
--rw-r--r--  2.0 unx     2855 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/LitePoseEstimator.py
--rw-r--r--  2.0 unx     3100 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/MediaPipePoseEstimator.py
--rw-r--r--  2.0 unx     6641 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/MobileHumanPoseEstimator.py
--rw-r--r--  2.0 unx     9658 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/MobileNetV2PoseEstimator.py
--rw-r--r--  2.0 unx     4325 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/MoveNetPoseEstimator.py
--rw-r--r--  2.0 unx     1754 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/OpenPoseEstimator.py
--rw-r--r--  2.0 unx      518 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/PoseEstimator.py
--rw-r--r--  2.0 unx     2347 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/TopDownPoseEstimator.py
--rw-r--r--  2.0 unx     4815 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/__init__.py
--rw-r--r--  2.0 unx     7516 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/segmentation/MaskRCNNEstimator.py
--rw-r--r--  2.0 unx     1989 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/segmentation/MediaPipeSelfieSegmentation.py
--rw-r--r--  2.0 unx     3287 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/segmentation/YolactEstimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/segmentation/__init__.py
--rw-r--r--  2.0 unx     1714 b- defN 23-Apr-14 15:29 visiongraph/estimator/translation/DeblurGANv2.py
--rw-r--r--  2.0 unx      314 b- defN 23-Apr-14 15:29 visiongraph/estimator/translation/DepthEstimator.py
--rw-r--r--  2.0 unx     2898 b- defN 23-Apr-14 15:29 visiongraph/estimator/translation/MidasDepthEstimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/translation/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/external/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/external/intel/__init__.py
--rw-r--r--  2.0 unx     4337 b- defN 23-Apr-14 15:29 visiongraph/external/intel/performance_metrics.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/external/intel/adapters/__init__.py
--rw-r--r--  2.0 unx     5682 b- defN 23-Apr-14 15:29 visiongraph/external/intel/adapters/inference_adapter.py
--rw-r--r--  2.0 unx    15557 b- defN 23-Apr-14 15:29 visiongraph/external/intel/adapters/openvino_adapter.py
--rw-r--r--  2.0 unx     7413 b- defN 23-Apr-14 15:29 visiongraph/external/intel/adapters/ovms_adapter.py
--rw-r--r--  2.0 unx    10920 b- defN 23-Apr-14 15:29 visiongraph/external/intel/adapters/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/__init__.py
--rw-r--r--  2.0 unx     7582 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/centernet.py
--rw-r--r--  2.0 unx     6784 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/detection_model.py
--rw-r--r--  2.0 unx     3215 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/detr.py
--rw-r--r--  2.0 unx    16363 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/hpe_associative_embedding.py
--rw-r--r--  2.0 unx     8434 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/image_model.py
--rw-r--r--  2.0 unx    19269 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/model.py
--rw-r--r--  2.0 unx    19768 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/open_pose.py
--rw-r--r--  2.0 unx     5995 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/ssd.py
--rw-r--r--  2.0 unx     7510 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/types.py
--rw-r--r--  2.0 unx     7600 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/utils.py
--rw-r--r--  2.0 unx    24161 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/yolo.py
--rw-r--r--  2.0 unx      154 b- defN 23-Apr-14 15:29 visiongraph/external/intel/pipelines/__init__.py
--rw-r--r--  2.0 unx     5407 b- defN 23-Apr-14 15:29 visiongraph/external/intel/pipelines/async_pipeline.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/external/midas/__init__.py
--rw-r--r--  2.0 unx     7868 b- defN 23-Apr-14 15:29 visiongraph/external/midas/transforms.py
--rw-r--r--  2.0 unx      193 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/__init__.py
--rw-r--r--  2.0 unx     1816 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/core.py
--rw-r--r--  2.0 unx      333 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/detector.py
--rw-r--r--  2.0 unx     1147 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/metrics.py
--rw-r--r--  2.0 unx     5402 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/model.py
--rw-r--r--  2.0 unx     3576 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/testing.py
--rw-r--r--  2.0 unx     2647 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/testing_viz.py
--rw-r--r--  2.0 unx    16512 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/tracker.py
--rw-r--r--  2.0 unx      652 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/utils.py
--rw-r--r--  2.0 unx     5312 b- defN 23-Apr-14 15:29 visiongraph/external/motrackers/Track.py
--rw-r--r--  2.0 unx     7486 b- defN 23-Apr-14 15:29 visiongraph/external/motrackers/Tracker.py
--rw-r--r--  2.0 unx      184 b- defN 23-Apr-14 15:29 visiongraph/external/motrackers/__init__.py
--rw-r--r--  2.0 unx       83 b- defN 23-Apr-14 15:29 visiongraph/external/motrackers/utils/__init__.py
--rw-r--r--  2.0 unx     8978 b- defN 23-Apr-14 15:29 visiongraph/external/motrackers/utils/misc.py
--rw-r--r--  2.0 unx    16025 b- defN 23-Apr-14 15:29 visiongraph/input/AzureKinectInput.py
--rw-r--r--  2.0 unx     4108 b- defN 23-Apr-14 15:29 visiongraph/input/BaseDepthCamera.py
--rw-r--r--  2.0 unx     1309 b- defN 23-Apr-14 15:29 visiongraph/input/BaseDepthInput.py
--rw-r--r--  2.0 unx     3760 b- defN 23-Apr-14 15:29 visiongraph/input/BaseInput.py
--rw-r--r--  2.0 unx     1721 b- defN 23-Apr-14 15:29 visiongraph/input/CamGearInput.py
--rw-r--r--  2.0 unx     1493 b- defN 23-Apr-14 15:29 visiongraph/input/ImageInput.py
--rw-r--r--  2.0 unx    18995 b- defN 23-Apr-14 15:29 visiongraph/input/RealSenseInput.py
--rw-r--r--  2.0 unx     5032 b- defN 23-Apr-14 15:29 visiongraph/input/VideoCaptureInput.py
--rw-r--r--  2.0 unx     1305 b- defN 23-Apr-14 15:29 visiongraph/input/__init__.py
--rw-r--r--  2.0 unx     1887 b- defN 23-Apr-14 15:29 visiongraph/model/CameraIntrinsics.py
--rw-r--r--  2.0 unx      101 b- defN 23-Apr-14 15:29 visiongraph/model/CameraStreamType.py
--rw-r--r--  2.0 unx      549 b- defN 23-Apr-14 15:29 visiongraph/model/DepthBuffer.py
--rw-r--r--  2.0 unx      753 b- defN 23-Apr-14 15:29 visiongraph/model/VisionEngineOutput.py
--rw-r--r--  2.0 unx      135 b- defN 23-Apr-14 15:29 visiongraph/model/_ImportStub.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/model/__init__.py
--rw-r--r--  2.0 unx     4229 b- defN 23-Apr-14 15:29 visiongraph/model/geometry/BoundingBox2D.py
--rw-r--r--  2.0 unx      815 b- defN 23-Apr-14 15:29 visiongraph/model/geometry/Size2D.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/model/geometry/__init__.py
--rw-r--r--  2.0 unx      585 b- defN 23-Apr-14 15:29 visiongraph/model/parameter/ArgumentConfigurable.py
--rw-r--r--  2.0 unx      186 b- defN 23-Apr-14 15:29 visiongraph/model/parameter/NamedParameter.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/model/parameter/__init__.py
--rw-r--r--  2.0 unx      399 b- defN 23-Apr-14 15:29 visiongraph/model/tracker/Trackable.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/model/tracker/__init__.py
--rw-r--r--  2.0 unx      440 b- defN 23-Apr-14 15:29 visiongraph/model/types/ModelPrecision.py
--rw-r--r--  2.0 unx      199 b- defN 23-Apr-14 15:29 visiongraph/model/types/RealSenseColorScheme.py
--rw-r--r--  2.0 unx      204 b- defN 23-Apr-14 15:29 visiongraph/model/types/RealSenseFilter.py
--rw-r--r--  2.0 unx     1180 b- defN 23-Apr-14 15:29 visiongraph/model/types/VideoCaptureBackend.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/model/types/__init__.py
--rw-r--r--  2.0 unx      905 b- defN 23-Apr-14 15:29 visiongraph/node/ApplyNode.py
--rw-r--r--  2.0 unx      753 b- defN 23-Apr-14 15:29 visiongraph/node/BreakpointNode.py
--rw-r--r--  2.0 unx      815 b- defN 23-Apr-14 15:29 visiongraph/node/CustomNode.py
--rw-r--r--  2.0 unx      903 b- defN 23-Apr-14 15:29 visiongraph/node/ExtractNode.py
--rw-r--r--  2.0 unx      525 b- defN 23-Apr-14 15:29 visiongraph/node/PassThroughNode.py
--rw-r--r--  2.0 unx      825 b- defN 23-Apr-14 15:29 visiongraph/node/SequenceNode.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/node/__init__.py
--rw-r--r--  2.0 unx     1471 b- defN 23-Apr-14 15:29 visiongraph/output/ImagePreview.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/output/__init__.py
--rw-r--r--  2.0 unx      935 b- defN 23-Apr-14 15:29 visiongraph/output/fbs/FrameBufferSharingServer.py
--rw-r--r--  2.0 unx     1390 b- defN 23-Apr-14 15:29 visiongraph/output/fbs/SpoutServer.py
--rw-r--r--  2.0 unx     3287 b- defN 23-Apr-14 15:29 visiongraph/output/fbs/SyphonServer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/output/fbs/__init__.py
--rw-r--r--  2.0 unx      980 b- defN 23-Apr-14 15:29 visiongraph/recorder/AsyncFrameSetRecorder.py
--rw-r--r--  2.0 unx     1108 b- defN 23-Apr-14 15:29 visiongraph/recorder/BaseFrameRecorder.py
--rw-r--r--  2.0 unx     1143 b- defN 23-Apr-14 15:29 visiongraph/recorder/CV2VideoRecorder.py
--rw-r--r--  2.0 unx     1016 b- defN 23-Apr-14 15:29 visiongraph/recorder/FrameSetRecorder.py
--rw-r--r--  2.0 unx      905 b- defN 23-Apr-14 15:29 visiongraph/recorder/MoviePyVideoRecorder.py
--rw-r--r--  2.0 unx     1377 b- defN 23-Apr-14 15:29 visiongraph/recorder/VidGearVideoRecorder.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/recorder/__init__.py
--rw-r--r--  2.0 unx      564 b- defN 23-Apr-14 15:29 visiongraph/result/ArUcoCameraPose.py
--rw-r--r--  2.0 unx     1521 b- defN 23-Apr-14 15:29 visiongraph/result/ArUcoMarkerDetection.py
--rw-r--r--  2.0 unx      167 b- defN 23-Apr-14 15:29 visiongraph/result/BaseResult.py
--rw-r--r--  2.0 unx      525 b- defN 23-Apr-14 15:29 visiongraph/result/CameraPoseResult.py
--rw-r--r--  2.0 unx      378 b- defN 23-Apr-14 15:29 visiongraph/result/ClassificationResult.py
--rw-r--r--  2.0 unx     1709 b- defN 23-Apr-14 15:29 visiongraph/result/DepthMap.py
--rw-r--r--  2.0 unx      487 b- defN 23-Apr-14 15:29 visiongraph/result/EmbeddingResult.py
--rw-r--r--  2.0 unx      474 b- defN 23-Apr-14 15:29 visiongraph/result/HeadPoseResult.py
--rw-r--r--  2.0 unx      333 b- defN 23-Apr-14 15:29 visiongraph/result/ImageResult.py
--rw-r--r--  2.0 unx     1165 b- defN 23-Apr-14 15:29 visiongraph/result/ResultAnnotator.py
--rw-r--r--  2.0 unx      483 b- defN 23-Apr-14 15:29 visiongraph/result/ResultDict.py
--rw-r--r--  2.0 unx      466 b- defN 23-Apr-14 15:29 visiongraph/result/ResultList.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/result/__init__.py
--rw-r--r--  2.0 unx      779 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/CrowdHumanResult.py
--rw-r--r--  2.0 unx     1354 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/InstanceSegmentationResult.py
--rw-r--r--  2.0 unx     4199 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/LandmarkDetectionResult.py
--rw-r--r--  2.0 unx     3475 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/ObjectDetectionResult.py
--rw-r--r--  2.0 unx      878 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/SpatialCascadeResult.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/__init__.py
--rw-r--r--  2.0 unx      924 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/face/BlazeFace.py
--rw-r--r--  2.0 unx     2064 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/face/BlazeFaceMesh.py
--rw-r--r--  2.0 unx      702 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/face/EmotionClassificationResult.py
--rw-r--r--  2.0 unx      409 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/face/FaceDetectionResult.py
--rw-r--r--  2.0 unx      881 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/face/FaceLandmarkResult.py
--rw-r--r--  2.0 unx     1390 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/face/IrisDistanceResult.py
--rw-r--r--  2.0 unx      868 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/face/RegressionFace.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/face/__init__.py
--rw-r--r--  2.0 unx     2648 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/hand/BlazeHand.py
--rw-r--r--  2.0 unx      409 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/hand/HandDetectionResult.py
--rw-r--r--  2.0 unx     2590 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/hand/HandLandmarkResult.py
--rw-r--r--  2.0 unx       88 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/hand/Handedness.py
--rw-r--r--  2.0 unx      106 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/hand/OpenPoseHand.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/hand/__init__.py
--rw-r--r--  2.0 unx     3435 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/pose/BlazePose.py
--rw-r--r--  2.0 unx     1266 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/pose/BlazePoseSegmentation.py
--rw-r--r--  2.0 unx     2826 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/pose/COCOOpenPose.py
--rw-r--r--  2.0 unx     2680 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/pose/COCOPose.py
--rw-r--r--  2.0 unx     2337 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/pose/EfficientPose.py
--rw-r--r--  2.0 unx     2738 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/pose/MobileHumanPose.py
--rw-r--r--  2.0 unx     2823 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/pose/PoseLandmarkResult.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/pose/__init__.py
--rw-r--r--  2.0 unx      492 b- defN 23-Apr-14 15:29 visiongraph/tracker/BaseObjectDetectionTracker.py
--rw-r--r--  2.0 unx     1908 b- defN 23-Apr-14 15:29 visiongraph/tracker/CentroidTracker.py
--rw-r--r--  2.0 unx     4906 b- defN 23-Apr-14 15:29 visiongraph/tracker/FlateTracker.py
--rw-r--r--  2.0 unx     2705 b- defN 23-Apr-14 15:29 visiongraph/tracker/MotpyTracker.py
--rw-r--r--  2.0 unx     3299 b- defN 23-Apr-14 15:29 visiongraph/tracker/ObjectAssignmentSolver.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/tracker/__init__.py
--rw-r--r--  2.0 unx     3105 b- defN 23-Apr-14 15:29 visiongraph/util/ArgUtils.py
--rw-r--r--  2.0 unx     1009 b- defN 23-Apr-14 15:29 visiongraph/util/CodeUtils.py
--rw-r--r--  2.0 unx      222 b- defN 23-Apr-14 15:29 visiongraph/util/CollectionUtils.py
--rw-r--r--  2.0 unx      314 b- defN 23-Apr-14 15:29 visiongraph/util/CommonArgs.py
--rw-r--r--  2.0 unx     3653 b- defN 23-Apr-14 15:29 visiongraph/util/DrawingUtils.py
--rw-r--r--  2.0 unx     3588 b- defN 23-Apr-14 15:29 visiongraph/util/ImageUtils.py
--rw-r--r--  2.0 unx     2608 b- defN 23-Apr-14 15:29 visiongraph/util/LinalgUtils.py
--rw-r--r--  2.0 unx      539 b- defN 23-Apr-14 15:29 visiongraph/util/LoggingUtils.py
--rw-r--r--  2.0 unx     1752 b- defN 23-Apr-14 15:29 visiongraph/util/MathUtils.py
--rw-r--r--  2.0 unx     2084 b- defN 23-Apr-14 15:29 visiongraph/util/NetworkUtils.py
--rw-r--r--  2.0 unx      195 b- defN 23-Apr-14 15:29 visiongraph/util/OSUtils.py
--rw-r--r--  2.0 unx      704 b- defN 23-Apr-14 15:29 visiongraph/util/OpenVinoUtils.py
--rw-r--r--  2.0 unx     1240 b- defN 23-Apr-14 15:29 visiongraph/util/ResultUtils.py
--rw-r--r--  2.0 unx     2102 b- defN 23-Apr-14 15:29 visiongraph/util/TimeUtils.py
--rw-r--r--  2.0 unx     3225 b- defN 23-Apr-14 15:29 visiongraph/util/VectorUtils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/util/__init__.py
--rw-r--r--  2.0 unx    11845 b- defN 23-Apr-14 15:30 visiongraph-0.1.44.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 15:30 visiongraph-0.1.44.dist-info/WHEEL
--rw-r--r--  2.0 unx       66 b- defN 23-Apr-14 15:30 visiongraph-0.1.44.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 23-Apr-14 15:30 visiongraph-0.1.44.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    26401 b- defN 23-Apr-14 15:30 visiongraph-0.1.44.dist-info/RECORD
-265 files, 661344 bytes uncompressed, 198561 bytes compressed:  70.0%
+Zip file size: 240119 bytes, number of entries: 262
+-rw-r--r--  2.0 unx     1758 b- defN 23-Apr-14 20:00 visiongraph/AsyncGraphNode.py
+-rw-r--r--  2.0 unx     2806 b- defN 23-Apr-14 20:00 visiongraph/BaseGraph.py
+-rw-r--r--  2.0 unx      678 b- defN 23-Apr-14 20:00 visiongraph/GraphNode.py
+-rw-r--r--  2.0 unx      276 b- defN 23-Apr-14 20:00 visiongraph/Processable.py
+-rw-r--r--  2.0 unx     2094 b- defN 23-Apr-14 20:00 visiongraph/VisionGraph.py
+-rw-r--r--  2.0 unx     1898 b- defN 23-Apr-14 20:00 visiongraph/VisionGraphBuilder.py
+-rw-r--r--  2.0 unx    23701 b- defN 23-Apr-14 20:00 visiongraph/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/cache/__init__.py
+-rw-r--r--  2.0 unx      368 b- defN 23-Apr-14 20:00 visiongraph/data/Asset.py
+-rw-r--r--  2.0 unx      376 b- defN 23-Apr-14 20:00 visiongraph/data/LocalAsset.py
+-rw-r--r--  2.0 unx     1099 b- defN 23-Apr-14 20:00 visiongraph/data/RepositoryAsset.py
+-rw-r--r--  2.0 unx      324 b- defN 23-Apr-14 20:00 visiongraph/data/__init__.py
+-rw-r--r--  2.0 unx     2568 b- defN 23-Apr-14 20:00 visiongraph/data/labels/COCO.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/data/labels/__init__.py
+-rw-r--r--  2.0 unx      172 b- defN 23-Apr-14 20:00 visiongraph/dsp/BaseFilterNumpy.py
+-rw-r--r--  2.0 unx     2421 b- defN 23-Apr-14 20:00 visiongraph/dsp/LandmarkSmoothFilter.py
+-rw-r--r--  2.0 unx     1487 b- defN 23-Apr-14 20:00 visiongraph/dsp/OneEuroFilter.py
+-rw-r--r--  2.0 unx     1651 b- defN 23-Apr-14 20:00 visiongraph/dsp/OneEuroFilterNumba.py
+-rw-r--r--  2.0 unx     2642 b- defN 23-Apr-14 20:00 visiongraph/dsp/OneEuroFilterNumpy.py
+-rw-r--r--  2.0 unx     1037 b- defN 23-Apr-14 20:00 visiongraph/dsp/VectorNumpySmoothFilter.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/dsp/__init__.py
+-rw-r--r--  2.0 unx      619 b- defN 23-Apr-14 20:00 visiongraph/estimator/BaseClassifier.py
+-rw-r--r--  2.0 unx      397 b- defN 23-Apr-14 20:00 visiongraph/estimator/BaseEstimator.py
+-rw-r--r--  2.0 unx     4091 b- defN 23-Apr-14 20:00 visiongraph/estimator/BaseVisionEngine.py
+-rw-r--r--  2.0 unx     1100 b- defN 23-Apr-14 20:00 visiongraph/estimator/ChainEstimator.py
+-rw-r--r--  2.0 unx      403 b- defN 23-Apr-14 20:00 visiongraph/estimator/ScoreThresholdEstimator.py
+-rw-r--r--  2.0 unx      868 b- defN 23-Apr-14 20:00 visiongraph/estimator/VisionClassifier.py
+-rw-r--r--  2.0 unx      410 b- defN 23-Apr-14 20:00 visiongraph/estimator/VisionEstimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/__init__.py
+-rw-r--r--  2.0 unx     2448 b- defN 23-Apr-14 20:00 visiongraph/estimator/calculator/UndistortionCalculator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/calculator/__init__.py
+-rw-r--r--  2.0 unx     1231 b- defN 23-Apr-14 20:00 visiongraph/estimator/engine/InferenceEngineFactory.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/engine/__init__.py
+-rw-r--r--  2.0 unx      529 b- defN 23-Apr-14 20:00 visiongraph/estimator/inpaint/BaseInpainter.py
+-rw-r--r--  2.0 unx     2161 b- defN 23-Apr-14 20:00 visiongraph/estimator/inpaint/GMCNNInpainter.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/inpaint/__init__.py
+-rw-r--r--  2.0 unx     2077 b- defN 23-Apr-14 20:00 visiongraph/estimator/onnx/ONNXVisionEngine.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/onnx/__init__.py
+-rw-r--r--  2.0 unx     2220 b- defN 23-Apr-14 20:00 visiongraph/estimator/openvino/OpenVinoEngine.py
+-rw-r--r--  2.0 unx     2516 b- defN 23-Apr-14 20:00 visiongraph/estimator/openvino/OpenVinoObjectDetector.py
+-rw-r--r--  2.0 unx     2967 b- defN 23-Apr-14 20:00 visiongraph/estimator/openvino/OpenVinoPoseEstimator.py
+-rw-r--r--  2.0 unx      726 b- defN 23-Apr-14 20:00 visiongraph/estimator/openvino/SyncInferencePipeline.py
+-rw-r--r--  2.0 unx     1703 b- defN 23-Apr-14 20:00 visiongraph/estimator/openvino/VisionInferenceEngine.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/openvino/__init__.py
+-rw-r--r--  2.0 unx     1750 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/CenterNetDetector.py
+-rw-r--r--  2.0 unx     3270 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/CrowdHumanDetector.py
+-rw-r--r--  2.0 unx     1781 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/DETRDetector.py
+-rw-r--r--  2.0 unx      544 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/InstanceSegmentationEstimator.py
+-rw-r--r--  2.0 unx      523 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/LandmarkEstimator.py
+-rw-r--r--  2.0 unx      524 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/ObjectDetector.py
+-rw-r--r--  2.0 unx     1279 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/RoiEstimator.py
+-rw-r--r--  2.0 unx     3147 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/SSDDetector.py
+-rw-r--r--  2.0 unx     2082 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/SlidingWindowEstimator.py
+-rw-r--r--  2.0 unx     1436 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/SpatialCascadeEstimator.py
+-rw-r--r--  2.0 unx     3173 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/YOLODetector.py
+-rw-r--r--  2.0 unx     3594 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/YOLOv5Detector.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/__init__.py
+-rw-r--r--  2.0 unx     3441 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/camera/ArUcoCameraPoseEstimator.py
+-rw-r--r--  2.0 unx      850 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/camera/BoardCameraCalibrator.py
+-rw-r--r--  2.0 unx     4276 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/camera/ChArUcoCalibrator.py
+-rw-r--r--  2.0 unx     3145 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/camera/ChessboardCalibrator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/camera/__init__.py
+-rw-r--r--  2.0 unx     1127 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/AdasFaceDetector.py
+-rw-r--r--  2.0 unx      512 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/FaceDetector.py
+-rw-r--r--  2.0 unx     3805 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/OpenVinoFaceDetector.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/__init__.py
+-rw-r--r--  2.0 unx     1781 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/emotion/AffectNetEmotionClassifier.py
+-rw-r--r--  2.0 unx     2038 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/emotion/FERPlusEmotionClassifier.py
+-rw-r--r--  2.0 unx      450 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/emotion/FaceEmotionEstimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/emotion/__init__.py
+-rw-r--r--  2.0 unx      609 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/landmark/FaceLandmarkEstimator.py
+-rw-r--r--  2.0 unx     2646 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/landmark/IrisDistanceCalculator.py
+-rw-r--r--  2.0 unx     2204 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/landmark/MediaPipeFaceDetector.py
+-rw-r--r--  2.0 unx     2324 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/landmark/MediaPipeFaceMeshEstimator.py
+-rw-r--r--  2.0 unx     1832 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/landmark/RegressionLandmarkEstimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/landmark/__init__.py
+-rw-r--r--  2.0 unx     1301 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/pose/AdasHeadPoseEstimator.py
+-rw-r--r--  2.0 unx      315 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/pose/HeadPoseEstimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/pose/__init__.py
+-rw-r--r--  2.0 unx     4265 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/recognition/FaceRecognitionEstimator.py
+-rw-r--r--  2.0 unx     2842 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/recognition/FaceReidentificationEstimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/face/recognition/__init__.py
+-rw-r--r--  2.0 unx      517 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/hand/HandDetector.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/hand/__init__.py
+-rw-r--r--  2.0 unx      608 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/hand/landmark/HandLandmarkEstimator.py
+-rw-r--r--  2.0 unx     2778 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/hand/landmark/MediaPipeHandEstimator.py
+-rw-r--r--  2.0 unx     2330 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/hand/landmark/OpenPoseHandEstimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/hand/landmark/__init__.py
+-rw-r--r--  2.0 unx     2086 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/pose/AEPoseEstimator.py
+-rw-r--r--  2.0 unx     5139 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/pose/EfficientPoseEstimator.py
+-rw-r--r--  2.0 unx     3890 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/pose/LiteHRNetEstimator.py
+-rw-r--r--  2.0 unx     2855 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/pose/LitePoseEstimator.py
+-rw-r--r--  2.0 unx     3100 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/pose/MediaPipePoseEstimator.py
+-rw-r--r--  2.0 unx     6641 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/pose/MobileHumanPoseEstimator.py
+-rw-r--r--  2.0 unx     9658 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/pose/MobileNetV2PoseEstimator.py
+-rw-r--r--  2.0 unx     4325 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/pose/MoveNetPoseEstimator.py
+-rw-r--r--  2.0 unx     1754 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/pose/OpenPoseEstimator.py
+-rw-r--r--  2.0 unx      518 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/pose/PoseEstimator.py
+-rw-r--r--  2.0 unx     2347 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/pose/TopDownPoseEstimator.py
+-rw-r--r--  2.0 unx     4815 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/pose/__init__.py
+-rw-r--r--  2.0 unx     7516 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/segmentation/MaskRCNNEstimator.py
+-rw-r--r--  2.0 unx     1989 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/segmentation/MediaPipeSelfieSegmentation.py
+-rw-r--r--  2.0 unx     3287 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/segmentation/YolactEstimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/spatial/segmentation/__init__.py
+-rw-r--r--  2.0 unx     1714 b- defN 23-Apr-14 20:00 visiongraph/estimator/translation/DeblurGANv2.py
+-rw-r--r--  2.0 unx      314 b- defN 23-Apr-14 20:00 visiongraph/estimator/translation/DepthEstimator.py
+-rw-r--r--  2.0 unx     2898 b- defN 23-Apr-14 20:00 visiongraph/estimator/translation/MidasDepthEstimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/estimator/translation/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/external/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/external/intel/__init__.py
+-rw-r--r--  2.0 unx     4337 b- defN 23-Apr-14 20:00 visiongraph/external/intel/performance_metrics.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/external/intel/adapters/__init__.py
+-rw-r--r--  2.0 unx     5682 b- defN 23-Apr-14 20:00 visiongraph/external/intel/adapters/inference_adapter.py
+-rw-r--r--  2.0 unx    15557 b- defN 23-Apr-14 20:00 visiongraph/external/intel/adapters/openvino_adapter.py
+-rw-r--r--  2.0 unx     7413 b- defN 23-Apr-14 20:00 visiongraph/external/intel/adapters/ovms_adapter.py
+-rw-r--r--  2.0 unx    10920 b- defN 23-Apr-14 20:00 visiongraph/external/intel/adapters/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/external/intel/models/__init__.py
+-rw-r--r--  2.0 unx     7582 b- defN 23-Apr-14 20:00 visiongraph/external/intel/models/centernet.py
+-rw-r--r--  2.0 unx     6784 b- defN 23-Apr-14 20:00 visiongraph/external/intel/models/detection_model.py
+-rw-r--r--  2.0 unx     3215 b- defN 23-Apr-14 20:00 visiongraph/external/intel/models/detr.py
+-rw-r--r--  2.0 unx    16363 b- defN 23-Apr-14 20:00 visiongraph/external/intel/models/hpe_associative_embedding.py
+-rw-r--r--  2.0 unx     8434 b- defN 23-Apr-14 20:00 visiongraph/external/intel/models/image_model.py
+-rw-r--r--  2.0 unx    19269 b- defN 23-Apr-14 20:00 visiongraph/external/intel/models/model.py
+-rw-r--r--  2.0 unx    19768 b- defN 23-Apr-14 20:00 visiongraph/external/intel/models/open_pose.py
+-rw-r--r--  2.0 unx     5995 b- defN 23-Apr-14 20:00 visiongraph/external/intel/models/ssd.py
+-rw-r--r--  2.0 unx     7510 b- defN 23-Apr-14 20:00 visiongraph/external/intel/models/types.py
+-rw-r--r--  2.0 unx     7600 b- defN 23-Apr-14 20:00 visiongraph/external/intel/models/utils.py
+-rw-r--r--  2.0 unx    24161 b- defN 23-Apr-14 20:00 visiongraph/external/intel/models/yolo.py
+-rw-r--r--  2.0 unx      154 b- defN 23-Apr-14 20:00 visiongraph/external/intel/pipelines/__init__.py
+-rw-r--r--  2.0 unx     5407 b- defN 23-Apr-14 20:00 visiongraph/external/intel/pipelines/async_pipeline.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/external/midas/__init__.py
+-rw-r--r--  2.0 unx     7868 b- defN 23-Apr-14 20:00 visiongraph/external/midas/transforms.py
+-rw-r--r--  2.0 unx      193 b- defN 23-Apr-14 20:00 visiongraph/external/motpy/__init__.py
+-rw-r--r--  2.0 unx     1816 b- defN 23-Apr-14 20:00 visiongraph/external/motpy/core.py
+-rw-r--r--  2.0 unx      333 b- defN 23-Apr-14 20:00 visiongraph/external/motpy/detector.py
+-rw-r--r--  2.0 unx     1147 b- defN 23-Apr-14 20:00 visiongraph/external/motpy/metrics.py
+-rw-r--r--  2.0 unx     5402 b- defN 23-Apr-14 20:00 visiongraph/external/motpy/model.py
+-rw-r--r--  2.0 unx     3576 b- defN 23-Apr-14 20:00 visiongraph/external/motpy/testing.py
+-rw-r--r--  2.0 unx     2647 b- defN 23-Apr-14 20:00 visiongraph/external/motpy/testing_viz.py
+-rw-r--r--  2.0 unx    16512 b- defN 23-Apr-14 20:00 visiongraph/external/motpy/tracker.py
+-rw-r--r--  2.0 unx      652 b- defN 23-Apr-14 20:00 visiongraph/external/motpy/utils.py
+-rw-r--r--  2.0 unx     5312 b- defN 23-Apr-14 20:00 visiongraph/external/motrackers/Track.py
+-rw-r--r--  2.0 unx     7486 b- defN 23-Apr-14 20:00 visiongraph/external/motrackers/Tracker.py
+-rw-r--r--  2.0 unx      184 b- defN 23-Apr-14 20:00 visiongraph/external/motrackers/__init__.py
+-rw-r--r--  2.0 unx       83 b- defN 23-Apr-14 20:00 visiongraph/external/motrackers/utils/__init__.py
+-rw-r--r--  2.0 unx     8978 b- defN 23-Apr-14 20:00 visiongraph/external/motrackers/utils/misc.py
+-rw-r--r--  2.0 unx    16025 b- defN 23-Apr-14 20:00 visiongraph/input/AzureKinectInput.py
+-rw-r--r--  2.0 unx     4108 b- defN 23-Apr-14 20:00 visiongraph/input/BaseDepthCamera.py
+-rw-r--r--  2.0 unx     1309 b- defN 23-Apr-14 20:00 visiongraph/input/BaseDepthInput.py
+-rw-r--r--  2.0 unx     3760 b- defN 23-Apr-14 20:00 visiongraph/input/BaseInput.py
+-rw-r--r--  2.0 unx     1721 b- defN 23-Apr-14 20:00 visiongraph/input/CamGearInput.py
+-rw-r--r--  2.0 unx     1493 b- defN 23-Apr-14 20:00 visiongraph/input/ImageInput.py
+-rw-r--r--  2.0 unx    18995 b- defN 23-Apr-14 20:00 visiongraph/input/RealSenseInput.py
+-rw-r--r--  2.0 unx     5032 b- defN 23-Apr-14 20:00 visiongraph/input/VideoCaptureInput.py
+-rw-r--r--  2.0 unx     1305 b- defN 23-Apr-14 20:00 visiongraph/input/__init__.py
+-rw-r--r--  2.0 unx     1887 b- defN 23-Apr-14 20:00 visiongraph/model/CameraIntrinsics.py
+-rw-r--r--  2.0 unx      101 b- defN 23-Apr-14 20:00 visiongraph/model/CameraStreamType.py
+-rw-r--r--  2.0 unx      549 b- defN 23-Apr-14 20:00 visiongraph/model/DepthBuffer.py
+-rw-r--r--  2.0 unx      753 b- defN 23-Apr-14 20:00 visiongraph/model/VisionEngineOutput.py
+-rw-r--r--  2.0 unx      135 b- defN 23-Apr-14 20:00 visiongraph/model/_ImportStub.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/model/__init__.py
+-rw-r--r--  2.0 unx     4229 b- defN 23-Apr-14 20:00 visiongraph/model/geometry/BoundingBox2D.py
+-rw-r--r--  2.0 unx      815 b- defN 23-Apr-14 20:00 visiongraph/model/geometry/Size2D.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/model/geometry/__init__.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Apr-14 20:00 visiongraph/model/parameter/ArgumentConfigurable.py
+-rw-r--r--  2.0 unx      186 b- defN 23-Apr-14 20:00 visiongraph/model/parameter/NamedParameter.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/model/parameter/__init__.py
+-rw-r--r--  2.0 unx      399 b- defN 23-Apr-14 20:00 visiongraph/model/tracker/Trackable.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/model/tracker/__init__.py
+-rw-r--r--  2.0 unx      440 b- defN 23-Apr-14 20:00 visiongraph/model/types/ModelPrecision.py
+-rw-r--r--  2.0 unx      199 b- defN 23-Apr-14 20:00 visiongraph/model/types/RealSenseColorScheme.py
+-rw-r--r--  2.0 unx      204 b- defN 23-Apr-14 20:00 visiongraph/model/types/RealSenseFilter.py
+-rw-r--r--  2.0 unx     1180 b- defN 23-Apr-14 20:00 visiongraph/model/types/VideoCaptureBackend.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/model/types/__init__.py
+-rw-r--r--  2.0 unx      905 b- defN 23-Apr-14 20:00 visiongraph/node/ApplyNode.py
+-rw-r--r--  2.0 unx      753 b- defN 23-Apr-14 20:00 visiongraph/node/BreakpointNode.py
+-rw-r--r--  2.0 unx      815 b- defN 23-Apr-14 20:00 visiongraph/node/CustomNode.py
+-rw-r--r--  2.0 unx      903 b- defN 23-Apr-14 20:00 visiongraph/node/ExtractNode.py
+-rw-r--r--  2.0 unx      525 b- defN 23-Apr-14 20:00 visiongraph/node/PassThroughNode.py
+-rw-r--r--  2.0 unx      825 b- defN 23-Apr-14 20:00 visiongraph/node/SequenceNode.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/node/__init__.py
+-rw-r--r--  2.0 unx     1471 b- defN 23-Apr-14 20:00 visiongraph/output/ImagePreview.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/output/__init__.py
+-rw-r--r--  2.0 unx      935 b- defN 23-Apr-14 20:00 visiongraph/output/fbs/FrameBufferSharingServer.py
+-rw-r--r--  2.0 unx     1390 b- defN 23-Apr-14 20:00 visiongraph/output/fbs/SpoutServer.py
+-rw-r--r--  2.0 unx     3287 b- defN 23-Apr-14 20:00 visiongraph/output/fbs/SyphonServer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/output/fbs/__init__.py
+-rw-r--r--  2.0 unx      980 b- defN 23-Apr-14 20:00 visiongraph/recorder/AsyncFrameSetRecorder.py
+-rw-r--r--  2.0 unx     1108 b- defN 23-Apr-14 20:00 visiongraph/recorder/BaseFrameRecorder.py
+-rw-r--r--  2.0 unx     1143 b- defN 23-Apr-14 20:00 visiongraph/recorder/CV2VideoRecorder.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-Apr-14 20:00 visiongraph/recorder/FrameSetRecorder.py
+-rw-r--r--  2.0 unx      905 b- defN 23-Apr-14 20:00 visiongraph/recorder/MoviePyVideoRecorder.py
+-rw-r--r--  2.0 unx     1377 b- defN 23-Apr-14 20:00 visiongraph/recorder/VidGearVideoRecorder.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/recorder/__init__.py
+-rw-r--r--  2.0 unx      564 b- defN 23-Apr-14 20:00 visiongraph/result/ArUcoCameraPose.py
+-rw-r--r--  2.0 unx     1521 b- defN 23-Apr-14 20:00 visiongraph/result/ArUcoMarkerDetection.py
+-rw-r--r--  2.0 unx      167 b- defN 23-Apr-14 20:00 visiongraph/result/BaseResult.py
+-rw-r--r--  2.0 unx      525 b- defN 23-Apr-14 20:00 visiongraph/result/CameraPoseResult.py
+-rw-r--r--  2.0 unx      378 b- defN 23-Apr-14 20:00 visiongraph/result/ClassificationResult.py
+-rw-r--r--  2.0 unx     1709 b- defN 23-Apr-14 20:00 visiongraph/result/DepthMap.py
+-rw-r--r--  2.0 unx      487 b- defN 23-Apr-14 20:00 visiongraph/result/EmbeddingResult.py
+-rw-r--r--  2.0 unx      474 b- defN 23-Apr-14 20:00 visiongraph/result/HeadPoseResult.py
+-rw-r--r--  2.0 unx      333 b- defN 23-Apr-14 20:00 visiongraph/result/ImageResult.py
+-rw-r--r--  2.0 unx     1165 b- defN 23-Apr-14 20:00 visiongraph/result/ResultAnnotator.py
+-rw-r--r--  2.0 unx      483 b- defN 23-Apr-14 20:00 visiongraph/result/ResultDict.py
+-rw-r--r--  2.0 unx      466 b- defN 23-Apr-14 20:00 visiongraph/result/ResultList.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/result/__init__.py
+-rw-r--r--  2.0 unx      779 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/CrowdHumanResult.py
+-rw-r--r--  2.0 unx     1354 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/InstanceSegmentationResult.py
+-rw-r--r--  2.0 unx     4199 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/LandmarkDetectionResult.py
+-rw-r--r--  2.0 unx     3475 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/ObjectDetectionResult.py
+-rw-r--r--  2.0 unx      878 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/SpatialCascadeResult.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/__init__.py
+-rw-r--r--  2.0 unx      924 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/face/BlazeFace.py
+-rw-r--r--  2.0 unx     2064 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/face/BlazeFaceMesh.py
+-rw-r--r--  2.0 unx      702 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/face/EmotionClassificationResult.py
+-rw-r--r--  2.0 unx      409 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/face/FaceDetectionResult.py
+-rw-r--r--  2.0 unx      881 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/face/FaceLandmarkResult.py
+-rw-r--r--  2.0 unx     1390 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/face/IrisDistanceResult.py
+-rw-r--r--  2.0 unx      868 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/face/RegressionFace.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/face/__init__.py
+-rw-r--r--  2.0 unx     2648 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/hand/BlazeHand.py
+-rw-r--r--  2.0 unx      409 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/hand/HandDetectionResult.py
+-rw-r--r--  2.0 unx     2590 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/hand/HandLandmarkResult.py
+-rw-r--r--  2.0 unx       88 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/hand/Handedness.py
+-rw-r--r--  2.0 unx      106 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/hand/OpenPoseHand.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/hand/__init__.py
+-rw-r--r--  2.0 unx     3435 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/pose/BlazePose.py
+-rw-r--r--  2.0 unx     1266 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/pose/BlazePoseSegmentation.py
+-rw-r--r--  2.0 unx     2826 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/pose/COCOOpenPose.py
+-rw-r--r--  2.0 unx     2680 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/pose/COCOPose.py
+-rw-r--r--  2.0 unx     2337 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/pose/EfficientPose.py
+-rw-r--r--  2.0 unx     2738 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/pose/MobileHumanPose.py
+-rw-r--r--  2.0 unx     2823 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/pose/PoseLandmarkResult.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/result/spatial/pose/__init__.py
+-rw-r--r--  2.0 unx      492 b- defN 23-Apr-14 20:00 visiongraph/tracker/BaseObjectDetectionTracker.py
+-rw-r--r--  2.0 unx     1908 b- defN 23-Apr-14 20:00 visiongraph/tracker/CentroidTracker.py
+-rw-r--r--  2.0 unx     4906 b- defN 23-Apr-14 20:00 visiongraph/tracker/FlateTracker.py
+-rw-r--r--  2.0 unx     2705 b- defN 23-Apr-14 20:00 visiongraph/tracker/MotpyTracker.py
+-rw-r--r--  2.0 unx     3299 b- defN 23-Apr-14 20:00 visiongraph/tracker/ObjectAssignmentSolver.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/tracker/__init__.py
+-rw-r--r--  2.0 unx     3105 b- defN 23-Apr-14 20:00 visiongraph/util/ArgUtils.py
+-rw-r--r--  2.0 unx     1009 b- defN 23-Apr-14 20:00 visiongraph/util/CodeUtils.py
+-rw-r--r--  2.0 unx      222 b- defN 23-Apr-14 20:00 visiongraph/util/CollectionUtils.py
+-rw-r--r--  2.0 unx      314 b- defN 23-Apr-14 20:00 visiongraph/util/CommonArgs.py
+-rw-r--r--  2.0 unx     3653 b- defN 23-Apr-14 20:00 visiongraph/util/DrawingUtils.py
+-rw-r--r--  2.0 unx     3588 b- defN 23-Apr-14 20:00 visiongraph/util/ImageUtils.py
+-rw-r--r--  2.0 unx     2608 b- defN 23-Apr-14 20:00 visiongraph/util/LinalgUtils.py
+-rw-r--r--  2.0 unx      539 b- defN 23-Apr-14 20:00 visiongraph/util/LoggingUtils.py
+-rw-r--r--  2.0 unx     1752 b- defN 23-Apr-14 20:00 visiongraph/util/MathUtils.py
+-rw-r--r--  2.0 unx     2084 b- defN 23-Apr-14 20:00 visiongraph/util/NetworkUtils.py
+-rw-r--r--  2.0 unx      195 b- defN 23-Apr-14 20:00 visiongraph/util/OSUtils.py
+-rw-r--r--  2.0 unx      704 b- defN 23-Apr-14 20:00 visiongraph/util/OpenVinoUtils.py
+-rw-r--r--  2.0 unx     1240 b- defN 23-Apr-14 20:00 visiongraph/util/ResultUtils.py
+-rw-r--r--  2.0 unx     2102 b- defN 23-Apr-14 20:00 visiongraph/util/TimeUtils.py
+-rw-r--r--  2.0 unx     3225 b- defN 23-Apr-14 20:00 visiongraph/util/VectorUtils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 20:00 visiongraph/util/__init__.py
+-rw-r--r--  2.0 unx    11847 b- defN 23-Apr-14 20:00 visiongraph-0.1.44.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 20:00 visiongraph-0.1.44.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Apr-14 20:00 visiongraph-0.1.44.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-14 20:00 visiongraph-0.1.44.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    26225 b- defN 23-Apr-14 20:00 visiongraph-0.1.44.1.dist-info/RECORD
+262 files, 657842 bytes uncompressed, 197103 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -1,19 +1,7 @@
-Filename: tools/CameraCalibratorTool.py
-Comment: 
-
-Filename: tools/OpenVinoModelRenamer.py
-Comment: 
-
-Filename: tools/__init__.py
-Comment: 
-
-Filename: tools/utils.py
-Comment: 
-
 Filename: visiongraph/AsyncGraphNode.py
 Comment: 
 
 Filename: visiongraph/BaseGraph.py
 Comment: 
 
 Filename: visiongraph/GraphNode.py
@@ -207,14 +195,17 @@
 
 Filename: visiongraph/estimator/spatial/face/__init__.py
 Comment: 
 
 Filename: visiongraph/estimator/spatial/face/emotion/AffectNetEmotionClassifier.py
 Comment: 
 
+Filename: visiongraph/estimator/spatial/face/emotion/FERPlusEmotionClassifier.py
+Comment: 
+
 Filename: visiongraph/estimator/spatial/face/emotion/FaceEmotionEstimator.py
 Comment: 
 
 Filename: visiongraph/estimator/spatial/face/emotion/__init__.py
 Comment: 
 
 Filename: visiongraph/estimator/spatial/face/landmark/FaceLandmarkEstimator.py
@@ -774,23 +765,23 @@
 
 Filename: visiongraph/util/VectorUtils.py
 Comment: 
 
 Filename: visiongraph/util/__init__.py
 Comment: 
 
-Filename: visiongraph-0.1.44.dist-info/METADATA
+Filename: visiongraph-0.1.44.1.dist-info/METADATA
 Comment: 
 
-Filename: visiongraph-0.1.44.dist-info/WHEEL
+Filename: visiongraph-0.1.44.1.dist-info/WHEEL
 Comment: 
 
-Filename: visiongraph-0.1.44.dist-info/entry_points.txt
+Filename: visiongraph-0.1.44.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: visiongraph-0.1.44.dist-info/top_level.txt
+Filename: visiongraph-0.1.44.1.dist-info/top_level.txt
 Comment: 
 
-Filename: visiongraph-0.1.44.dist-info/RECORD
+Filename: visiongraph-0.1.44.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## visiongraph/__init__.py

```diff
@@ -154,14 +154,18 @@
     from .estimator.spatial.face.OpenVinoFaceDetector import OpenVinoFaceDetector
 except ModuleNotFoundError as ex:
     logging.info(f"Module OpenVinoFaceDetector not found")
 try:
     from .estimator.spatial.face.emotion.AffectNetEmotionClassifier import AffectNetEmotionClassifier
 except ModuleNotFoundError as ex:
     logging.info(f"Module AffectNetEmotionClassifier not found")
+try:
+    from .estimator.spatial.face.emotion.FERPlusEmotionClassifier import FERPlusEmotionClassifier
+except ModuleNotFoundError as ex:
+    logging.info(f"Module FERPlusEmotionClassifier not found")
 from .estimator.spatial.face.emotion.FaceEmotionEstimator import FaceEmotionEstimator
 from .estimator.spatial.face.landmark.FaceLandmarkEstimator import FaceLandmarkEstimator
 try:
     from .estimator.spatial.face.landmark.IrisDistanceCalculator import IrisDistanceCalculator
 except ModuleNotFoundError as ex:
     logging.info(f"Module IrisDistanceCalculator not found")
 try:
```

## Comparing `visiongraph-0.1.44.dist-info/METADATA` & `visiongraph-0.1.44.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visiongraph
-Version: 0.1.44
+Version: 0.1.44.1
 Summary: Visiongraph is a high level computer vision framework.
 Home-page: https://github.com/cansik/visiongraph
 Author: Florian Bruggisser
 Author-email: github@broox.ch
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `visiongraph-0.1.44.dist-info/RECORD` & `visiongraph-0.1.44.1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-tools/CameraCalibratorTool.py,sha256=lhnYn-yLYnAH5Jl3l5XpUhAfvCoDl8K5ymPbI5xtieo,4275
-tools/OpenVinoModelRenamer.py,sha256=16t7-MkTm6JnZFVzS-nHfExfGD_6HLD96vHhzd9qDgc,1018
-tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tools/utils.py,sha256=cOX2YMHx5A9aVTeFjXRsyhNbCPavkCCyaw9cMNGvGg0,221
 visiongraph/AsyncGraphNode.py,sha256=sGVtD16mFM0okNXW9wdEHVJ9zzd7tD4gLFIA2lP4Wpo,1758
 visiongraph/BaseGraph.py,sha256=q_UPq53arsmW2wnZMo-jD9bGby2WFNTWwSBMvSLsxfU,2806
 visiongraph/GraphNode.py,sha256=o2uAgN4WknZV1b3gMIKF3TUFRahRRu7AdXiuXMX4hYI,678
 visiongraph/Processable.py,sha256=bhe_zj7nT2xgmD0xYM_BEWMmDlAUtjfsi3jfdLhMb60,276
 visiongraph/VisionGraph.py,sha256=d5EkjL24hmRteBXfSqZD9xfglkM4bDUIZl4GFlhADcQ,2094
 visiongraph/VisionGraphBuilder.py,sha256=i0bn8HLb3yRACeblpk4yFtMJ6hY61R46mFL1Pdkw_Vg,1898
-visiongraph/__init__.py,sha256=0f47zhxJW66wo7euwlCPrjeKE3CIjWYOVGSGXak7CWs,23501
+visiongraph/__init__.py,sha256=9hYKmkC7Crc7UpRG5Cpslp8khGBOinkGn3UKkykiqQ0,23701
 visiongraph/cache/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/data/Asset.py,sha256=N43JxIuOjCmW9CropssmFaXvrtIFnQ382YvXT2nfdlM,368
 visiongraph/data/LocalAsset.py,sha256=7AIWlgdwaWHBiC0RbooqpWoRf68nQx3AT0wWdfJ4hk8,376
 visiongraph/data/RepositoryAsset.py,sha256=D9Vmjn4qKjtUdHHryRHVVKaZZg8jWExZX2frDNt2NwE,1099
 visiongraph/data/__init__.py,sha256=-6VQqFg1a72cAwplIbNMVHTDMm7pXqh_-EuWr0gwgrY,324
 visiongraph/data/labels/COCO.py,sha256=4kP0wW4j16KIfdmCPhPNlQAnacZ3Etp2XC8LeECbe5A,2568
 visiongraph/data/labels/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -65,14 +61,15 @@
 visiongraph/estimator/spatial/camera/ChessboardCalibrator.py,sha256=8WN2RC93HRtlTz5bY0iNItGpOSBUGX58SAU7O-9T5JU,3145
 visiongraph/estimator/spatial/camera/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/estimator/spatial/face/AdasFaceDetector.py,sha256=I1vXSt9QviYl12jLdy6pUjjRGgFVLAh2v9MTPF7BBQo,1127
 visiongraph/estimator/spatial/face/FaceDetector.py,sha256=L_W5LFzrD1fqK7jbZSRlaphA3Yma0Q-sw2nctk72aYE,512
 visiongraph/estimator/spatial/face/OpenVinoFaceDetector.py,sha256=ZXw_wGa6VJ3HYMn9uE1ukYFrCwCq9Ijggmmu6LAAkSA,3805
 visiongraph/estimator/spatial/face/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/estimator/spatial/face/emotion/AffectNetEmotionClassifier.py,sha256=gOrT83tV8E4x-0uYDIj7xHmLRb-LsGyfwatiN1KXvwU,1781
+visiongraph/estimator/spatial/face/emotion/FERPlusEmotionClassifier.py,sha256=uG8rbg5f5WGd4fjqJok8DOAFwaDg_Qk1tQPu7b7P6io,2038
 visiongraph/estimator/spatial/face/emotion/FaceEmotionEstimator.py,sha256=8H_t4Eej-bxtNYsz8IserQxSaIdHCZSRy0Pyn8i4GoY,450
 visiongraph/estimator/spatial/face/emotion/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/estimator/spatial/face/landmark/FaceLandmarkEstimator.py,sha256=wheWNMlElKmtax-1brYwWVWIGdDb_Br7ogbM2uFX6U8,609
 visiongraph/estimator/spatial/face/landmark/IrisDistanceCalculator.py,sha256=EL0xwtMVDWQD79_vZsdWof9LPixxwC7_pDO0MMD_oHc,2646
 visiongraph/estimator/spatial/face/landmark/MediaPipeFaceDetector.py,sha256=__v18t7-RVut5NXOu7ypsZ2YpIrIdodprbIzJfJk8Lg,2204
 visiongraph/estimator/spatial/face/landmark/MediaPipeFaceMeshEstimator.py,sha256=rAWX83HyOV767H_g33Su5pUP-MgK_WOyHwT7GkWw2rc,2324
 visiongraph/estimator/spatial/face/landmark/RegressionLandmarkEstimator.py,sha256=f7dO2uuXvVsHQZKJMuZ0uGZWvuoyvID8JtuDMVm3KSc,1832
@@ -254,12 +251,12 @@
 visiongraph/util/NetworkUtils.py,sha256=JIYgwgTfbPfHmMtLGEZmouWUgRDkafmLJ78NlMb8eIQ,2084
 visiongraph/util/OSUtils.py,sha256=B1wbK-iZMKCfVJf1j_0GGAror2VEDto1aikTBnhcEqw,195
 visiongraph/util/OpenVinoUtils.py,sha256=aQNS4nHxi16TZArVqQLZNZMEwOuJR-lUEGBwT8zr6Es,704
 visiongraph/util/ResultUtils.py,sha256=ow5p1FtfIIuXo7VJMBQz0cuaG0nfZr0NO9LnTJrWgH8,1240
 visiongraph/util/TimeUtils.py,sha256=IVCLc5PtSYhmGB8hp6-oZMceva8Y6uU0K_1BDTZXGmE,2102
 visiongraph/util/VectorUtils.py,sha256=OSjJ1LGBQiEJp-wEocJvLXM1CyS09LesNA-H86Irnjw,3225
 visiongraph/util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-visiongraph-0.1.44.dist-info/METADATA,sha256=2MxSmg0jtddykiMTb9O5Mk9tc3TD5dMWsHoD4ozqSFs,11845
-visiongraph-0.1.44.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-visiongraph-0.1.44.dist-info/entry_points.txt,sha256=Oe-0WHEIftikIMS0mh3HdskyVa241gZLS1N7LHhb60A,66
-visiongraph-0.1.44.dist-info/top_level.txt,sha256=bRATNp8TOnl0xo3F0GYIhPVJh_W1FzO_tQyT-apCFgY,18
-visiongraph-0.1.44.dist-info/RECORD,,
+visiongraph-0.1.44.1.dist-info/METADATA,sha256=HggN3-UP4AHkrSZqG3Mbtta5IGt_QeIwnv63TSbIYZY,11847
+visiongraph-0.1.44.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+visiongraph-0.1.44.1.dist-info/entry_points.txt,sha256=eqGnTHtEVMYwfXVk1Z9MhC8O2N8wuqAbr0lisLmrkxs,20
+visiongraph-0.1.44.1.dist-info/top_level.txt,sha256=rMp8bfRr_CcL2T8juTpUUszIVf1_BFmagl0lhq3L16o,12
+visiongraph-0.1.44.1.dist-info/RECORD,,
```

