# Comparing `tmp/visiongraph-0.1.43-py3-none-any.whl.zip` & `tmp/visiongraph-0.1.44-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,260 +1,267 @@
-Zip file size: 235863 bytes, number of entries: 258
--rw-r--r--  2.0 unx     4270 b- defN 23-Mar-30 09:25 tools/CameraCalibratorTool.py
--rw-r--r--  2.0 unx     1018 b- defN 23-Mar-30 09:25 tools/OpenVinoModelRenamer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 tools/__init__.py
--rw-r--r--  2.0 unx      221 b- defN 23-Mar-30 09:25 tools/utils.py
--rw-r--r--  2.0 unx     1758 b- defN 23-Mar-30 09:25 visiongraph/AsyncGraphNode.py
--rw-r--r--  2.0 unx     2806 b- defN 23-Mar-30 09:25 visiongraph/BaseGraph.py
--rw-r--r--  2.0 unx      678 b- defN 23-Mar-30 09:25 visiongraph/GraphNode.py
--rw-r--r--  2.0 unx      276 b- defN 23-Mar-30 09:25 visiongraph/Processable.py
--rw-r--r--  2.0 unx     2094 b- defN 23-Mar-30 09:25 visiongraph/VisionGraph.py
--rw-r--r--  2.0 unx     1898 b- defN 23-Mar-30 09:25 visiongraph/VisionGraphBuilder.py
--rw-r--r--  2.0 unx    22210 b- defN 23-Mar-30 09:25 visiongraph/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/cache/__init__.py
--rw-r--r--  2.0 unx      368 b- defN 23-Mar-30 09:25 visiongraph/data/Asset.py
--rw-r--r--  2.0 unx      376 b- defN 23-Mar-30 09:25 visiongraph/data/LocalAsset.py
--rw-r--r--  2.0 unx     1099 b- defN 23-Mar-30 09:25 visiongraph/data/RepositoryAsset.py
--rw-r--r--  2.0 unx      324 b- defN 23-Mar-30 09:25 visiongraph/data/__init__.py
--rw-r--r--  2.0 unx     2568 b- defN 23-Mar-30 09:25 visiongraph/data/labels/COCO.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/data/labels/__init__.py
--rw-r--r--  2.0 unx      172 b- defN 23-Mar-30 09:25 visiongraph/dsp/BaseFilterNumpy.py
--rw-r--r--  2.0 unx     2421 b- defN 23-Mar-30 09:25 visiongraph/dsp/LandmarkSmoothFilter.py
--rw-r--r--  2.0 unx     1487 b- defN 23-Mar-30 09:25 visiongraph/dsp/OneEuroFilter.py
--rw-r--r--  2.0 unx     1651 b- defN 23-Mar-30 09:25 visiongraph/dsp/OneEuroFilterNumba.py
--rw-r--r--  2.0 unx     2642 b- defN 23-Mar-30 09:25 visiongraph/dsp/OneEuroFilterNumpy.py
--rw-r--r--  2.0 unx     1037 b- defN 23-Mar-30 09:25 visiongraph/dsp/VectorNumpySmoothFilter.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/dsp/__init__.py
--rw-r--r--  2.0 unx      619 b- defN 23-Mar-30 09:25 visiongraph/estimator/BaseClassifier.py
--rw-r--r--  2.0 unx      397 b- defN 23-Mar-30 09:25 visiongraph/estimator/BaseEstimator.py
--rw-r--r--  2.0 unx     4091 b- defN 23-Mar-30 09:25 visiongraph/estimator/BaseVisionEngine.py
--rw-r--r--  2.0 unx     1100 b- defN 23-Mar-30 09:25 visiongraph/estimator/ChainEstimator.py
--rw-r--r--  2.0 unx      403 b- defN 23-Mar-30 09:25 visiongraph/estimator/ScoreThresholdEstimator.py
--rw-r--r--  2.0 unx      868 b- defN 23-Mar-30 09:25 visiongraph/estimator/VisionClassifier.py
--rw-r--r--  2.0 unx      410 b- defN 23-Mar-30 09:25 visiongraph/estimator/VisionEstimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/estimator/__init__.py
--rw-r--r--  2.0 unx     2448 b- defN 23-Mar-30 09:25 visiongraph/estimator/calculator/UndistortionCalculator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/estimator/calculator/__init__.py
--rw-r--r--  2.0 unx      529 b- defN 23-Mar-30 09:25 visiongraph/estimator/inpaint/BaseInpainter.py
--rw-r--r--  2.0 unx     2161 b- defN 23-Mar-30 09:25 visiongraph/estimator/inpaint/GMCNNInpainter.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/estimator/inpaint/__init__.py
--rw-r--r--  2.0 unx     2108 b- defN 23-Mar-30 09:25 visiongraph/estimator/onnx/ONNXVisionEngine.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/estimator/onnx/__init__.py
--rw-r--r--  2.0 unx     2220 b- defN 23-Mar-30 09:25 visiongraph/estimator/openvino/OpenVinoEngine.py
--rw-r--r--  2.0 unx     2516 b- defN 23-Mar-30 09:25 visiongraph/estimator/openvino/OpenVinoObjectDetector.py
--rw-r--r--  2.0 unx     2967 b- defN 23-Mar-30 09:25 visiongraph/estimator/openvino/OpenVinoPoseEstimator.py
--rw-r--r--  2.0 unx      726 b- defN 23-Mar-30 09:25 visiongraph/estimator/openvino/SyncInferencePipeline.py
--rw-r--r--  2.0 unx     1703 b- defN 23-Mar-30 09:25 visiongraph/estimator/openvino/VisionInferenceEngine.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/estimator/openvino/__init__.py
--rw-r--r--  2.0 unx     1750 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/CenterNetDetector.py
--rw-r--r--  2.0 unx     1781 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/DETRDetector.py
--rw-r--r--  2.0 unx      544 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/InstanceSegmentationEstimator.py
--rw-r--r--  2.0 unx      523 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/LandmarkEstimator.py
--rw-r--r--  2.0 unx      524 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/ObjectDetector.py
--rw-r--r--  2.0 unx     1279 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/RoiEstimator.py
--rw-r--r--  2.0 unx     3147 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/SSDDetector.py
--rw-r--r--  2.0 unx     2082 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/SlidingWindowEstimator.py
--rw-r--r--  2.0 unx     1436 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/SpatialCascadeEstimator.py
--rw-r--r--  2.0 unx     3173 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/YOLODetector.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/__init__.py
--rw-r--r--  2.0 unx     3441 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/camera/ArUcoCameraPoseEstimator.py
--rw-r--r--  2.0 unx      850 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/camera/BoardCameraCalibrator.py
--rw-r--r--  2.0 unx     4276 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/camera/ChArUcoCalibrator.py
--rw-r--r--  2.0 unx     3145 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/camera/ChessboardCalibrator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/camera/__init__.py
--rw-r--r--  2.0 unx     1127 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/AdasFaceDetector.py
--rw-r--r--  2.0 unx      512 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/FaceDetector.py
--rw-r--r--  2.0 unx     3826 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/OpenVinoFaceDetector.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/__init__.py
--rw-r--r--  2.0 unx     1781 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/emotion/AffectNetEmotionClassifier.py
--rw-r--r--  2.0 unx      450 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/emotion/FaceEmotionEstimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/emotion/__init__.py
--rw-r--r--  2.0 unx      609 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/landmark/FaceLandmarkEstimator.py
--rw-r--r--  2.0 unx     2646 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/landmark/IrisDistanceCalculator.py
--rw-r--r--  2.0 unx     2204 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/landmark/MediaPipeFaceDetector.py
--rw-r--r--  2.0 unx     2324 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/landmark/MediaPipeFaceMeshEstimator.py
--rw-r--r--  2.0 unx     1832 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/landmark/RegressionLandmarkEstimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/landmark/__init__.py
--rw-r--r--  2.0 unx     1301 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/pose/AdasHeadPoseEstimator.py
--rw-r--r--  2.0 unx      315 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/pose/HeadPoseEstimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/pose/__init__.py
--rw-r--r--  2.0 unx     4265 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/recognition/FaceRecognitionEstimator.py
--rw-r--r--  2.0 unx     2842 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/recognition/FaceReidentificationEstimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/face/recognition/__init__.py
--rw-r--r--  2.0 unx      517 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/hand/HandDetector.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/hand/__init__.py
--rw-r--r--  2.0 unx      608 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/hand/landmark/HandLandmarkEstimator.py
--rw-r--r--  2.0 unx     2778 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/hand/landmark/MediaPipeHandEstimator.py
--rw-r--r--  2.0 unx     2330 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/hand/landmark/OpenPoseHandEstimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/hand/landmark/__init__.py
--rw-r--r--  2.0 unx     2086 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/pose/AEPoseEstimator.py
--rw-r--r--  2.0 unx     5139 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/pose/EfficientPoseEstimator.py
--rw-r--r--  2.0 unx     3890 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/pose/LiteHRNetEstimator.py
--rw-r--r--  2.0 unx     2855 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/pose/LitePoseEstimator.py
--rw-r--r--  2.0 unx     3100 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/pose/MediaPipePoseEstimator.py
--rw-r--r--  2.0 unx     6641 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/pose/MobileHumanPoseEstimator.py
--rw-r--r--  2.0 unx     9658 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/pose/MobileNetV2PoseEstimator.py
--rw-r--r--  2.0 unx     4325 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/pose/MoveNetPoseEstimator.py
--rw-r--r--  2.0 unx     1754 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/pose/OpenPoseEstimator.py
--rw-r--r--  2.0 unx      518 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/pose/PoseEstimator.py
--rw-r--r--  2.0 unx     2347 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/pose/TopDownPoseEstimator.py
--rw-r--r--  2.0 unx     4815 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/pose/__init__.py
--rw-r--r--  2.0 unx     7516 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/segmentation/MaskRCNNEstimator.py
--rw-r--r--  2.0 unx     1989 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/segmentation/MediaPipeSelfieSegmentation.py
--rw-r--r--  2.0 unx     3287 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/segmentation/YolactEstimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/estimator/spatial/segmentation/__init__.py
--rw-r--r--  2.0 unx     1648 b- defN 23-Mar-30 09:25 visiongraph/estimator/translation/DeblurGANv2.py
--rw-r--r--  2.0 unx      314 b- defN 23-Mar-30 09:25 visiongraph/estimator/translation/DepthEstimator.py
--rw-r--r--  2.0 unx     2898 b- defN 23-Mar-30 09:25 visiongraph/estimator/translation/MidasDepthEstimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/estimator/translation/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/external/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/external/intel/__init__.py
--rw-r--r--  2.0 unx     4337 b- defN 23-Mar-30 09:25 visiongraph/external/intel/performance_metrics.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/external/intel/adapters/__init__.py
--rw-r--r--  2.0 unx     5682 b- defN 23-Mar-30 09:25 visiongraph/external/intel/adapters/inference_adapter.py
--rw-r--r--  2.0 unx    15557 b- defN 23-Mar-30 09:25 visiongraph/external/intel/adapters/openvino_adapter.py
--rw-r--r--  2.0 unx     7413 b- defN 23-Mar-30 09:25 visiongraph/external/intel/adapters/ovms_adapter.py
--rw-r--r--  2.0 unx    10920 b- defN 23-Mar-30 09:25 visiongraph/external/intel/adapters/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/external/intel/models/__init__.py
--rw-r--r--  2.0 unx     7582 b- defN 23-Mar-30 09:25 visiongraph/external/intel/models/centernet.py
--rw-r--r--  2.0 unx     6784 b- defN 23-Mar-30 09:25 visiongraph/external/intel/models/detection_model.py
--rw-r--r--  2.0 unx     3215 b- defN 23-Mar-30 09:25 visiongraph/external/intel/models/detr.py
--rw-r--r--  2.0 unx    16363 b- defN 23-Mar-30 09:25 visiongraph/external/intel/models/hpe_associative_embedding.py
--rw-r--r--  2.0 unx     8434 b- defN 23-Mar-30 09:25 visiongraph/external/intel/models/image_model.py
--rw-r--r--  2.0 unx    19269 b- defN 23-Mar-30 09:25 visiongraph/external/intel/models/model.py
--rw-r--r--  2.0 unx    19768 b- defN 23-Mar-30 09:25 visiongraph/external/intel/models/open_pose.py
--rw-r--r--  2.0 unx     5995 b- defN 23-Mar-30 09:25 visiongraph/external/intel/models/ssd.py
--rw-r--r--  2.0 unx     7510 b- defN 23-Mar-30 09:25 visiongraph/external/intel/models/types.py
--rw-r--r--  2.0 unx     7600 b- defN 23-Mar-30 09:25 visiongraph/external/intel/models/utils.py
--rw-r--r--  2.0 unx    24161 b- defN 23-Mar-30 09:25 visiongraph/external/intel/models/yolo.py
--rw-r--r--  2.0 unx      154 b- defN 23-Mar-30 09:25 visiongraph/external/intel/pipelines/__init__.py
--rw-r--r--  2.0 unx     5407 b- defN 23-Mar-30 09:25 visiongraph/external/intel/pipelines/async_pipeline.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/external/midas/__init__.py
--rw-r--r--  2.0 unx     7868 b- defN 23-Mar-30 09:25 visiongraph/external/midas/transforms.py
--rw-r--r--  2.0 unx      193 b- defN 23-Mar-30 09:25 visiongraph/external/motpy/__init__.py
--rw-r--r--  2.0 unx     1816 b- defN 23-Mar-30 09:25 visiongraph/external/motpy/core.py
--rw-r--r--  2.0 unx      333 b- defN 23-Mar-30 09:25 visiongraph/external/motpy/detector.py
--rw-r--r--  2.0 unx     1147 b- defN 23-Mar-30 09:25 visiongraph/external/motpy/metrics.py
--rw-r--r--  2.0 unx     5402 b- defN 23-Mar-30 09:25 visiongraph/external/motpy/model.py
--rw-r--r--  2.0 unx     3576 b- defN 23-Mar-30 09:25 visiongraph/external/motpy/testing.py
--rw-r--r--  2.0 unx     2647 b- defN 23-Mar-30 09:25 visiongraph/external/motpy/testing_viz.py
--rw-r--r--  2.0 unx    16512 b- defN 23-Mar-30 09:25 visiongraph/external/motpy/tracker.py
--rw-r--r--  2.0 unx      652 b- defN 23-Mar-30 09:25 visiongraph/external/motpy/utils.py
--rw-r--r--  2.0 unx     5312 b- defN 23-Mar-30 09:25 visiongraph/external/motrackers/Track.py
--rw-r--r--  2.0 unx     7486 b- defN 23-Mar-30 09:25 visiongraph/external/motrackers/Tracker.py
--rw-r--r--  2.0 unx      184 b- defN 23-Mar-30 09:25 visiongraph/external/motrackers/__init__.py
--rw-r--r--  2.0 unx       83 b- defN 23-Mar-30 09:25 visiongraph/external/motrackers/utils/__init__.py
--rw-r--r--  2.0 unx     8978 b- defN 23-Mar-30 09:25 visiongraph/external/motrackers/utils/misc.py
--rw-r--r--  2.0 unx    16025 b- defN 23-Mar-30 09:25 visiongraph/input/AzureKinectInput.py
--rw-r--r--  2.0 unx     4108 b- defN 23-Mar-30 09:25 visiongraph/input/BaseDepthCamera.py
--rw-r--r--  2.0 unx     1309 b- defN 23-Mar-30 09:25 visiongraph/input/BaseDepthInput.py
--rw-r--r--  2.0 unx     3760 b- defN 23-Mar-30 09:25 visiongraph/input/BaseInput.py
--rw-r--r--  2.0 unx     1721 b- defN 23-Mar-30 09:25 visiongraph/input/CamGearInput.py
--rw-r--r--  2.0 unx     1493 b- defN 23-Mar-30 09:25 visiongraph/input/ImageInput.py
--rw-r--r--  2.0 unx    18995 b- defN 23-Mar-30 09:25 visiongraph/input/RealSenseInput.py
--rw-r--r--  2.0 unx     5032 b- defN 23-Mar-30 09:25 visiongraph/input/VideoCaptureInput.py
--rw-r--r--  2.0 unx     1305 b- defN 23-Mar-30 09:25 visiongraph/input/__init__.py
--rw-r--r--  2.0 unx     1520 b- defN 23-Mar-30 09:25 visiongraph/model/CameraIntrinsics.py
--rw-r--r--  2.0 unx      101 b- defN 23-Mar-30 09:25 visiongraph/model/CameraStreamType.py
--rw-r--r--  2.0 unx      549 b- defN 23-Mar-30 09:25 visiongraph/model/DepthBuffer.py
--rw-r--r--  2.0 unx      753 b- defN 23-Mar-30 09:25 visiongraph/model/VisionEngineOutput.py
--rw-r--r--  2.0 unx      135 b- defN 23-Mar-30 09:25 visiongraph/model/_ImportStub.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/model/__init__.py
--rw-r--r--  2.0 unx     3784 b- defN 23-Mar-30 09:25 visiongraph/model/geometry/BoundingBox2D.py
--rw-r--r--  2.0 unx      815 b- defN 23-Mar-30 09:25 visiongraph/model/geometry/Size2D.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/model/geometry/__init__.py
--rw-r--r--  2.0 unx      585 b- defN 23-Mar-30 09:25 visiongraph/model/parameter/ArgumentConfigurable.py
--rw-r--r--  2.0 unx      186 b- defN 23-Mar-30 09:25 visiongraph/model/parameter/NamedParameter.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/model/parameter/__init__.py
--rw-r--r--  2.0 unx      399 b- defN 23-Mar-30 09:25 visiongraph/model/tracker/Trackable.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/model/tracker/__init__.py
--rw-r--r--  2.0 unx      440 b- defN 23-Mar-30 09:25 visiongraph/model/types/ModelPrecision.py
--rw-r--r--  2.0 unx      199 b- defN 23-Mar-30 09:25 visiongraph/model/types/RealSenseColorScheme.py
--rw-r--r--  2.0 unx      204 b- defN 23-Mar-30 09:25 visiongraph/model/types/RealSenseFilter.py
--rw-r--r--  2.0 unx     1180 b- defN 23-Mar-30 09:25 visiongraph/model/types/VideoCaptureBackend.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/model/types/__init__.py
--rw-r--r--  2.0 unx      905 b- defN 23-Mar-30 09:25 visiongraph/node/ApplyNode.py
--rw-r--r--  2.0 unx      753 b- defN 23-Mar-30 09:25 visiongraph/node/BreakpointNode.py
--rw-r--r--  2.0 unx      815 b- defN 23-Mar-30 09:25 visiongraph/node/CustomNode.py
--rw-r--r--  2.0 unx      903 b- defN 23-Mar-30 09:25 visiongraph/node/ExtractNode.py
--rw-r--r--  2.0 unx      525 b- defN 23-Mar-30 09:25 visiongraph/node/PassThroughNode.py
--rw-r--r--  2.0 unx      825 b- defN 23-Mar-30 09:25 visiongraph/node/SequenceNode.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/node/__init__.py
--rw-r--r--  2.0 unx     1471 b- defN 23-Mar-30 09:25 visiongraph/output/ImagePreview.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/output/__init__.py
--rw-r--r--  2.0 unx      935 b- defN 23-Mar-30 09:25 visiongraph/output/fbs/FrameBufferSharingServer.py
--rw-r--r--  2.0 unx     1390 b- defN 23-Mar-30 09:25 visiongraph/output/fbs/SpoutServer.py
--rw-r--r--  2.0 unx     3123 b- defN 23-Mar-30 09:25 visiongraph/output/fbs/SyphonServer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/output/fbs/__init__.py
--rw-r--r--  2.0 unx      980 b- defN 23-Mar-30 09:25 visiongraph/recorder/AsyncFrameSetRecorder.py
--rw-r--r--  2.0 unx     1108 b- defN 23-Mar-30 09:25 visiongraph/recorder/BaseFrameRecorder.py
--rw-r--r--  2.0 unx     1143 b- defN 23-Mar-30 09:25 visiongraph/recorder/CV2VideoRecorder.py
--rw-r--r--  2.0 unx     1016 b- defN 23-Mar-30 09:25 visiongraph/recorder/FrameSetRecorder.py
--rw-r--r--  2.0 unx      905 b- defN 23-Mar-30 09:25 visiongraph/recorder/MoviePyVideoRecorder.py
--rw-r--r--  2.0 unx     1377 b- defN 23-Mar-30 09:25 visiongraph/recorder/VidGearVideoRecorder.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/recorder/__init__.py
--rw-r--r--  2.0 unx      564 b- defN 23-Mar-30 09:25 visiongraph/result/ArUcoCameraPose.py
--rw-r--r--  2.0 unx     1521 b- defN 23-Mar-30 09:25 visiongraph/result/ArUcoMarkerDetection.py
--rw-r--r--  2.0 unx      167 b- defN 23-Mar-30 09:25 visiongraph/result/BaseResult.py
--rw-r--r--  2.0 unx      525 b- defN 23-Mar-30 09:25 visiongraph/result/CameraPoseResult.py
--rw-r--r--  2.0 unx      378 b- defN 23-Mar-30 09:25 visiongraph/result/ClassificationResult.py
--rw-r--r--  2.0 unx     1709 b- defN 23-Mar-30 09:25 visiongraph/result/DepthMap.py
--rw-r--r--  2.0 unx      487 b- defN 23-Mar-30 09:25 visiongraph/result/EmbeddingResult.py
--rw-r--r--  2.0 unx      474 b- defN 23-Mar-30 09:25 visiongraph/result/HeadPoseResult.py
--rw-r--r--  2.0 unx      333 b- defN 23-Mar-30 09:25 visiongraph/result/ImageResult.py
--rw-r--r--  2.0 unx     1165 b- defN 23-Mar-30 09:25 visiongraph/result/ResultAnnotator.py
--rw-r--r--  2.0 unx      483 b- defN 23-Mar-30 09:25 visiongraph/result/ResultDict.py
--rw-r--r--  2.0 unx      466 b- defN 23-Mar-30 09:25 visiongraph/result/ResultList.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/result/__init__.py
--rw-r--r--  2.0 unx     1354 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/InstanceSegmentationResult.py
--rw-r--r--  2.0 unx     4199 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/LandmarkDetectionResult.py
--rw-r--r--  2.0 unx     3475 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/ObjectDetectionResult.py
--rw-r--r--  2.0 unx      878 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/SpatialCascadeResult.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/__init__.py
--rw-r--r--  2.0 unx      924 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/face/BlazeFace.py
--rw-r--r--  2.0 unx     2064 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/face/BlazeFaceMesh.py
--rw-r--r--  2.0 unx      702 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/face/EmotionClassificationResult.py
--rw-r--r--  2.0 unx      409 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/face/FaceDetectionResult.py
--rw-r--r--  2.0 unx      881 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/face/FaceLandmarkResult.py
--rw-r--r--  2.0 unx     1390 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/face/IrisDistanceResult.py
--rw-r--r--  2.0 unx      868 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/face/RegressionFace.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/face/__init__.py
--rw-r--r--  2.0 unx     2648 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/hand/BlazeHand.py
--rw-r--r--  2.0 unx      409 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/hand/HandDetectionResult.py
--rw-r--r--  2.0 unx     2590 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/hand/HandLandmarkResult.py
--rw-r--r--  2.0 unx       88 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/hand/Handedness.py
--rw-r--r--  2.0 unx      106 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/hand/OpenPoseHand.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/hand/__init__.py
--rw-r--r--  2.0 unx     3435 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/pose/BlazePose.py
--rw-r--r--  2.0 unx     1266 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/pose/BlazePoseSegmentation.py
--rw-r--r--  2.0 unx     2826 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/pose/COCOOpenPose.py
--rw-r--r--  2.0 unx     2680 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/pose/COCOPose.py
--rw-r--r--  2.0 unx     2337 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/pose/EfficientPose.py
--rw-r--r--  2.0 unx     2738 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/pose/MobileHumanPose.py
--rw-r--r--  2.0 unx     2823 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/pose/PoseLandmarkResult.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/result/spatial/pose/__init__.py
--rw-r--r--  2.0 unx      492 b- defN 23-Mar-30 09:25 visiongraph/tracker/BaseObjectDetectionTracker.py
--rw-r--r--  2.0 unx     1908 b- defN 23-Mar-30 09:25 visiongraph/tracker/CentroidTracker.py
--rw-r--r--  2.0 unx     4906 b- defN 23-Mar-30 09:25 visiongraph/tracker/FlateTracker.py
--rw-r--r--  2.0 unx     2705 b- defN 23-Mar-30 09:25 visiongraph/tracker/MotpyTracker.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/tracker/__init__.py
--rw-r--r--  2.0 unx     3105 b- defN 23-Mar-30 09:25 visiongraph/util/ArgUtils.py
--rw-r--r--  2.0 unx     1009 b- defN 23-Mar-30 09:25 visiongraph/util/CodeUtils.py
--rw-r--r--  2.0 unx      222 b- defN 23-Mar-30 09:25 visiongraph/util/CollectionUtils.py
--rw-r--r--  2.0 unx      314 b- defN 23-Mar-30 09:25 visiongraph/util/CommonArgs.py
--rw-r--r--  2.0 unx     3653 b- defN 23-Mar-30 09:25 visiongraph/util/DrawingUtils.py
--rw-r--r--  2.0 unx     3588 b- defN 23-Mar-30 09:25 visiongraph/util/ImageUtils.py
--rw-r--r--  2.0 unx     2608 b- defN 23-Mar-30 09:25 visiongraph/util/LinalgUtils.py
--rw-r--r--  2.0 unx      539 b- defN 23-Mar-30 09:25 visiongraph/util/LoggingUtils.py
--rw-r--r--  2.0 unx     1752 b- defN 23-Mar-30 09:25 visiongraph/util/MathUtils.py
--rw-r--r--  2.0 unx     2084 b- defN 23-Mar-30 09:25 visiongraph/util/NetworkUtils.py
--rw-r--r--  2.0 unx      704 b- defN 23-Mar-30 09:25 visiongraph/util/OpenVinoUtils.py
--rw-r--r--  2.0 unx     1132 b- defN 23-Mar-30 09:25 visiongraph/util/ResultUtils.py
--rw-r--r--  2.0 unx     2102 b- defN 23-Mar-30 09:25 visiongraph/util/TimeUtils.py
--rw-r--r--  2.0 unx     3225 b- defN 23-Mar-30 09:25 visiongraph/util/VectorUtils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 09:25 visiongraph/util/__init__.py
--rw-r--r--  2.0 unx    11889 b- defN 23-Mar-30 09:25 visiongraph-0.1.43.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-30 09:25 visiongraph-0.1.43.dist-info/WHEEL
--rw-r--r--  2.0 unx       66 b- defN 23-Mar-30 09:25 visiongraph-0.1.43.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 23-Mar-30 09:25 visiongraph-0.1.43.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    25697 b- defN 23-Mar-30 09:25 visiongraph-0.1.43.dist-info/RECORD
-258 files, 645922 bytes uncompressed, 193753 bytes compressed:  70.0%
+Zip file size: 241823 bytes, number of entries: 265
+-rw-r--r--  2.0 unx     4275 b- defN 23-Apr-14 15:29 tools/CameraCalibratorTool.py
+-rw-r--r--  2.0 unx     1018 b- defN 23-Apr-14 15:29 tools/OpenVinoModelRenamer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 tools/__init__.py
+-rw-r--r--  2.0 unx      221 b- defN 23-Apr-14 15:29 tools/utils.py
+-rw-r--r--  2.0 unx     1758 b- defN 23-Apr-14 15:29 visiongraph/AsyncGraphNode.py
+-rw-r--r--  2.0 unx     2806 b- defN 23-Apr-14 15:29 visiongraph/BaseGraph.py
+-rw-r--r--  2.0 unx      678 b- defN 23-Apr-14 15:29 visiongraph/GraphNode.py
+-rw-r--r--  2.0 unx      276 b- defN 23-Apr-14 15:29 visiongraph/Processable.py
+-rw-r--r--  2.0 unx     2094 b- defN 23-Apr-14 15:29 visiongraph/VisionGraph.py
+-rw-r--r--  2.0 unx     1898 b- defN 23-Apr-14 15:29 visiongraph/VisionGraphBuilder.py
+-rw-r--r--  2.0 unx    23501 b- defN 23-Apr-14 15:29 visiongraph/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/cache/__init__.py
+-rw-r--r--  2.0 unx      368 b- defN 23-Apr-14 15:29 visiongraph/data/Asset.py
+-rw-r--r--  2.0 unx      376 b- defN 23-Apr-14 15:29 visiongraph/data/LocalAsset.py
+-rw-r--r--  2.0 unx     1099 b- defN 23-Apr-14 15:29 visiongraph/data/RepositoryAsset.py
+-rw-r--r--  2.0 unx      324 b- defN 23-Apr-14 15:29 visiongraph/data/__init__.py
+-rw-r--r--  2.0 unx     2568 b- defN 23-Apr-14 15:29 visiongraph/data/labels/COCO.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/data/labels/__init__.py
+-rw-r--r--  2.0 unx      172 b- defN 23-Apr-14 15:29 visiongraph/dsp/BaseFilterNumpy.py
+-rw-r--r--  2.0 unx     2421 b- defN 23-Apr-14 15:29 visiongraph/dsp/LandmarkSmoothFilter.py
+-rw-r--r--  2.0 unx     1487 b- defN 23-Apr-14 15:29 visiongraph/dsp/OneEuroFilter.py
+-rw-r--r--  2.0 unx     1651 b- defN 23-Apr-14 15:29 visiongraph/dsp/OneEuroFilterNumba.py
+-rw-r--r--  2.0 unx     2642 b- defN 23-Apr-14 15:29 visiongraph/dsp/OneEuroFilterNumpy.py
+-rw-r--r--  2.0 unx     1037 b- defN 23-Apr-14 15:29 visiongraph/dsp/VectorNumpySmoothFilter.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/dsp/__init__.py
+-rw-r--r--  2.0 unx      619 b- defN 23-Apr-14 15:29 visiongraph/estimator/BaseClassifier.py
+-rw-r--r--  2.0 unx      397 b- defN 23-Apr-14 15:29 visiongraph/estimator/BaseEstimator.py
+-rw-r--r--  2.0 unx     4091 b- defN 23-Apr-14 15:29 visiongraph/estimator/BaseVisionEngine.py
+-rw-r--r--  2.0 unx     1100 b- defN 23-Apr-14 15:29 visiongraph/estimator/ChainEstimator.py
+-rw-r--r--  2.0 unx      403 b- defN 23-Apr-14 15:29 visiongraph/estimator/ScoreThresholdEstimator.py
+-rw-r--r--  2.0 unx      868 b- defN 23-Apr-14 15:29 visiongraph/estimator/VisionClassifier.py
+-rw-r--r--  2.0 unx      410 b- defN 23-Apr-14 15:29 visiongraph/estimator/VisionEstimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/__init__.py
+-rw-r--r--  2.0 unx     2448 b- defN 23-Apr-14 15:29 visiongraph/estimator/calculator/UndistortionCalculator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/calculator/__init__.py
+-rw-r--r--  2.0 unx     1231 b- defN 23-Apr-14 15:29 visiongraph/estimator/engine/InferenceEngineFactory.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/engine/__init__.py
+-rw-r--r--  2.0 unx      529 b- defN 23-Apr-14 15:29 visiongraph/estimator/inpaint/BaseInpainter.py
+-rw-r--r--  2.0 unx     2161 b- defN 23-Apr-14 15:29 visiongraph/estimator/inpaint/GMCNNInpainter.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/inpaint/__init__.py
+-rw-r--r--  2.0 unx     2077 b- defN 23-Apr-14 15:29 visiongraph/estimator/onnx/ONNXVisionEngine.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/onnx/__init__.py
+-rw-r--r--  2.0 unx     2220 b- defN 23-Apr-14 15:29 visiongraph/estimator/openvino/OpenVinoEngine.py
+-rw-r--r--  2.0 unx     2516 b- defN 23-Apr-14 15:29 visiongraph/estimator/openvino/OpenVinoObjectDetector.py
+-rw-r--r--  2.0 unx     2967 b- defN 23-Apr-14 15:29 visiongraph/estimator/openvino/OpenVinoPoseEstimator.py
+-rw-r--r--  2.0 unx      726 b- defN 23-Apr-14 15:29 visiongraph/estimator/openvino/SyncInferencePipeline.py
+-rw-r--r--  2.0 unx     1703 b- defN 23-Apr-14 15:29 visiongraph/estimator/openvino/VisionInferenceEngine.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/openvino/__init__.py
+-rw-r--r--  2.0 unx     1750 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/CenterNetDetector.py
+-rw-r--r--  2.0 unx     3270 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/CrowdHumanDetector.py
+-rw-r--r--  2.0 unx     1781 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/DETRDetector.py
+-rw-r--r--  2.0 unx      544 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/InstanceSegmentationEstimator.py
+-rw-r--r--  2.0 unx      523 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/LandmarkEstimator.py
+-rw-r--r--  2.0 unx      524 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/ObjectDetector.py
+-rw-r--r--  2.0 unx     1279 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/RoiEstimator.py
+-rw-r--r--  2.0 unx     3147 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/SSDDetector.py
+-rw-r--r--  2.0 unx     2082 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/SlidingWindowEstimator.py
+-rw-r--r--  2.0 unx     1436 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/SpatialCascadeEstimator.py
+-rw-r--r--  2.0 unx     3173 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/YOLODetector.py
+-rw-r--r--  2.0 unx     3594 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/YOLOv5Detector.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/__init__.py
+-rw-r--r--  2.0 unx     3441 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/camera/ArUcoCameraPoseEstimator.py
+-rw-r--r--  2.0 unx      850 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/camera/BoardCameraCalibrator.py
+-rw-r--r--  2.0 unx     4276 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/camera/ChArUcoCalibrator.py
+-rw-r--r--  2.0 unx     3145 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/camera/ChessboardCalibrator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/camera/__init__.py
+-rw-r--r--  2.0 unx     1127 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/AdasFaceDetector.py
+-rw-r--r--  2.0 unx      512 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/FaceDetector.py
+-rw-r--r--  2.0 unx     3805 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/OpenVinoFaceDetector.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/__init__.py
+-rw-r--r--  2.0 unx     1781 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/emotion/AffectNetEmotionClassifier.py
+-rw-r--r--  2.0 unx      450 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/emotion/FaceEmotionEstimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/emotion/__init__.py
+-rw-r--r--  2.0 unx      609 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/landmark/FaceLandmarkEstimator.py
+-rw-r--r--  2.0 unx     2646 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/landmark/IrisDistanceCalculator.py
+-rw-r--r--  2.0 unx     2204 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/landmark/MediaPipeFaceDetector.py
+-rw-r--r--  2.0 unx     2324 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/landmark/MediaPipeFaceMeshEstimator.py
+-rw-r--r--  2.0 unx     1832 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/landmark/RegressionLandmarkEstimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/landmark/__init__.py
+-rw-r--r--  2.0 unx     1301 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/pose/AdasHeadPoseEstimator.py
+-rw-r--r--  2.0 unx      315 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/pose/HeadPoseEstimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/pose/__init__.py
+-rw-r--r--  2.0 unx     4265 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/recognition/FaceRecognitionEstimator.py
+-rw-r--r--  2.0 unx     2842 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/recognition/FaceReidentificationEstimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/face/recognition/__init__.py
+-rw-r--r--  2.0 unx      517 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/hand/HandDetector.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/hand/__init__.py
+-rw-r--r--  2.0 unx      608 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/hand/landmark/HandLandmarkEstimator.py
+-rw-r--r--  2.0 unx     2778 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/hand/landmark/MediaPipeHandEstimator.py
+-rw-r--r--  2.0 unx     2330 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/hand/landmark/OpenPoseHandEstimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/hand/landmark/__init__.py
+-rw-r--r--  2.0 unx     2086 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/AEPoseEstimator.py
+-rw-r--r--  2.0 unx     5139 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/EfficientPoseEstimator.py
+-rw-r--r--  2.0 unx     3890 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/LiteHRNetEstimator.py
+-rw-r--r--  2.0 unx     2855 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/LitePoseEstimator.py
+-rw-r--r--  2.0 unx     3100 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/MediaPipePoseEstimator.py
+-rw-r--r--  2.0 unx     6641 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/MobileHumanPoseEstimator.py
+-rw-r--r--  2.0 unx     9658 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/MobileNetV2PoseEstimator.py
+-rw-r--r--  2.0 unx     4325 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/MoveNetPoseEstimator.py
+-rw-r--r--  2.0 unx     1754 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/OpenPoseEstimator.py
+-rw-r--r--  2.0 unx      518 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/PoseEstimator.py
+-rw-r--r--  2.0 unx     2347 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/TopDownPoseEstimator.py
+-rw-r--r--  2.0 unx     4815 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/pose/__init__.py
+-rw-r--r--  2.0 unx     7516 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/segmentation/MaskRCNNEstimator.py
+-rw-r--r--  2.0 unx     1989 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/segmentation/MediaPipeSelfieSegmentation.py
+-rw-r--r--  2.0 unx     3287 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/segmentation/YolactEstimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/spatial/segmentation/__init__.py
+-rw-r--r--  2.0 unx     1714 b- defN 23-Apr-14 15:29 visiongraph/estimator/translation/DeblurGANv2.py
+-rw-r--r--  2.0 unx      314 b- defN 23-Apr-14 15:29 visiongraph/estimator/translation/DepthEstimator.py
+-rw-r--r--  2.0 unx     2898 b- defN 23-Apr-14 15:29 visiongraph/estimator/translation/MidasDepthEstimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/estimator/translation/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/external/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/external/intel/__init__.py
+-rw-r--r--  2.0 unx     4337 b- defN 23-Apr-14 15:29 visiongraph/external/intel/performance_metrics.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/external/intel/adapters/__init__.py
+-rw-r--r--  2.0 unx     5682 b- defN 23-Apr-14 15:29 visiongraph/external/intel/adapters/inference_adapter.py
+-rw-r--r--  2.0 unx    15557 b- defN 23-Apr-14 15:29 visiongraph/external/intel/adapters/openvino_adapter.py
+-rw-r--r--  2.0 unx     7413 b- defN 23-Apr-14 15:29 visiongraph/external/intel/adapters/ovms_adapter.py
+-rw-r--r--  2.0 unx    10920 b- defN 23-Apr-14 15:29 visiongraph/external/intel/adapters/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/__init__.py
+-rw-r--r--  2.0 unx     7582 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/centernet.py
+-rw-r--r--  2.0 unx     6784 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/detection_model.py
+-rw-r--r--  2.0 unx     3215 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/detr.py
+-rw-r--r--  2.0 unx    16363 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/hpe_associative_embedding.py
+-rw-r--r--  2.0 unx     8434 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/image_model.py
+-rw-r--r--  2.0 unx    19269 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/model.py
+-rw-r--r--  2.0 unx    19768 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/open_pose.py
+-rw-r--r--  2.0 unx     5995 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/ssd.py
+-rw-r--r--  2.0 unx     7510 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/types.py
+-rw-r--r--  2.0 unx     7600 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/utils.py
+-rw-r--r--  2.0 unx    24161 b- defN 23-Apr-14 15:29 visiongraph/external/intel/models/yolo.py
+-rw-r--r--  2.0 unx      154 b- defN 23-Apr-14 15:29 visiongraph/external/intel/pipelines/__init__.py
+-rw-r--r--  2.0 unx     5407 b- defN 23-Apr-14 15:29 visiongraph/external/intel/pipelines/async_pipeline.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/external/midas/__init__.py
+-rw-r--r--  2.0 unx     7868 b- defN 23-Apr-14 15:29 visiongraph/external/midas/transforms.py
+-rw-r--r--  2.0 unx      193 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/__init__.py
+-rw-r--r--  2.0 unx     1816 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/core.py
+-rw-r--r--  2.0 unx      333 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/detector.py
+-rw-r--r--  2.0 unx     1147 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/metrics.py
+-rw-r--r--  2.0 unx     5402 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/model.py
+-rw-r--r--  2.0 unx     3576 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/testing.py
+-rw-r--r--  2.0 unx     2647 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/testing_viz.py
+-rw-r--r--  2.0 unx    16512 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/tracker.py
+-rw-r--r--  2.0 unx      652 b- defN 23-Apr-14 15:29 visiongraph/external/motpy/utils.py
+-rw-r--r--  2.0 unx     5312 b- defN 23-Apr-14 15:29 visiongraph/external/motrackers/Track.py
+-rw-r--r--  2.0 unx     7486 b- defN 23-Apr-14 15:29 visiongraph/external/motrackers/Tracker.py
+-rw-r--r--  2.0 unx      184 b- defN 23-Apr-14 15:29 visiongraph/external/motrackers/__init__.py
+-rw-r--r--  2.0 unx       83 b- defN 23-Apr-14 15:29 visiongraph/external/motrackers/utils/__init__.py
+-rw-r--r--  2.0 unx     8978 b- defN 23-Apr-14 15:29 visiongraph/external/motrackers/utils/misc.py
+-rw-r--r--  2.0 unx    16025 b- defN 23-Apr-14 15:29 visiongraph/input/AzureKinectInput.py
+-rw-r--r--  2.0 unx     4108 b- defN 23-Apr-14 15:29 visiongraph/input/BaseDepthCamera.py
+-rw-r--r--  2.0 unx     1309 b- defN 23-Apr-14 15:29 visiongraph/input/BaseDepthInput.py
+-rw-r--r--  2.0 unx     3760 b- defN 23-Apr-14 15:29 visiongraph/input/BaseInput.py
+-rw-r--r--  2.0 unx     1721 b- defN 23-Apr-14 15:29 visiongraph/input/CamGearInput.py
+-rw-r--r--  2.0 unx     1493 b- defN 23-Apr-14 15:29 visiongraph/input/ImageInput.py
+-rw-r--r--  2.0 unx    18995 b- defN 23-Apr-14 15:29 visiongraph/input/RealSenseInput.py
+-rw-r--r--  2.0 unx     5032 b- defN 23-Apr-14 15:29 visiongraph/input/VideoCaptureInput.py
+-rw-r--r--  2.0 unx     1305 b- defN 23-Apr-14 15:29 visiongraph/input/__init__.py
+-rw-r--r--  2.0 unx     1887 b- defN 23-Apr-14 15:29 visiongraph/model/CameraIntrinsics.py
+-rw-r--r--  2.0 unx      101 b- defN 23-Apr-14 15:29 visiongraph/model/CameraStreamType.py
+-rw-r--r--  2.0 unx      549 b- defN 23-Apr-14 15:29 visiongraph/model/DepthBuffer.py
+-rw-r--r--  2.0 unx      753 b- defN 23-Apr-14 15:29 visiongraph/model/VisionEngineOutput.py
+-rw-r--r--  2.0 unx      135 b- defN 23-Apr-14 15:29 visiongraph/model/_ImportStub.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/model/__init__.py
+-rw-r--r--  2.0 unx     4229 b- defN 23-Apr-14 15:29 visiongraph/model/geometry/BoundingBox2D.py
+-rw-r--r--  2.0 unx      815 b- defN 23-Apr-14 15:29 visiongraph/model/geometry/Size2D.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/model/geometry/__init__.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Apr-14 15:29 visiongraph/model/parameter/ArgumentConfigurable.py
+-rw-r--r--  2.0 unx      186 b- defN 23-Apr-14 15:29 visiongraph/model/parameter/NamedParameter.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/model/parameter/__init__.py
+-rw-r--r--  2.0 unx      399 b- defN 23-Apr-14 15:29 visiongraph/model/tracker/Trackable.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/model/tracker/__init__.py
+-rw-r--r--  2.0 unx      440 b- defN 23-Apr-14 15:29 visiongraph/model/types/ModelPrecision.py
+-rw-r--r--  2.0 unx      199 b- defN 23-Apr-14 15:29 visiongraph/model/types/RealSenseColorScheme.py
+-rw-r--r--  2.0 unx      204 b- defN 23-Apr-14 15:29 visiongraph/model/types/RealSenseFilter.py
+-rw-r--r--  2.0 unx     1180 b- defN 23-Apr-14 15:29 visiongraph/model/types/VideoCaptureBackend.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/model/types/__init__.py
+-rw-r--r--  2.0 unx      905 b- defN 23-Apr-14 15:29 visiongraph/node/ApplyNode.py
+-rw-r--r--  2.0 unx      753 b- defN 23-Apr-14 15:29 visiongraph/node/BreakpointNode.py
+-rw-r--r--  2.0 unx      815 b- defN 23-Apr-14 15:29 visiongraph/node/CustomNode.py
+-rw-r--r--  2.0 unx      903 b- defN 23-Apr-14 15:29 visiongraph/node/ExtractNode.py
+-rw-r--r--  2.0 unx      525 b- defN 23-Apr-14 15:29 visiongraph/node/PassThroughNode.py
+-rw-r--r--  2.0 unx      825 b- defN 23-Apr-14 15:29 visiongraph/node/SequenceNode.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/node/__init__.py
+-rw-r--r--  2.0 unx     1471 b- defN 23-Apr-14 15:29 visiongraph/output/ImagePreview.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/output/__init__.py
+-rw-r--r--  2.0 unx      935 b- defN 23-Apr-14 15:29 visiongraph/output/fbs/FrameBufferSharingServer.py
+-rw-r--r--  2.0 unx     1390 b- defN 23-Apr-14 15:29 visiongraph/output/fbs/SpoutServer.py
+-rw-r--r--  2.0 unx     3287 b- defN 23-Apr-14 15:29 visiongraph/output/fbs/SyphonServer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/output/fbs/__init__.py
+-rw-r--r--  2.0 unx      980 b- defN 23-Apr-14 15:29 visiongraph/recorder/AsyncFrameSetRecorder.py
+-rw-r--r--  2.0 unx     1108 b- defN 23-Apr-14 15:29 visiongraph/recorder/BaseFrameRecorder.py
+-rw-r--r--  2.0 unx     1143 b- defN 23-Apr-14 15:29 visiongraph/recorder/CV2VideoRecorder.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-Apr-14 15:29 visiongraph/recorder/FrameSetRecorder.py
+-rw-r--r--  2.0 unx      905 b- defN 23-Apr-14 15:29 visiongraph/recorder/MoviePyVideoRecorder.py
+-rw-r--r--  2.0 unx     1377 b- defN 23-Apr-14 15:29 visiongraph/recorder/VidGearVideoRecorder.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/recorder/__init__.py
+-rw-r--r--  2.0 unx      564 b- defN 23-Apr-14 15:29 visiongraph/result/ArUcoCameraPose.py
+-rw-r--r--  2.0 unx     1521 b- defN 23-Apr-14 15:29 visiongraph/result/ArUcoMarkerDetection.py
+-rw-r--r--  2.0 unx      167 b- defN 23-Apr-14 15:29 visiongraph/result/BaseResult.py
+-rw-r--r--  2.0 unx      525 b- defN 23-Apr-14 15:29 visiongraph/result/CameraPoseResult.py
+-rw-r--r--  2.0 unx      378 b- defN 23-Apr-14 15:29 visiongraph/result/ClassificationResult.py
+-rw-r--r--  2.0 unx     1709 b- defN 23-Apr-14 15:29 visiongraph/result/DepthMap.py
+-rw-r--r--  2.0 unx      487 b- defN 23-Apr-14 15:29 visiongraph/result/EmbeddingResult.py
+-rw-r--r--  2.0 unx      474 b- defN 23-Apr-14 15:29 visiongraph/result/HeadPoseResult.py
+-rw-r--r--  2.0 unx      333 b- defN 23-Apr-14 15:29 visiongraph/result/ImageResult.py
+-rw-r--r--  2.0 unx     1165 b- defN 23-Apr-14 15:29 visiongraph/result/ResultAnnotator.py
+-rw-r--r--  2.0 unx      483 b- defN 23-Apr-14 15:29 visiongraph/result/ResultDict.py
+-rw-r--r--  2.0 unx      466 b- defN 23-Apr-14 15:29 visiongraph/result/ResultList.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/result/__init__.py
+-rw-r--r--  2.0 unx      779 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/CrowdHumanResult.py
+-rw-r--r--  2.0 unx     1354 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/InstanceSegmentationResult.py
+-rw-r--r--  2.0 unx     4199 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/LandmarkDetectionResult.py
+-rw-r--r--  2.0 unx     3475 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/ObjectDetectionResult.py
+-rw-r--r--  2.0 unx      878 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/SpatialCascadeResult.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/__init__.py
+-rw-r--r--  2.0 unx      924 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/face/BlazeFace.py
+-rw-r--r--  2.0 unx     2064 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/face/BlazeFaceMesh.py
+-rw-r--r--  2.0 unx      702 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/face/EmotionClassificationResult.py
+-rw-r--r--  2.0 unx      409 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/face/FaceDetectionResult.py
+-rw-r--r--  2.0 unx      881 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/face/FaceLandmarkResult.py
+-rw-r--r--  2.0 unx     1390 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/face/IrisDistanceResult.py
+-rw-r--r--  2.0 unx      868 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/face/RegressionFace.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/face/__init__.py
+-rw-r--r--  2.0 unx     2648 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/hand/BlazeHand.py
+-rw-r--r--  2.0 unx      409 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/hand/HandDetectionResult.py
+-rw-r--r--  2.0 unx     2590 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/hand/HandLandmarkResult.py
+-rw-r--r--  2.0 unx       88 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/hand/Handedness.py
+-rw-r--r--  2.0 unx      106 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/hand/OpenPoseHand.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/hand/__init__.py
+-rw-r--r--  2.0 unx     3435 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/pose/BlazePose.py
+-rw-r--r--  2.0 unx     1266 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/pose/BlazePoseSegmentation.py
+-rw-r--r--  2.0 unx     2826 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/pose/COCOOpenPose.py
+-rw-r--r--  2.0 unx     2680 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/pose/COCOPose.py
+-rw-r--r--  2.0 unx     2337 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/pose/EfficientPose.py
+-rw-r--r--  2.0 unx     2738 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/pose/MobileHumanPose.py
+-rw-r--r--  2.0 unx     2823 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/pose/PoseLandmarkResult.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/result/spatial/pose/__init__.py
+-rw-r--r--  2.0 unx      492 b- defN 23-Apr-14 15:29 visiongraph/tracker/BaseObjectDetectionTracker.py
+-rw-r--r--  2.0 unx     1908 b- defN 23-Apr-14 15:29 visiongraph/tracker/CentroidTracker.py
+-rw-r--r--  2.0 unx     4906 b- defN 23-Apr-14 15:29 visiongraph/tracker/FlateTracker.py
+-rw-r--r--  2.0 unx     2705 b- defN 23-Apr-14 15:29 visiongraph/tracker/MotpyTracker.py
+-rw-r--r--  2.0 unx     3299 b- defN 23-Apr-14 15:29 visiongraph/tracker/ObjectAssignmentSolver.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/tracker/__init__.py
+-rw-r--r--  2.0 unx     3105 b- defN 23-Apr-14 15:29 visiongraph/util/ArgUtils.py
+-rw-r--r--  2.0 unx     1009 b- defN 23-Apr-14 15:29 visiongraph/util/CodeUtils.py
+-rw-r--r--  2.0 unx      222 b- defN 23-Apr-14 15:29 visiongraph/util/CollectionUtils.py
+-rw-r--r--  2.0 unx      314 b- defN 23-Apr-14 15:29 visiongraph/util/CommonArgs.py
+-rw-r--r--  2.0 unx     3653 b- defN 23-Apr-14 15:29 visiongraph/util/DrawingUtils.py
+-rw-r--r--  2.0 unx     3588 b- defN 23-Apr-14 15:29 visiongraph/util/ImageUtils.py
+-rw-r--r--  2.0 unx     2608 b- defN 23-Apr-14 15:29 visiongraph/util/LinalgUtils.py
+-rw-r--r--  2.0 unx      539 b- defN 23-Apr-14 15:29 visiongraph/util/LoggingUtils.py
+-rw-r--r--  2.0 unx     1752 b- defN 23-Apr-14 15:29 visiongraph/util/MathUtils.py
+-rw-r--r--  2.0 unx     2084 b- defN 23-Apr-14 15:29 visiongraph/util/NetworkUtils.py
+-rw-r--r--  2.0 unx      195 b- defN 23-Apr-14 15:29 visiongraph/util/OSUtils.py
+-rw-r--r--  2.0 unx      704 b- defN 23-Apr-14 15:29 visiongraph/util/OpenVinoUtils.py
+-rw-r--r--  2.0 unx     1240 b- defN 23-Apr-14 15:29 visiongraph/util/ResultUtils.py
+-rw-r--r--  2.0 unx     2102 b- defN 23-Apr-14 15:29 visiongraph/util/TimeUtils.py
+-rw-r--r--  2.0 unx     3225 b- defN 23-Apr-14 15:29 visiongraph/util/VectorUtils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 15:29 visiongraph/util/__init__.py
+-rw-r--r--  2.0 unx    11845 b- defN 23-Apr-14 15:30 visiongraph-0.1.44.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 15:30 visiongraph-0.1.44.dist-info/WHEEL
+-rw-r--r--  2.0 unx       66 b- defN 23-Apr-14 15:30 visiongraph-0.1.44.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-Apr-14 15:30 visiongraph-0.1.44.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    26401 b- defN 23-Apr-14 15:30 visiongraph-0.1.44.dist-info/RECORD
+265 files, 661344 bytes uncompressed, 198561 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -99,14 +99,20 @@
 
 Filename: visiongraph/estimator/calculator/UndistortionCalculator.py
 Comment: 
 
 Filename: visiongraph/estimator/calculator/__init__.py
 Comment: 
 
