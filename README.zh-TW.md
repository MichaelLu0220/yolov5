<div align="center">

[English](README.md) | [繁體中文](README.zh-TW.md)
<br>


YOLOv5 🚀 is the world's most loved vision AI, representing <a href="https://ultralytics.com">Ultralytics</a> open-source research into future vision AI methods, incorporating lessons learned and best practices evolved over thousands of hours of research and development.

We hope that the resources here will help you get the most out of YOLOv5. Please browse the YOLOv5 <a href="https://docs.ultralytics.com/yolov5">Docs</a> for details, raise an issue on <a href="https://github.com/ultralytics/yolov5/issues/new/choose">GitHub</a> for support, and join our <a href="https://ultralytics.com/discord">Discord</a> community for questions and discussions!

To request an Enterprise License please complete the form at [Ultralytics Licensing](https://ultralytics.com/license).

<div align="center">
  <a href="https://github.com/MichaelLu0220" style="text-decoration:none;">
    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="4%" alt="" /></a>
  
  <a href="https://www.linkedin.com/company/ultralytics/" style="text-decoration:none;">
    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="4%" alt="" /></a>
  
</div>

</div>
<br>

## <div align="center">參考並修改自 **[[這個GITHUB](https://github.com/ultralytics/yolov5)]**</div>

借鑑YOLOV5模型訓練辨識息肉之MODEL

請參閱 [YOLOv8 Docs](https://docs.ultralytics.com) 以了解詳細資訊並開始使用:

開始前，下載相關套件
```bash
!pip install ultralytics
```

<div align="center">
  <a href="https://ultralytics.com/yolov8" target="_blank">
  <img width="100%" src="https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/yolo-comparison-plots.png"></a>
</div>

## <div align="center">開始文件</div>

從這 [YOLOv5 Docs](https://docs.ultralytics.com/yolov5) 裡有關培訓、測試和部署的完整文檔。請參閱下面的快速入門示例。
本文將由Google Colab為示範:

<details open>
<summary>下載</summary>

```bash
!git clone https://github.com/MichaelLu0220/polyp_yolov5
%cd polyp_yolov5
```

</details>
<details open>
<summary>訓練參數</summary>

```bash
!python detect.py --weights final.pt --img 256 --conf 0.5 --source /content/polyp_yolov5/images
```

</details>
<details open>
<summary>結果顯示</summary>

```bash
import glob
from IPython.display import Image, display

for imageName in glob.glob('/content/polyp_yolov5/runs/detect/exp/*.png'): #assuming JPG
    display(Image(filename=imageName))
    print("\n")
```

</details>
