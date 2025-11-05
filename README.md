# 🧠 YOLOv11 모델 비교 및 다운로드

아래 표는 YOLOv11의 다양한 모델 버전별 성능 및 사양을 비교한 것입니다.  
파란 글씨 모델명을 클릭하면 각 모델의 가중치(`.pt` 파일)를 다운로드할 수 있습니다.

---

## 📊 YOLOv11 모델 성능 비교

| Model | size (pixels) | mAP<sup>val</sup> 50–95 | Speed (CPU ONNX, ms) | Speed (T4 TensorRT10, ms) | Params (M) | FLOPs (B) |
|:------|:--------------:|:-----------------------:|:---------------------:|:---------------------------:|:-----------:|:----------:|
| [YOLO11n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolo11n.pt) | 640 | 39.5 | 56.1 ± 0.8 | 1.5 ± 0.0 | 2.6 | 6.5 |
| [YOLO11s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolo11s.pt) | 640 | 47.0 | 90.0 ± 1.2 | 2.5 ± 0.0 | 9.4 | 21.5 |
| [YOLO11m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolo11m.pt) | 640 | 51.5 | 183.2 ± 2.0 | 4.7 ± 0.1 | 20.1 | 68.0 |
| [YOLO11l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolo11l.pt) | 640 | 53.4 | 238.6 ± 1.4 | 6.2 ± 0.1 | 25.3 | 86.9 |
| [YOLO11x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolo11x.pt) | 640 | 54.7 | 462.8 ± 6.7 | 11.3 ± 0.2 | 56.9 | 194.9 |

---

### 📥 사용 방법

모델을 다운로드하려면 위의 표에서 원하는 버전을 클릭하세요.  
예를 들어, YOLOv11n을 다운로드하려면 다음 명령어를 사용할 수 있습니다:

```bash
# YOLOv11n 다운로드
wget https://github.com/ultralytics/assets/releases/download/v0.0.0/yolo11n.pt

# 또는 Python 명령어로 사용
yolo predict model=yolo11n.pt source=images/