+Filename: visiongraph/estimator/engine/InferenceEngineFactory.py
+Comment: 
+
+Filename: visiongraph/estimator/engine/__init__.py
+Comment: 
+
 Filename: visiongraph/estimator/inpaint/BaseInpainter.py
 Comment: 
 
 Filename: visiongraph/estimator/inpaint/GMCNNInpainter.py
 Comment: 
 
 Filename: visiongraph/estimator/inpaint/__init__.py
@@ -135,14 +141,17 @@
 
 Filename: visiongraph/estimator/openvino/__init__.py
 Comment: 
 
 Filename: visiongraph/estimator/spatial/CenterNetDetector.py
 Comment: 
 
+Filename: visiongraph/estimator/spatial/CrowdHumanDetector.py
+Comment: 
+
 Filename: visiongraph/estimator/spatial/DETRDetector.py
 Comment: 
 
 Filename: visiongraph/estimator/spatial/InstanceSegmentationEstimator.py
 Comment: 
 
 Filename: visiongraph/estimator/spatial/LandmarkEstimator.py
@@ -162,14 +171,17 @@
 
 Filename: visiongraph/estimator/spatial/SpatialCascadeEstimator.py
 Comment: 
 
 Filename: visiongraph/estimator/spatial/YOLODetector.py
 Comment: 
 
