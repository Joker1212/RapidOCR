## rapidocr-openvino Package
<p>
    <a href=""><img src="https://img.shields.io/badge/Python-3.6+-aff.svg"></a>
    <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
</p>

### 1. Install package by pypi.
```shell
$ pip install rapidocr-openvino
```


### 2. Use.
```python
import cv2
from rapidocr_openvino import RapidOCR

text_sys = RapidOCR('config.yaml')

img = cv2.imread('test_images/ch_en_num.jpg')

result = text_sys(img)
print(result)

# result: [[dt_boxes], txt, score]
# 示例：[[左上, 右上, 右下, 左下], '小明', '0.99']
```