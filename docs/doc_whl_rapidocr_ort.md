## rapidocr-onnxruntime Package
<p>
    <a href=""><img src="https://img.shields.io/badge/Python-3.6+-aff.svg"></a>
    <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
</p>

### 1. Install package by pypi.
```bash
$ pip install rapidocr-onnxruntime
```

### 2. Use.
```python
import cv2
from rapidocr_onnxruntime import RapidOCR

text_sys = RapidOCR()

img = cv2.imread('test_images/ch_en_num.jpg')

result = text_sys(img)
print(result)

# result: [[dt_boxes], txt, score]
# 示例：[[左上, 右上, 右下, 左下], '小明', '0.99']
```