+Filename: visiongraph/estimator/spatial/YOLOv5Detector.py
+Comment: 
+
 Filename: visiongraph/estimator/spatial/__init__.py
 Comment: 
 
 Filename: visiongraph/estimator/spatial/camera/ArUcoCameraPoseEstimator.py
 Comment: 
 
 Filename: visiongraph/estimator/spatial/camera/BoardCameraCalibrator.py
@@ -612,14 +624,17 @@
 
 Filename: visiongraph/result/ResultList.py
 Comment: 
 
 Filename: visiongraph/result/__init__.py
 Comment: 
 
+Filename: visiongraph/result/spatial/CrowdHumanResult.py
+Comment: 
+
 Filename: visiongraph/result/spatial/InstanceSegmentationResult.py
 Comment: 
 
 Filename: visiongraph/result/spatial/LandmarkDetectionResult.py
 Comment: 
 
 Filename: visiongraph/result/spatial/ObjectDetectionResult.py
@@ -705,14 +720,17 @@
 
 Filename: visiongraph/tracker/FlateTracker.py
 Comment: 
 
 Filename: visiongraph/tracker/MotpyTracker.py
 Comment: 
 
+Filename: visiongraph/tracker/ObjectAssignmentSolver.py
+Comment: 
+
 Filename: visiongraph/tracker/__init__.py
 Comment: 
 
 Filename: visiongraph/util/ArgUtils.py
 Comment: 
 
 Filename: visiongraph/util/CodeUtils.py
