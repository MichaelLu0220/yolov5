<div align="center">

[English](README.md) | [繁體中文](README.zh-TW.md)
<br>

Please browse the YOLOv5 <a href="https://docs.ultralytics.com/yolov5">Docs</a> for details, raise an issue on <a href="https://github.com/ultralytics/yolov5/issues/new/choose">GitHub</a> for support!

<div align="center">
  <a href="https://github.com/MichaelLu0220" style="text-decoration:none;">
    <img src="https://i.imgur.com/7FLt7C8.png" width="3%" alt="" /></a>
  
  <a href="https://www.linkedin.com/in/michaellu-03868b318/" style="text-decoration:none;">
    <img src="https://i.imgur.com/qAFPI7r.png" width="3%" alt="" /></a>
  
</div>

</div>
<br>

## <div align="center">Referenced and modified from this **[[GITHUB](https://github.com/ultralytics/yolov5)]**</div>

Learn from the YOLOV5 model to train and identify polyps MODEL

See the [YOLOv8 Docs](https://docs.ultralytics.com) to learn more and get started

Directly refer to the provided [Colab](https://colab.research.google.com/drive/1b9Iem2EoKzS9pJABb_CSdJuhV0Q7ob4M?usp=sharing) for operation

Or before you start, download the relevant packages
```bash
!pip install ultralytics
```


## <div align="center">Install</div>

Get complete documentation on training, testing and deployment here [YOLOv5 Docs](https://docs.ultralytics.com/yolov5). See the quickstart example below.
This article will be demonstrated by Google Colab:

<details open>
<summary>Install</summary>

```bash
!git clone https://github.com/MichaelLu0220/yolov5
%cd polyp_yolov5
```

</details>
<details open>
<summary>Inference</summary>

```bash
!python detect.py --weights final.pt --img 256 --conf 0.5 --source /content/polyp_yolov5/images
```

</details>
<details open>
<summary>Result</summary>

```bash
import glob
from IPython.display import Image, display

for imageName in glob.glob('/content/polyp_yolov5/runs/detect/exp/*.png'): #assuming JPG
    display(Image(filename=imageName))
    print("\n")
```

</details>
