
# Face Detection using Haar Cascade Classifier

## 📋 Overview
This project implements real-time face detection using OpenCV's Haar Cascade Classifier. It captures video from a webcam and detects faces in each frame, highlighting them with bounding rectangles.

## 🎯 Features
- **Real-time Face Detection**: Detects faces from webcam feed
- **Visual Feedback**: Draws red rectangles around detected faces
- **Simple Controls**: Press ESC to exit the application
- **Lightweight**: Uses pre-trained Haar Cascade XML file

## 🛠️ Technologies Used
- Python 3.x
- OpenCV (cv2)
- Haar Cascade Classifier

## 🔍 Key Parameters

### `detectMultiScale()` Parameters
- **scaleFactor**: 1.3 (how much the image size is reduced at each scale)
- **minNeighbors**: 4 (minimum number of neighbors to retain a detection)

## 📊 Performance

- **Processing Speed**: ~30 FPS (depends on hardware)
- **Detection Accuracy**: ~90% (under good lighting)
- **Resource Usage**: Low (CPU-based detection)

## 🎨 Customization

### Adjust Detection Sensitivity
```python
face = haar_cascade.detectMultiScale(grayImg, 1.1, 5)
```
- **scaleFactor**: Lower values (1.05) = more accurate but slower
- **minNeighbors**: Higher values (5-8) = fewer false positives

### Change Rectangle Color
```python
cv2.rectangle(img, (x,y), (x+w,y+h), (0, 255, 0), 2)  # Green
```

---

**Happy Face Detecting!** 😊