@@ -738,14 +756,17 @@
 
 Filename: visiongraph/util/MathUtils.py
 Comment: 
 
 Filename: visiongraph/util/NetworkUtils.py
 Comment: 
 
+Filename: visiongraph/util/OSUtils.py
+Comment: 
+
 Filename: visiongraph/util/OpenVinoUtils.py
 Comment: 
 
 Filename: visiongraph/util/ResultUtils.py
 Comment: 
 
 Filename: visiongraph/util/TimeUtils.py
@@ -753,23 +774,23 @@
 
 Filename: visiongraph/util/VectorUtils.py
 Comment: 
 
 Filename: visiongraph/util/__init__.py
 Comment: 
 
-Filename: visiongraph-0.1.43.dist-info/METADATA
+Filename: visiongraph-0.1.44.dist-info/METADATA
 Comment: 
 
-Filename: visiongraph-0.1.43.dist-info/WHEEL
+Filename: visiongraph-0.1.44.dist-info/WHEEL
 Comment: 
 
-Filename: visiongraph-0.1.43.dist-info/entry_points.txt
+Filename: visiongraph-0.1.44.dist-info/entry_points.txt
 Comment: 
 
-Filename: visiongraph-0.1.43.dist-info/top_level.txt
+Filename: visiongraph-0.1.44.dist-info/top_level.txt
 Comment: 
 
-Filename: visiongraph-0.1.43.dist-info/RECORD
+Filename: visiongraph-0.1.44.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tools/CameraCalibratorTool.py

```diff
@@ -13,15 +13,15 @@
 from visiongraph.estimator.spatial.camera.BoardCameraCalibrator import BoardCameraCalibrator
 from visiongraph.input import add_input_step_choices
 from visiongraph.input.BaseInput import BaseInput
 from visiongraph.util.LoggingUtils import add_logging_parameter
 
 BOARD_CALIBRATORS = {
     "chessboard": ChessboardCalibrator,
-    "charuco": ChArUcoCalibrator
+    # "charuco": ChArUcoCalibrator
 }
 
 
 class CameraCalibratorTool(BaseGraph):
 
     def __init__(self, input: BaseInput, calibrator: BoardCameraCalibrator):
         super().__init__()
@@ -106,15 +106,15 @@
 def main():
     parser = argparse.ArgumentParser("Camera Calibrator Tool", description="Calibrate cameras with boards.")
     add_logging_parameter(parser)
     input_group = parser.add_argument_group("input provider")
     add_input_step_choices(input_group)
 
     add_step_choice_argument(parser, BOARD_CALIBRATORS, "--calibrator", help="Board calibrator system.",
-                             default="charuco", add_params=True)
+                             default="chessboard", add_params=True)
     CameraCalibratorTool.add_params(parser)
 
     args = parser.parse_args()
 
     pipeline = CameraCalibratorTool(args.input(), args.calibrator(6, 7))
     pipeline.configure(args)
     pipeline.open()
```

## visiongraph/__init__.py

```diff
@@ -28,14 +28,22 @@
 from .estimator.BaseEstimator import BaseEstimator
 from .estimator.BaseVisionEngine import BaseVisionEngine
 from .estimator.ChainEstimator import ChainEstimator
 from .estimator.ScoreThresholdEstimator import ScoreThresholdEstimator
 from .estimator.VisionClassifier import VisionClassifier
 from .estimator.VisionEstimator import VisionEstimator
 from .estimator.calculator.UndistortionCalculator import UndistortionCalculator
+try:
+    from .estimator.engine.InferenceEngineFactory import InferenceEngine
+except ModuleNotFoundError as ex:
+    logging.info(f"Module InferenceEngine not found")
+try:
+    from .estimator.engine.InferenceEngineFactory import InferenceEngineFactory
+except ModuleNotFoundError as ex:
+    logging.info(f"Module InferenceEngineFactory not found")
 from .estimator.inpaint.BaseInpainter import BaseInpainter
 try:
     from .estimator.inpaint.GMCNNInpainter import GMCNNConfig
 except ModuleNotFoundError as ex:
     logging.info(f"Module GMCNNConfig not found")
 try:
     from .estimator.inpaint.GMCNNInpainter import GMCNNInpainter
@@ -66,14 +74,22 @@
 except ModuleNotFoundError as ex:
     logging.info(f"Module CenterNetConfig not found")
 try:
     from .estimator.spatial.CenterNetDetector import CenterNetDetector
 except ModuleNotFoundError as ex:
     logging.info(f"Module CenterNetDetector not found")
 try:
+    from .estimator.spatial.CrowdHumanDetector import CrowdHumanConfig
+except ModuleNotFoundError as ex:
+    logging.info(f"Module CrowdHumanConfig not found")
+try:
+    from .estimator.spatial.CrowdHumanDetector import CrowdHumanDetector
+except ModuleNotFoundError as ex:
+    logging.info(f"Module CrowdHumanDetector not found")
+try:
     from .estimator.spatial.DETRDetector import DETRConfig
 except ModuleNotFoundError as ex:
     logging.info(f"Module DETRConfig not found")
 try:
     from .estimator.spatial.DETRDetector import DETRDetector
 except ModuleNotFoundError as ex:
     logging.info(f"Module DETRDetector not found")
@@ -100,14 +116,22 @@
 except ModuleNotFoundError as ex:
     logging.info(f"Module YOLOConfig not found")
 try:
     from .estimator.spatial.YOLODetector import YOLODetector
 except ModuleNotFoundError as ex:
     logging.info(f"Module YOLODetector not found")
 try:
+    from .estimator.spatial.YOLOv5Detector import YOLOv5Config
+except ModuleNotFoundError as ex:
+    logging.info(f"Module YOLOv5Config not found")
+try:
+    from .estimator.spatial.YOLOv5Detector import YOLOv5Detector
+except ModuleNotFoundError as ex:
+    logging.info(f"Module YOLOv5Detector not found")
+try:
     from .estimator.spatial.camera.ArUcoCameraPoseEstimator import ArUcoCameraPoseEstimator
 except ModuleNotFoundError as ex:
     logging.info(f"Module ArUcoCameraPoseEstimator not found")
 from .estimator.spatial.camera.BoardCameraCalibrator import BoardCameraCalibrator
 try:
     from .estimator.spatial.camera.ChArUcoCalibrator import ChArUcoCalibrator
 except ModuleNotFoundError as ex:
@@ -358,14 +382,15 @@
 from .result.DepthMap import DepthMap
 from .result.EmbeddingResult import EmbeddingResult
 from .result.HeadPoseResult import HeadPoseResult
 from .result.ImageResult import ImageResult
 from .result.ResultAnnotator import ResultAnnotator
 from .result.ResultDict import ResultDict
 from .result.ResultList import ResultList
+from .result.spatial.CrowdHumanResult import CrowdHumanResult
 from .result.spatial.InstanceSegmentationResult import InstanceSegmentationResult
 from .result.spatial.LandmarkDetectionResult import LandmarkDetectionResult
 from .result.spatial.ObjectDetectionResult import ObjectDetectionResult
 from .result.spatial.SpatialCascadeResult import SpatialCascadeResult
 from .result.spatial.face.BlazeFace import BlazeFace
 try:
     from .result.spatial.face.BlazeFaceMesh import BlazeFaceMesh
@@ -401,14 +426,16 @@
 from .result.spatial.pose.EfficientPose import EfficientPose
 from .result.spatial.pose.MobileHumanPose import MobileHumanPose
 from .result.spatial.pose.PoseLandmarkResult import PoseLandmarkResult
 from .tracker.BaseObjectDetectionTracker import BaseObjectDetectionTracker
 from .tracker.CentroidTracker import CentroidTracker
 from .tracker.FlateTracker import FlateTracker
 from .tracker.MotpyTracker import MotpyTracker
+from .tracker.ObjectAssignmentSolver import ObjectAssignmentResult
+from .tracker.ObjectAssignmentSolver import ObjectAssignmentSolver
 from .util.ArgUtils import PipelineNodeFactory
 from .util.ArgUtils import add_dict_choice_argument
 from .util.ArgUtils import add_enum_choice_argument
 from .util.ArgUtils import add_step_choice_argument
 from .util.ArgUtils import dict_choice
 from .util.ArgUtils import float_range
 from .util.CodeUtils import deprecated
@@ -433,14 +460,17 @@
 from .util.MathUtils import constrain
 from .util.MathUtils import map_value
 from .util.MathUtils import rotate_2d
 from .util.MathUtils import transform_coordinates
 from .util.NetworkUtils import download_file
 from .util.NetworkUtils import prepare_data_file
 from .util.NetworkUtils import prepare_openvino_model
+from .util.OSUtils import isLinux
+from .util.OSUtils import isMacOSX
+from .util.OSUtils import isWindows
 try:
     from .util.OpenVinoUtils import get_inference_engine_device
 except ModuleNotFoundError as ex:
     logging.info(f"Module get_inference_engine_device not found")
 from .util.ResultUtils import extract_object_detection_roi
 from .util.ResultUtils import non_maximum_suppression
 from .util.TimeUtils import FPSTracer
```

## visiongraph/estimator/onnx/ONNXVisionEngine.py

```diff
@@ -21,17 +21,15 @@
         self.execution_providers = execution_providers
 
         self.session: Optional[rt.InferenceSession] = None
         self.session_options = rt.SessionOptions()
 
     def setup(self):
         if self.execution_providers is None:
-            self.execution_providers = ["CUDAExecutionProvider",
-                                        "OpenVINOExecutionProvider",
-                                        "CPUExecutionProvider"]
+            self.execution_providers = self.get_execution_providers()
 
         self.session = rt.InferenceSession(self.model.path,
                                            providers=self.execution_providers,
                                            sess_options=self.session_options)
 
         # read input infos
         self.input_names = [e.name for e in self.session.get_inputs()]
@@ -47,7 +45,10 @@
             if input.name == input_name:
                 return input.shape
 
         return []
 
     def release(self):
         self.session = None
+
+    def get_execution_providers(self) -> List[str]:
+        return rt.get_available_providers()
```

## visiongraph/estimator/spatial/face/OpenVinoFaceDetector.py

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 from typing import List, Dict, Tuple, Optional
 
 import numpy as np
 
 from visiongraph.data.Asset import Asset
 from visiongraph.data.RepositoryAsset import RepositoryAsset
-from visiongraph.estimator.openvino.VisionInferenceEngine import VisionInferenceEngine
+from visiongraph.estimator.openvino.OpenVinoEngine import OpenVinoEngine
 from visiongraph.estimator.spatial.face.FaceDetector import FaceDetector
 from visiongraph.model.geometry.BoundingBox2D import BoundingBox2D
 from visiongraph.result.ResultList import ResultList
 from visiongraph.result.spatial.face.FaceDetectionResult import FaceDetectionResult
 
 BOXES_NAME = "boxes"
 
@@ -34,15 +34,15 @@
 class OpenVinoFaceDetector(FaceDetector[FaceDetectionResult]):
     def __init__(self, model: Asset, weights: Asset, min_score: float = 0.5, device: str = "AUTO"):
         super().__init__(min_score)
 
         self.width: Optional[int] = None
         self.height: Optional[int] = None
 
-        self.engine = VisionInferenceEngine(model, weights, device=device)
+        self.engine = OpenVinoEngine(model, weights, device=device)
 
     def setup(self):
         self.engine.setup()
         _, _, self.height, self.width = self.engine.first_input_shape
 
     def process(self, data: np.ndarray) -> ResultList[FaceDetectionResult]:
         output = self._get_results(self.engine.process(data))
```

## visiongraph/estimator/translation/DeblurGANv2.py

```diff
@@ -3,26 +3,27 @@
 
 import cv2
 import numpy as np
 
 from visiongraph.data.Asset import Asset
 from visiongraph.data.RepositoryAsset import RepositoryAsset
 from visiongraph.estimator.VisionEstimator import VisionEstimator
+from visiongraph.estimator.openvino.OpenVinoEngine import OpenVinoEngine
 from visiongraph.estimator.openvino.VisionInferenceEngine import VisionInferenceEngine
 from visiongraph.result.ImageResult import ImageResult
 
 
 class DeblurGANv2Config(Enum):
     DeblurGANv2_FP16 = RepositoryAsset.openVino("deblurgan-v2-fp16")
     DeblurGANv2_FP32 = RepositoryAsset.openVino("deblurgan-v2-fp32")
 
 
 class DeblurGANv2(VisionEstimator[ImageResult]):
     def __init__(self, model: Asset, weights: Asset):
-        self.engine = VisionInferenceEngine(model, weights)
+        self.engine = OpenVinoEngine(model, weights)
 
     def setup(self):
         self.engine.setup()
 
     def process(self, data: np.ndarray) -> ImageResult:
         outputs = self.engine.process(data)
         output = outputs[self.engine.output_names[0]]
```

## visiongraph/model/CameraIntrinsics.py

```diff
@@ -1,9 +1,10 @@
 import json
 
+import cv2
 import numpy as np
 
 INTRINSIC_MATRIX_NAME = "intrinsic_matrix"
 DISTORTION_COEFFICIENTS_NAME = "distortion_coefficients"
 
 
 class CameraIntrinsics:
@@ -26,14 +27,23 @@
             data = json.load(file)
 
         intrinsic_mat = np.array(data[INTRINSIC_MATRIX_NAME], dtype=float)
         distortion_coeff = np.array(data[DISTORTION_COEFFICIENTS_NAME], dtype=float)
 
         return CameraIntrinsics(intrinsic_mat, distortion_coeff)
 
+    @staticmethod
+    def load_from_file_storage(path: str):
+        storage = cv2.FileStorage(path, cv2.FILE_STORAGE_READ)
+        intrinsic_mat = storage.getNode('Camera_Matrix').mat()
+        distortion_coeff = storage.getNode('Distortion_Coefficients').mat()
+        storage.release()
+
+        return CameraIntrinsics(intrinsic_mat, distortion_coeff)
+
     @property
     def px(self) -> float:
         return self.intrinsic_matrix[0, 2]
 
     @property
     def py(self) -> float:
         return self.intrinsic_matrix[1, 2]
```

## visiongraph/model/geometry/BoundingBox2D.py

```diff
@@ -24,18 +24,26 @@
         return vector.obj(x=self.x_min + self.width * 0.5, y=self.y_min + self.height * 0.5)
 
     @property
     def top_left(self) -> vector.Vector2D:
         return vector.obj(x=self.x_min, y=self.y_min)
 
     @property
+    def top_right(self) -> vector.Vector2D:
+        return vector.obj(x=self.x_min + self.width, y=self.y_min)
+
+    @property
     def bottom_right(self) -> vector.Vector2D:
         return vector.obj(x=self.x_min + self.width, y=self.y_min + self.height)
 
     @property
+    def bottom_left(self) -> vector.Vector2D:
+        return vector.obj(x=self.x_min, y=self.y_min + self.height)
+
+    @property
     def x_max(self) -> float:
         return self.x_min + self.width
 
     @property
     def y_max(self):
         return self.y_min + self.height
 
@@ -107,9 +115,15 @@
 
         box_a_area = (box_a[2] - box_a[0] + 1) * (box_a[3] - box_a[1] + 1)
         box_b_area = (box_b[2] - box_b[0] + 1) * (box_b[3] - box_b[1] + 1)
 
         iou = inter_area / float(box_a_area + box_b_area - inter_area)
         return iou
 
+    def contains(self, p: vector.Vector2D) -> bool:
+        if self.x_min < p.x < self.x_max:
+            if self.y_min < p.y < self.y_max:
+                return True
+        return False
+
     def __repr__(self):
         return f"BoundingBox2D(x={self.x_min:.4f}, y={self.y_min:.4f}, w={self.width:.4f}, h={self.height:.4f})"
```

## visiongraph/output/fbs/SyphonServer.py

```diff
@@ -1,32 +1,35 @@
+import logging
 from argparse import Namespace, ArgumentParser
 from typing import Optional, Any
 
 import cv2
 import glfw
 
-
-def monkeypatch_ctypes():
-    import os
-    import ctypes.util
-    uname = os.uname()
-    if uname.sysname == "Darwin" and uname.release >= "20.":
-        real_find_library = ctypes.util.find_library
-
-        def find_library(name):
-            if name in {"OpenGL", "GLUT"}:  # add more names here if necessary
-                return f"/System/Library/Frameworks/{name}.framework/{name}"
-            return real_find_library(name)
-
-        ctypes.util.find_library = find_library
-    return
-
-
-# fixes opengl import on MacOS
-monkeypatch_ctypes()
+try:
+    def monkeypatch_ctypes():
+        import os
+        import ctypes.util
+        uname = os.uname()
+        if uname.sysname == "Darwin" and uname.release >= "20.":
+            real_find_library = ctypes.util.find_library
+
+            def find_library(name):
+                if name in {"OpenGL", "GLUT"}:  # add more names here if necessary
+                    return f"/System/Library/Frameworks/{name}.framework/{name}"
+                return real_find_library(name)
+
+            ctypes.util.find_library = find_library
+        return
+
+
+    # fixes opengl import on MacOS
+    monkeypatch_ctypes()
+except Exception as ex:
+    logging.warning(f"Error in Syphon Server monkeypatch: {ex}")
 
 import numpy as np
 import syphonpy
 
 from OpenGL.GL import *
 from OpenGL.GLU import *
 from OpenGL.GLUT import *
```

## visiongraph/util/ResultUtils.py

```diff
@@ -1,25 +1,26 @@
 import copy
-from typing import List, TypeVar, Tuple
+from typing import List, TypeVar, Tuple, Optional
 
 import cv2
 import numpy as np
 
 from visiongraph.model.geometry.Size2D import Size2D
 from visiongraph.model.geometry.BoundingBox2D import BoundingBox2D
 from visiongraph.result.spatial.ObjectDetectionResult import ObjectDetectionResult
 from visiongraph.util import ImageUtils
 
 ODR = TypeVar("ODR", bound=ObjectDetectionResult)
 
 
-def non_maximum_suppression(results: List[ODR], min_score: float, iou_threshold: float) -> List[ODR]:
+def non_maximum_suppression(results: List[ODR], min_score: float, iou_threshold: float,
+                            eta: Optional[float] = None, top_k: Optional[int] = None) -> List[ODR]:
     boxes = [list(result.bounding_box) for result in results]
     confidences = [result.score for result in results]
-    indices = cv2.dnn.NMSBoxes(boxes, confidences, min_score, iou_threshold)
+    indices = cv2.dnn.NMSBoxes(boxes, confidences, min_score, iou_threshold, eta, top_k)
     return [results[int(i)] for i in list(indices)]
 
 
 def extract_object_detection_roi(image: np.ndarray,
                                  detection: ODR) -> Tuple[np.ndarray, ODR]:
     box: BoundingBox2D = detection.bounding_box.scale_with(Size2D.from_image(image))
     roi = ImageUtils.roi(image, box)
```

## Comparing `visiongraph-0.1.43.dist-info/METADATA` & `visiongraph-0.1.44.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visiongraph
-Version: 0.1.43
+Version: 0.1.44
 Summary: Visiongraph is a high level computer vision framework.
 Home-page: https://github.com/cansik/visiongraph
 Author: Florian Bruggisser
 Author-email: github@broox.ch
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -34,18 +34,18 @@
 Provides-Extra: all
 Requires-Dist: openvino (~=2022.3.0) ; extra == 'all'
 Requires-Dist: protobuf (<4,>=3.11) ; extra == 'all'
 Requires-Dist: onnxruntime (~=1.12.0) ; extra == 'all'
 Requires-Dist: moviepy ; extra == 'all'
 Requires-Dist: vidgear[core] ; extra == 'all'
 Requires-Dist: numba ; extra == 'all'
-Requires-Dist: pyrealsense2 (~=2.53.1) ; (platform_system != "Darwin") and extra == 'all'
+Requires-Dist: pyrealsense2 ; (platform_system != "Darwin") and extra == 'all'
 Requires-Dist: onnxruntime-gpu (~=1.12.0) ; (platform_system != "Darwin") and extra == 'all'
 Requires-Dist: mediapipe (~=0.9.1) ; (platform_system != "Darwin" or platform_machine != "arm64") and extra == 'all'
-Requires-Dist: pyrealsense2-macosx (~=2.53.1) ; (platform_system == "Darwin") and extra == 'all'
+Requires-Dist: pyrealsense2-macosx ; (platform_system == "Darwin") and extra == 'all'
 Requires-Dist: onnxruntime (~=1.12.0) ; (platform_system == "Darwin") and extra == 'all'
 Requires-Dist: syphonpy ; (platform_system == "Darwin") and extra == 'all'
 Requires-Dist: glfw ; (platform_system == "Darwin") and extra == 'all'
 Requires-Dist: mediapipe-silicon (~=0.9.1) ; (platform_system == "Darwin" and platform_machine == "arm64") and extra == 'all'
 Requires-Dist: pyopengl ; (platform_system == "Darwin" or platform_system == "Windows") and extra == 'all'
 Requires-Dist: SpoutGL (>=0.0.4) ; (platform_system == "Windows") and extra == 'all'
 Requires-Dist: pyk4a-bundle (~=1.3.0.2) ; (platform_system == "Windows" or platform_system == "Linux") and extra == 'all'
@@ -70,16 +70,16 @@
 Provides-Extra: onnx-gpu
 Requires-Dist: onnxruntime-gpu (~=1.12.0) ; (platform_system != "Darwin") and extra == 'onnx-gpu'
 Requires-Dist: onnxruntime (~=1.12.0) ; (platform_system == "Darwin") and extra == 'onnx-gpu'
 Provides-Extra: opencv-contrib
 Provides-Extra: openvino
 Requires-Dist: openvino (~=2022.3.0) ; extra == 'openvino'
 Provides-Extra: realsense
-Requires-Dist: pyrealsense2 (~=2.53.1) ; (platform_system != "Darwin") and extra == 'realsense'
-Requires-Dist: pyrealsense2-macosx (~=2.53.1) ; (platform_system == "Darwin") and extra == 'realsense'
+Requires-Dist: pyrealsense2 ; (platform_system != "Darwin") and extra == 'realsense'
+Requires-Dist: pyrealsense2-macosx ; (platform_system == "Darwin") and extra == 'realsense'
 
 # ![image](https://user-images.githubusercontent.com/5220162/192808079-2043fb41-8637-4697-8286-985bc5340f37.png) Visiongraph [![PyPI](https://img.shields.io/pypi/v/visiongraph)](https://pypi.org/project/visiongraph/)
 Visiongraph is a high level computer vision framework that includes predefined modules to quickly create and run algorithms on images. It is based on opencv and includes other computer vision frameworks like [Intel openVINO](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html) and [Google MediaPipe](https://google.github.io/mediapipe/).
 
 Here an example on how to start a webcam capture and display the image:
 
 ```python
@@ -204,15 +204,15 @@
 
 ## Roadmap
 Next roadmap points:
 
 - Async input and network model (run when ready)
 
 ## About
-Copyright (c) 2022 Florian Bruggisser
+Copyright (c) 2023 Florian Bruggisser
 
 ### Included Libraries
 
 Parts of these libraries are directly included and adapted to work with visiongraph.
 
 * [motpy](https://github.com/wmuron/motpy) - simple multi object tracking library (MIT License)
 * [motrackers](https://github.com/adipandas/multi-object-tracker) - Multi-object trackers in Python (MIT License)
```

## Comparing `visiongraph-0.1.43.dist-info/RECORD` & `visiongraph-0.1.44.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-tools/CameraCalibratorTool.py,sha256=xRIIlIiM0SpcCS9Z6NLakQQnZPM26PN81HxTHk5rawA,4270
+tools/CameraCalibratorTool.py,sha256=lhnYn-yLYnAH5Jl3l5XpUhAfvCoDl8K5ymPbI5xtieo,4275
 tools/OpenVinoModelRenamer.py,sha256=16t7-MkTm6JnZFVzS-nHfExfGD_6HLD96vHhzd9qDgc,1018
 tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tools/utils.py,sha256=cOX2YMHx5A9aVTeFjXRsyhNbCPavkCCyaw9cMNGvGg0,221
 visiongraph/AsyncGraphNode.py,sha256=sGVtD16mFM0okNXW9wdEHVJ9zzd7tD4gLFIA2lP4Wpo,1758
 visiongraph/BaseGraph.py,sha256=q_UPq53arsmW2wnZMo-jD9bGby2WFNTWwSBMvSLsxfU,2806
 visiongraph/GraphNode.py,sha256=o2uAgN4WknZV1b3gMIKF3TUFRahRRu7AdXiuXMX4hYI,678
 visiongraph/Processable.py,sha256=bhe_zj7nT2xgmD0xYM_BEWMmDlAUtjfsi3jfdLhMb60,276
 visiongraph/VisionGraph.py,sha256=d5EkjL24hmRteBXfSqZD9xfglkM4bDUIZl4GFlhADcQ,2094
 visiongraph/VisionGraphBuilder.py,sha256=i0bn8HLb3yRACeblpk4yFtMJ6hY61R46mFL1Pdkw_Vg,1898
-visiongraph/__init__.py,sha256=TsB_OmVUJly_vwUubGqojtWC1ptyEyQnHCMWd1BJWnE,22210
+visiongraph/__init__.py,sha256=0f47zhxJW66wo7euwlCPrjeKE3CIjWYOVGSGXak7CWs,23501
 visiongraph/cache/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/data/Asset.py,sha256=N43JxIuOjCmW9CropssmFaXvrtIFnQ382YvXT2nfdlM,368
 visiongraph/data/LocalAsset.py,sha256=7AIWlgdwaWHBiC0RbooqpWoRf68nQx3AT0wWdfJ4hk8,376
 visiongraph/data/RepositoryAsset.py,sha256=D9Vmjn4qKjtUdHHryRHVVKaZZg8jWExZX2frDNt2NwE,1099
 visiongraph/data/__init__.py,sha256=-6VQqFg1a72cAwplIbNMVHTDMm7pXqh_-EuWr0gwgrY,324
 visiongraph/data/labels/COCO.py,sha256=4kP0wW4j16KIfdmCPhPNlQAnacZ3Etp2XC8LeECbe5A,2568
 visiongraph/data/labels/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -29,44 +29,48 @@
 visiongraph/estimator/ChainEstimator.py,sha256=MmZkwqBkL1w7t6k60mBn9bKfDx7cP1UGfLicASQfeEw,1100
 visiongraph/estimator/ScoreThresholdEstimator.py,sha256=ZqOctLVH052VwKGRj2EIPY9ngGIi8411LBEDEjJnW_o,403
 visiongraph/estimator/VisionClassifier.py,sha256=rBb-yuVKPIz3YVsvCu2HCAWh76mclIJWLTCjncKkXIA,868
 visiongraph/estimator/VisionEstimator.py,sha256=dPAVLBMGGey_zy9AGCVr0kQYu3QP7KTzScZ-1UEgaPo,410
 visiongraph/estimator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/estimator/calculator/UndistortionCalculator.py,sha256=IV7Vgc7UMUkXsAS7tBYespukRL5f52Q-VxOfh5wNhIc,2448
 visiongraph/estimator/calculator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+visiongraph/estimator/engine/InferenceEngineFactory.py,sha256=uOLuIGb9Ao7Yo2k-rWxqFGz8KSvKF7diY6lNZMtE-FY,1231
+visiongraph/estimator/engine/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/estimator/inpaint/BaseInpainter.py,sha256=D-YtOAvQpMIZx2dMp4sYuX_U4-GAxW8EUnQMUmW_9hg,529
 visiongraph/estimator/inpaint/GMCNNInpainter.py,sha256=vr_9uV8gmYEOWSUYfEW3iQQJVkRpQC5YGyC2QvUDpRs,2161
 visiongraph/estimator/inpaint/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-visiongraph/estimator/onnx/ONNXVisionEngine.py,sha256=e7AHrcBrHN0JIcs_zxOBlS52WRaFeJxnCAI-rnT779A,2108
+visiongraph/estimator/onnx/ONNXVisionEngine.py,sha256=Lo4jwsZ518xvmJdU4I39u66GeRdG5yFZICAClKuN4xk,2077
 visiongraph/estimator/onnx/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/estimator/openvino/OpenVinoEngine.py,sha256=hPjMx_IkTcjN_y5iLZbuuvVJINiTILG8CVwdGZScsrk,2220
 visiongraph/estimator/openvino/OpenVinoObjectDetector.py,sha256=vJryusJDc1YWMZdRdQnc1XLomowE1TcVF4mwODR02tU,2516
 visiongraph/estimator/openvino/OpenVinoPoseEstimator.py,sha256=c3geJ5Qm18uCRTp-_iBj62yfPXV5TP4HJ0aWRx9kZJ4,2967
 visiongraph/estimator/openvino/SyncInferencePipeline.py,sha256=A9Wpw7DkqXb584UhqJPBNLddi44fHMuNjXhI6RtD9ws,726
 visiongraph/estimator/openvino/VisionInferenceEngine.py,sha256=e98vb7jCguQ1L9Rzwm-HVdXYKlR5o_ddAM6OxtAj2XE,1703
 visiongraph/estimator/openvino/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/estimator/spatial/CenterNetDetector.py,sha256=v0RPUeSgWHl8n60xKl0HT13aZ25XEPRYJsLbjbgX2iU,1750
+visiongraph/estimator/spatial/CrowdHumanDetector.py,sha256=FA-rh-0mbcoqSNhs6SUwY9GFhhISclIP1QM2rnhIML4,3270
 visiongraph/estimator/spatial/DETRDetector.py,sha256=WdO5By3b4GO4jBsT4YdYjztAC6sEP-ntdeh55FeQLZc,1781
 visiongraph/estimator/spatial/InstanceSegmentationEstimator.py,sha256=FLwQBX8ZcB5-brYe-ye7XHIWmUaPaX0UOa1eCNikOD0,544
 visiongraph/estimator/spatial/LandmarkEstimator.py,sha256=H8bvBn3QWTsT3cqvCmyBFazT-yXhUaUTKPMUjbWGAns,523
 visiongraph/estimator/spatial/ObjectDetector.py,sha256=U5rEA-bGvLaHsV3zhMhAJumnPPiaTGUu0p6Rlk1nhcg,524
 visiongraph/estimator/spatial/RoiEstimator.py,sha256=cfZUne-PGV1PuFk7Hwy6Vqijvrlzqcpl9IryBfx0VaA,1279
 visiongraph/estimator/spatial/SSDDetector.py,sha256=NJHlb-3KMLaCS8l4TsfH4xk0gTjY5BnnEic8Mu0310s,3147
 visiongraph/estimator/spatial/SlidingWindowEstimator.py,sha256=x2KMrhsQesB8KVhDnx28399IgevXYQ_pGntREncmwJ4,2082
 visiongraph/estimator/spatial/SpatialCascadeEstimator.py,sha256=thm2fFIJ-SJZrDatQcgiT5DK35MNwA_7O0N1lWEO5jk,1436
 visiongraph/estimator/spatial/YOLODetector.py,sha256=g0XvES7Ol8SVHCerrKB64Hp3p_ldN0uVwzsrlafdJJw,3173
+visiongraph/estimator/spatial/YOLOv5Detector.py,sha256=CDGhz50x23KGjbHTB29to0Wjoaj0E_3BmNNY01W2mC0,3594
 visiongraph/estimator/spatial/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/estimator/spatial/camera/ArUcoCameraPoseEstimator.py,sha256=GrahyzDfdN0gDaGlAIjmZ27ZF2G3_-TZZMWM_Xqt2YU,3441
 visiongraph/estimator/spatial/camera/BoardCameraCalibrator.py,sha256=qlLwrjPfPa2kB-y_0NMYEqpqCaCU4K3EUaNY1F6sK8E,850
 visiongraph/estimator/spatial/camera/ChArUcoCalibrator.py,sha256=f0aX1ONvblYcItbf-R8e_qQOyixvhgDB_DKBRIrZcXU,4276
 visiongraph/estimator/spatial/camera/ChessboardCalibrator.py,sha256=8WN2RC93HRtlTz5bY0iNItGpOSBUGX58SAU7O-9T5JU,3145
 visiongraph/estimator/spatial/camera/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/estimator/spatial/face/AdasFaceDetector.py,sha256=I1vXSt9QviYl12jLdy6pUjjRGgFVLAh2v9MTPF7BBQo,1127
 visiongraph/estimator/spatial/face/FaceDetector.py,sha256=L_W5LFzrD1fqK7jbZSRlaphA3Yma0Q-sw2nctk72aYE,512
-visiongraph/estimator/spatial/face/OpenVinoFaceDetector.py,sha256=lxEmQCwxk2jBRcskOo4nL_m4CoZ4F6w7oUS-xN4QD7I,3826
+visiongraph/estimator/spatial/face/OpenVinoFaceDetector.py,sha256=ZXw_wGa6VJ3HYMn9uE1ukYFrCwCq9Ijggmmu6LAAkSA,3805
 visiongraph/estimator/spatial/face/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/estimator/spatial/face/emotion/AffectNetEmotionClassifier.py,sha256=gOrT83tV8E4x-0uYDIj7xHmLRb-LsGyfwatiN1KXvwU,1781
 visiongraph/estimator/spatial/face/emotion/FaceEmotionEstimator.py,sha256=8H_t4Eej-bxtNYsz8IserQxSaIdHCZSRy0Pyn8i4GoY,450
 visiongraph/estimator/spatial/face/emotion/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/estimator/spatial/face/landmark/FaceLandmarkEstimator.py,sha256=wheWNMlElKmtax-1brYwWVWIGdDb_Br7ogbM2uFX6U8,609
 visiongraph/estimator/spatial/face/landmark/IrisDistanceCalculator.py,sha256=EL0xwtMVDWQD79_vZsdWof9LPixxwC7_pDO0MMD_oHc,2646
 visiongraph/estimator/spatial/face/landmark/MediaPipeFaceDetector.py,sha256=__v18t7-RVut5NXOu7ypsZ2YpIrIdodprbIzJfJk8Lg,2204
@@ -97,15 +101,15 @@
 visiongraph/estimator/spatial/pose/PoseEstimator.py,sha256=X1JvTnef7g9frs89SwjCE8PiJtFS6qXWUZda66zKcKc,518
 visiongraph/estimator/spatial/pose/TopDownPoseEstimator.py,sha256=8OcnaFirohSyCyYchoUNwVoPWCh-qjU5F-bp6SkvdIM,2347
 visiongraph/estimator/spatial/pose/__init__.py,sha256=AAFuqiTFgX5hw7oi9zeoFLReijnxOWSKyWWDw-izGH0,4815
 visiongraph/estimator/spatial/segmentation/MaskRCNNEstimator.py,sha256=QUnUP9IIEbnantEcQPuGvQjle8NhSeTbXv5Ns-y3pOE,7516
 visiongraph/estimator/spatial/segmentation/MediaPipeSelfieSegmentation.py,sha256=y7oi5fZiEHRlbKFstap3ai5I0AYyXJrKMsSmWESMtRU,1989
 visiongraph/estimator/spatial/segmentation/YolactEstimator.py,sha256=tO6z6y-PvDW-8bJvmJdIyiQsHZbQhA0WDB50uXWVLRs,3287
 visiongraph/estimator/spatial/segmentation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-visiongraph/estimator/translation/DeblurGANv2.py,sha256=xsR4DqfGTTDzKY4ZkhQHbTTPf4K5qFZiubtvSU09uMU,1648
+visiongraph/estimator/translation/DeblurGANv2.py,sha256=E1cooQe8gIvtLWdwyd492bNfnbp_naic4pC4JmyABvg,1714
 visiongraph/estimator/translation/DepthEstimator.py,sha256=7-3ajpANUrYmkWHxTE6VDphAfmtp12ty-UXxcoddXzI,314
 visiongraph/estimator/translation/MidasDepthEstimator.py,sha256=-OxQaZrS7qc9-2DQwna2LfRlkCHY5NYREDDBRGb8oBc,2898
 visiongraph/estimator/translation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/external/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/external/intel/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/external/intel/performance_metrics.py,sha256=WWU9IXR7COl790yl3qhUU0fLLPBov8mkFsVplVkxuhs,4337
 visiongraph/external/intel/adapters/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -148,21 +152,21 @@
 visiongraph/input/BaseDepthInput.py,sha256=3nYxcLLLlPkT4oPewVQJMcLf8u3J5AABEW84qICY0mA,1309
 visiongraph/input/BaseInput.py,sha256=Uji-uvrAnHHXsTIBmT5wKDQGj9uO1NUlFLJHMvoAw0E,3760
 visiongraph/input/CamGearInput.py,sha256=FVQROPlYVpVrk2CqVeg_bT83Z0UkN9GsCLj0lUg2SZs,1721
 visiongraph/input/ImageInput.py,sha256=fX0sJcNcnd3vnu_2_23kpFPNr7goJNy7OIeERznTEjI,1493
 visiongraph/input/RealSenseInput.py,sha256=77yXdcoNbdI3k4GshC59SUz2U7zctbxyXc4aHe45JQU,18995
 visiongraph/input/VideoCaptureInput.py,sha256=hupeQtiYPJyc610Hjpp8PleWQ1_Guvx0Xkvw0bOgmmE,5032
 visiongraph/input/__init__.py,sha256=Vli1TwT7ro_EVAoNBgUVoPIXYJY8Yni-RbHSe8FR54Y,1305
-visiongraph/model/CameraIntrinsics.py,sha256=k50RjHIsTbPj1zjBNFsJwGgZ55mpKZueAIgOlGBoTKc,1520
+visiongraph/model/CameraIntrinsics.py,sha256=8VwgAVjwMocZqoRsbpd2beYetI3_v1WpcM9jppirUJw,1887
 visiongraph/model/CameraStreamType.py,sha256=lYCzWM6blHEi_cwKo2U-xx8LqOIfbjvUJyAppRRTXMg,101
 visiongraph/model/DepthBuffer.py,sha256=YjvpgAIcdoXVB2QdVzZxplDlkW0lX1mxdgAPukc9E2Y,549
 visiongraph/model/VisionEngineOutput.py,sha256=LdlYxbv8Rn5fnAnb7r8mDukBo2GWgYr3265lxOH-1A0,753
 visiongraph/model/_ImportStub.py,sha256=5kk04z_ji1TFi6IK0KlKditRTRvlIL7HCCF9Ztwplyw,135
 visiongraph/model/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-visiongraph/model/geometry/BoundingBox2D.py,sha256=jKKdHyAwxhttNkxdZgYH6UN_tzc9yrwiRqXT1kHwp4I,3784
+visiongraph/model/geometry/BoundingBox2D.py,sha256=ziKxXgBBihlZJlragX_3Mdpmw8KyQsZfbc1SgCIMZ3Q,4229
 visiongraph/model/geometry/Size2D.py,sha256=-t2jPBKm1vkEdRz7KKE16pTwqg6JUSZrDJGIoB48X_4,815
 visiongraph/model/geometry/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/model/parameter/ArgumentConfigurable.py,sha256=UOmxjHVaCl7In0KWPFah1hT6FLtyKg4rK13D35hxjKI,585
 visiongraph/model/parameter/NamedParameter.py,sha256=gtqJvJFVQDtjSYJ4mcYvLifcm8i_x4U15KE-hVs8iNk,186
 visiongraph/model/parameter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/model/tracker/Trackable.py,sha256=ZU-UBUdmace5tw4fUQNHxp0mOmvwTOtlhdIPlvP_mW0,399
 visiongraph/model/tracker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -178,15 +182,15 @@
 visiongraph/node/PassThroughNode.py,sha256=F6N_V1LgG-tRTA8ei2jW8SKmaf7TkXoVGlvmdPWfHts,525
 visiongraph/node/SequenceNode.py,sha256=sE7vJn5miS9J84JhujG9T6n-rQY5zO4ddI0gEbIcYzU,825
 visiongraph/node/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/output/ImagePreview.py,sha256=TVxwnGVYMNWGQelahPdLlmQPllv9051QxYIb5RE5__o,1471
 visiongraph/output/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/output/fbs/FrameBufferSharingServer.py,sha256=CHICjVwbvoUJODC5uKEwrHBMp7taBt8WrQ9AewxHRk0,935
 visiongraph/output/fbs/SpoutServer.py,sha256=m0WJjaDLKSgrpuQ1CRYCbylVc9gQF1ilzorYrqS8joU,1390
-visiongraph/output/fbs/SyphonServer.py,sha256=Nsg56nLe2ElA5QdobdjlExB9CYTi346nBkWb0YlIJBU,3123
+visiongraph/output/fbs/SyphonServer.py,sha256=UGoNlMF5Nf4kvaPR8ZXRThWQsrj2A1sjDo2dUf9Y4e8,3287
 visiongraph/output/fbs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/recorder/AsyncFrameSetRecorder.py,sha256=eE1WCZcoBiWdlOFuAx0x-x0O-pMRx-2o74ykIfw0-LU,980
 visiongraph/recorder/BaseFrameRecorder.py,sha256=XmZjy2rVupOYWB0of722ilvlUgxe_TI5gFYq14nntG0,1108
 visiongraph/recorder/CV2VideoRecorder.py,sha256=VjGmcfdqM--jAeFDR6BqBXVk5mu7wbPnDCR3tRKO4Fg,1143
 visiongraph/recorder/FrameSetRecorder.py,sha256=Oz3HeHT_-Zq-wEgFd8rfpF61Vicvr8wIbjSizXFDAXM,1016
 visiongraph/recorder/MoviePyVideoRecorder.py,sha256=4hWv0AKdLiDuDCuBkG-2Qo4BsoV4iFtaAP_lnOwnVeg,905
 visiongraph/recorder/VidGearVideoRecorder.py,sha256=8e2ILk_or6TUL80Ki44wWihvLZcxiV63TNgozFwEOUY,1377
@@ -200,14 +204,15 @@
 visiongraph/result/EmbeddingResult.py,sha256=oiEkwW0fhlN6J5Z1z-uQsqvMCH_fqUifzQePyp_WHoA,487
 visiongraph/result/HeadPoseResult.py,sha256=AiEfV736lqcq0VP2LKtlwYhpRTkN80lj5d9oQ-ZOa1A,474
 visiongraph/result/ImageResult.py,sha256=SZI45nXnRDKpVy_JdrVNE4HIiPcBfPS1kg40QnQWPKQ,333
 visiongraph/result/ResultAnnotator.py,sha256=sSvYcJPnwWcVmKDemnJF-QFZKHeNrN17e1ZfOYwECyg,1165
 visiongraph/result/ResultDict.py,sha256=MMY7vQeY0mUsucx3yItiDejz_7N-H9GF2RMDwMFKnbs,483
 visiongraph/result/ResultList.py,sha256=scFITiK6_ryqAWdESJFl_XG1HFXibToni4PIAlXk1yk,466
 visiongraph/result/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+visiongraph/result/spatial/CrowdHumanResult.py,sha256=vmBXlNYHvBmdMvOo1qgbXabvy6OEuom_YGsLceoUmV0,779
 visiongraph/result/spatial/InstanceSegmentationResult.py,sha256=usIcyhwF8rKxUhLKurqByZyvI1V32iW_it5si-6G9dA,1354
 visiongraph/result/spatial/LandmarkDetectionResult.py,sha256=uoZf4AuD7No14GSW7TyaVJEaoQOeLnvB8VdEBcWk8oo,4199
 visiongraph/result/spatial/ObjectDetectionResult.py,sha256=xzXC41Al0T6hIssivEKLj-6HclW41u4PI9tJX2w2kJA,3475
 visiongraph/result/spatial/SpatialCascadeResult.py,sha256=HoA3p-Yj0g7JirvEEEdLOpFohvSx57LimsNDJ-gcBUw,878
 visiongraph/result/spatial/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/result/spatial/face/BlazeFace.py,sha256=RCVta6C5WxeUIwqv_2k04GN6v3JddvE5uDJ2l5_uGUQ,924
 visiongraph/result/spatial/face/BlazeFaceMesh.py,sha256=WZRa8JaqanjkqxnMz2L6ZXJRHmjP1BnnvCPkb1Z6LLI,2064
@@ -231,28 +236,30 @@
 visiongraph/result/spatial/pose/MobileHumanPose.py,sha256=GpOtG1VGrJxMKVzIUvp49p9MrhuyDhLjqvijDoD9ylk,2738
 visiongraph/result/spatial/pose/PoseLandmarkResult.py,sha256=OSsw0WYQlbQ9MxxKuOZdIsjBAzI9CfT9H0bDkqWwWn4,2823
 visiongraph/result/spatial/pose/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/tracker/BaseObjectDetectionTracker.py,sha256=4e_1Cla7hT3BFRDSUmTgS3KfphYs0YcU2-9HIbYolNQ,492
 visiongraph/tracker/CentroidTracker.py,sha256=JVxG5CAu0rjgntMl2c4XGUj3hMybxcnKIvcJmH1QsxM,1908
 visiongraph/tracker/FlateTracker.py,sha256=9T8qmL0Z4WYuw3m4tx4MDE1Owg8ui46TUvcQfjdR7L8,4906
 visiongraph/tracker/MotpyTracker.py,sha256=NJ4wUYRsJy4Ns5aKlze4_JdEwjWByXoW3lgUs1hamgM,2705
+visiongraph/tracker/ObjectAssignmentSolver.py,sha256=UnatM7p0547-hrvLtcplD5PsZabpxZWoKa_wqnEVK-I,3299
 visiongraph/tracker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visiongraph/util/ArgUtils.py,sha256=ScmV828V-II5p0Wtpux1pDYDPENfka9cdzp8kLqSazI,3105
 visiongraph/util/CodeUtils.py,sha256=6xx82UlfereWKI7yczCApgTgOquvDXLONnfysSVYoiQ,1009
 visiongraph/util/CollectionUtils.py,sha256=IR178KrIULFRiSZzSMQkH78AaTvjhpaGFjJ57jZu0vw,222
 visiongraph/util/CommonArgs.py,sha256=sLhJv-vgMkaSCwbrfpDsZy8cAK7-kTAa5pnw_X_gqgU,314
 visiongraph/util/DrawingUtils.py,sha256=7_vksJauc7scpmFKHs8_S5xviGQoOd4n_p7sfix5G2U,3653
 visiongraph/util/ImageUtils.py,sha256=_eP8x8IrRiQv7IIOPsrBXFycGa8IgOPfKk_xsF9syi8,3588
 visiongraph/util/LinalgUtils.py,sha256=CXKcuq8WkLiARi9HU7gdfS9CdlWW7rlBKvnMl9gkFuc,2608
 visiongraph/util/LoggingUtils.py,sha256=kT0Z5N3PVpaD0kZmIUT3LIYGRz7xXfawXrwEjwITz2s,539
 visiongraph/util/MathUtils.py,sha256=K0O_ZLD1SJ9mq5q6cdtOxNXDrtjZ0MMnSZpqfB2wNxU,1752
 visiongraph/util/NetworkUtils.py,sha256=JIYgwgTfbPfHmMtLGEZmouWUgRDkafmLJ78NlMb8eIQ,2084
+visiongraph/util/OSUtils.py,sha256=B1wbK-iZMKCfVJf1j_0GGAror2VEDto1aikTBnhcEqw,195
 visiongraph/util/OpenVinoUtils.py,sha256=aQNS4nHxi16TZArVqQLZNZMEwOuJR-lUEGBwT8zr6Es,704
-visiongraph/util/ResultUtils.py,sha256=eAqoIzKOAFaAA-AlzvTEVI8wf9Vg-vyKzLXaXj6m_7M,1132
+visiongraph/util/ResultUtils.py,sha256=ow5p1FtfIIuXo7VJMBQz0cuaG0nfZr0NO9LnTJrWgH8,1240
 visiongraph/util/TimeUtils.py,sha256=IVCLc5PtSYhmGB8hp6-oZMceva8Y6uU0K_1BDTZXGmE,2102
 visiongraph/util/VectorUtils.py,sha256=OSjJ1LGBQiEJp-wEocJvLXM1CyS09LesNA-H86Irnjw,3225
 visiongraph/util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-visiongraph-0.1.43.dist-info/METADATA,sha256=AthZZiR06JxK0sKUxAf_ZbzxXKV8n3ylLbSBwDCWPYU,11889
-visiongraph-0.1.43.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-visiongraph-0.1.43.dist-info/entry_points.txt,sha256=Oe-0WHEIftikIMS0mh3HdskyVa241gZLS1N7LHhb60A,66
-visiongraph-0.1.43.dist-info/top_level.txt,sha256=bRATNp8TOnl0xo3F0GYIhPVJh_W1FzO_tQyT-apCFgY,18
-visiongraph-0.1.43.dist-info/RECORD,,
+visiongraph-0.1.44.dist-info/METADATA,sha256=2MxSmg0jtddykiMTb9O5Mk9tc3TD5dMWsHoD4ozqSFs,11845
+visiongraph-0.1.44.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+visiongraph-0.1.44.dist-info/entry_points.txt,sha256=Oe-0WHEIftikIMS0mh3HdskyVa241gZLS1N7LHhb60A,66
+visiongraph-0.1.44.dist-info/top_level.txt,sha256=bRATNp8TOnl0xo3F0GYIhPVJh_W1FzO_tQyT-apCFgY,18
+visiongraph-0.1.44.dist-info/RECORD,,
```

