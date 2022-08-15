# YOLOAir:  新的Air, Air, Air

YOLOAir算法库 是一个基于 PyTorch 的一系列 YOLO 检测算法组合工具箱。用来**组合不同模块构建不同网络**。  

<div align='center'>
    <img src='docs/image/logo1.png' width='500px'>
</div>

内置YOLOv5、YOLOv7、YOLOX、YOLOR、Transformer、Scaled_YOLOv4、YOLOv3、YOLOv4、YOLO-Facev2、TPH-YOLOv5、YOLOv5-Lite、PP-YOLO、PicoDet等算法模型(更新中)...

**模块组件化**：帮助用户自定义快速组合Backbone、Neck、Head，使得网络模型多样化，助力科研改进检测算法、模型改进，网络排列组合🏆。构建强大的网络模型。

**统一模型代码框架、统一应用方式、统一调参、、统一部署、易于模块组合、构建更强大的网络模型**。  

```

██╗   ██╗ ██████╗ ██╗      ██████╗      █████╗     ██╗    ██████╗ 
╚██╗ ██╔╝██╔═══██╗██║     ██╔═══██╗    ██╔══██╗    ██║    ██╔══██╗
 ╚████╔╝ ██║   ██║██║     ██║   ██║    ███████║    ██║    ██████╔╝
  ╚██╔╝  ██║   ██║██║     ██║   ██║    ██╔══██║    ██║    ██╔══██╗
   ██║   ╚██████╔╝███████╗╚██████╔╝    ██║  ██║    ██║    ██║  ██║
   ╚═╝    ╚═════╝ ╚══════╝ ╚═════╝     ╚═╝  ╚═╝    ╚═╝    ╚═╝  ╚═╝
```


基于 YOLOv5 代码框架，并同步适配 **稳定的YOLOv5_v6.1更新**, 同步v6.1部署生态。使用这个项目之前, 您可以先了解YOLOv5库。  

简体中文 | [English]()

[特性🚀](#Mainfeatures) • [使用🍉](#Usage) • [文档📒](https://github.com/iscyy/yoloair) • [报告问题🌟](https://github.com/iscyy/yoloair/issues/new)

![](https://img.shields.io/badge/News-2022-red)  ![](https://img.shields.io/badge/Update-YOLOAir-orange) ![](https://visitor-badge.glitch.me/badge?page_id=iscyy.yoloair)  

#### 支持
![](https://img.shields.io/badge/Support-YOLOv5-red) ![](https://img.shields.io/badge/Support-YOLOv7-brightgreen) ![](https://img.shields.io/badge/Support-YOLOX-yellow) ![](https://img.shields.io/badge/Support-YOLOv4-green) ![](https://img.shields.io/badge/Support-Scaled_YOLOv4-ff96b4)
![](https://img.shields.io/badge/Support-YOLOv3-yellowgreen) ![](https://img.shields.io/badge/Support-YOLOR-lightgrey) ![](https://img.shields.io/badge/Support-Transformer-9cf) ![](https://img.shields.io/badge/Support-Attention-green)

项目地址: https://github.com/iscyy/yoloair

### 主要特性🚀

🚀支持更多的YOLO系列算法模型(持续更新...)

YOLOAir 算法库汇总了多种主流YOLO系列检测模型，一套代码集成多种模型:
<div><span style="color: #ff0000">-</span><span style="color: #ff0300"> </span><span style="color: #ff0500">内</span><span style="color: #ff0800">置</span><span style="color: #ff0b00">集</span><span style="color: #ff0d00">成</span><span style="color: #ff1000"> </span><span style="color: #ff1300">Y</span><span style="color: #ff1500">O</span><span style="color: #ff1800">L</span><span style="color: #ff1a00">O</span><span style="color: #ff1d00">v</span><span style="color: #ff2000">5</span><span style="color: #ff2200"> </span><span style="color: #ff2500">模</span><span style="color: #ff2800">型</span><span style="color: #ff2a00">网</span><span style="color: #ff2d00">络</span><span style="color: #ff3000">结</span><span style="color: #ff3200">构</span></div><div><span style="color: #ff3500">-</span><span style="color: #ff3800"> </span><span style="color: #ff3a00">内</span><span style="color: #ff3d00">置</span><span style="color: #ff4000">集</span><span style="color: #ff4200">成</span><span style="color: #ff4500"> </span><span style="color: #ff4700">Y</span><span style="color: #ff4a00">O</span><span style="color: #ff4d00">L</span><span style="color: #ff4f00">O</span><span style="color: #ff5200">R</span><span style="color: #ff5500"> </span><span style="color: #ff5700">模</span><span style="color: #ff5a00">型</span><span style="color: #ff5d00">网</span><span style="color: #ff5f00">络</span><span style="color: #ff6200">结</span><span style="color: #ff6500">构</span></div><div><span style="color: #ff6700">-</span><span style="color: #ff6a00"> </span><span style="color: #ff6c00">内</span><span style="color: #ff6f00">置</span><span style="color: #ff7200">集</span><span style="color: #ff7400">成</span><span style="color: #ff7700"> </span><span style="color: #ff7a00">Y</span><span style="color: #ff7c00">O</span><span style="color: #ff7f00">L</span><span style="color: #ff8200">O</span><span style="color: #ff8400">X</span><span style="color: #ff8700"> </span><span style="color: #ff8900">模</span><span style="color: #ff8c00">型</span><span style="color: #ff8f00">网</span><span style="color: #ff9100">络</span><span style="color: #ff9400">结</span><span style="color: #ff9700">构</span></div><div><span style="color: #ff9900">-</span><span style="color: #ff9c00"> </span><span style="color: #ff9e00">内</span><span style="color: #ffa100">置</span><span style="color: #ffa400">集</span><span style="color: #ffa600">成</span><span style="color: #ffa900"> </span><span style="color: #ffab00">Y</span><span style="color: #ffae00">O</span><span style="color: #ffb100">L</span><span style="color: #ffb300">O</span><span style="color: #ffb600">v</span><span style="color: #ffb800">7</span><span style="color: #ffbb00"> </span><span style="color: #ffbe00">模</span><span style="color: #ffc000">型</span><span style="color: #ffc300">网</span><span style="color: #ffc600">络</span><span style="color: #ffc800">结</span><span style="color: #ffcb00">构</span></div><div><span style="color: #ffcd00">-</span><span style="color: #ffd000"> </span><span style="color: #ffd300">内</span><span style="color: #ffd500">置</span><span style="color: #ffd800">集</span><span style="color: #ffda00">成</span><span style="color: #ffdd00"> </span><span style="color: #ffe000">S</span><span style="color: #ffe200">c</span><span style="color: #ffe500">a</span><span style="color: #ffe700">l</span><span style="color: #ffea00">e</span><span style="color: #ffed00">d</span><span style="color: #ffef00">_</span><span style="color: #fff200">Y</span><span style="color: #fff500">O</span><span style="color: #fff700">L</span><span style="color: #fffa00">O</span><span style="color: #fffc00">v</span><span style="color: #ffff00">4</span><span style="color: #faff00"> </span><span style="color: #f4ff00">模</span><span style="color: #efff00">型</span><span style="color: #eaff00">网</span><span style="color: #e4ff00">络</span><span style="color: #dfff00">结</span><span style="color: #daff00">构</span></div><div><span style="color: #d5ff00">-</span><span style="color: #cfff00"> </span><span style="color: #caff00">内</span><span style="color: #c5ff00">置</span><span style="color: #bfff00">集</span><span style="color: #baff00">成</span><span style="color: #b5ff00"> </span><span style="color: #afff00">Y</span><span style="color: #aaff00">O</span><span style="color: #a5ff00">L</span><span style="color: #9fff00">O</span><span style="color: #9aff00">v</span><span style="color: #95ff00">4</span><span style="color: #8fff00"> </span><span style="color: #8aff00">模</span><span style="color: #85ff00">型</span><span style="color: #80ff00">网</span><span style="color: #7aff00">络</span><span style="color: #75ff00">结</span><span style="color: #70ff00">构</span></div><div><span style="color: #6aff00">-</span><span style="color: #65ff00"> </span><span style="color: #60ff00">内</span><span style="color: #5aff00">置</span><span style="color: #55ff00">集</span><span style="color: #50ff00">成</span><span style="color: #4aff00"> </span><span style="color: #45ff00">Y</span><span style="color: #40ff00">O</span><span style="color: #3aff00">L</span><span style="color: #35ff00">O</span><span style="color: #30ff00">v</span><span style="color: #2bff00">3</span><span style="color: #25ff00"> </span><span style="color: #20ff00">模</span><span style="color: #1bff00">型</span><span style="color: #15ff00">网</span><span style="color: #10ff00">络</span><span style="color: #0bff00">结</span><span style="color: #05ff00">构</span></div><div><span style="color: #00ff00">-</span><span style="color: #00ff05"> </span><span style="color: #00ff0a">以</span><span style="color: #00ff10">及</span><span style="color: #00ff15">优</span><span style="color: #00ff1a">秀</span><span style="color: #00ff1f">的</span><span style="color: #00ff24">部</span><span style="color: #00ff2a">分</span><span style="color: #00ff2f">改</span><span style="color: #00ff34">进</span><span style="color: #00ff39">模</span><span style="color: #00ff3e">型</span></div><div><span style="color: #00ff44">-</span><span style="color: #00ff49"> </span><span style="color: #00ff4e">Y</span><span style="color: #00ff53">O</span><span style="color: #00ff58">L</span><span style="color: #00ff5e">O</span><span style="color: #00ff63">-</span><span style="color: #00ff68">F</span><span style="color: #00ff6d">a</span><span style="color: #00ff72">c</span><span style="color: #00ff78">e</span><span style="color: #00ff7d">V</span><span style="color: #00ff82">2</span><span style="color: #00ff87">模</span><span style="color: #00ff8d">型</span><span style="color: #00ff92">网</span><span style="color: #00ff97">络</span><span style="color: #00ff9c">结</span><span style="color: #00ffa1">构</span></div><div><span style="color: #00ffa7">-</span><span style="color: #00ffac"> </span><span style="color: #00ffb1">T</span><span style="color: #00ffb6">P</span><span style="color: #00ffbb">H</span><span style="color: #00ffc1">-</span><span style="color: #00ffc6">Y</span><span style="color: #00ffcb">O</span><span style="color: #00ffd0">L</span><span style="color: #00ffd5">O</span><span style="color: #00ffdb">v</span><span style="color: #00ffe0">5</span><span style="color: #00ffe5">模</span><span style="color: #00ffea">型</span><span style="color: #00ffef">网</span><span style="color: #00fff5">络</span><span style="color: #00fffa">结</span><span style="color: #00ffff">构</span></div><div><span style="color: #00faff">-</span><span style="color: #00f4ff"> </span><span style="color: #00efff">Y</span><span style="color: #00eaff">O</span><span style="color: #00e4ff">L</span><span style="color: #00dfff">O</span><span style="color: #00daff">v</span><span style="color: #00d5ff">5</span><span style="color: #00cfff">-</span><span style="color: #00caff">L</span><span style="color: #00c5ff">i</span><span style="color: #00bfff">t</span><span style="color: #00baff">e</span><span style="color: #00b5ff">模</span><span style="color: #00afff">型</span><span style="color: #00aaff">网</span><span style="color: #00a5ff">络</span><span style="color: #009fff">结</span><span style="color: #009aff">构</span></div><div><span style="color: #0095ff">-</span><span style="color: #008fff"> </span><span style="color: #008aff">P</span><span style="color: #0085ff">P</span><span style="color: #0080ff">Y</span><span style="color: #007aff">O</span><span style="color: #0075ff">L</span><span style="color: #0070ff">O</span><span style="color: #006aff">模</span><span style="color: #0065ff">型</span><span style="color: #0060ff">网</span><span style="color: #005aff">络</span><span style="color: #0055ff">结</span><span style="color: #0050ff">构</span></div><div><span style="color: #004aff">-</span><span style="color: #0045ff"> </span><span style="color: #0040ff">P</span><span style="color: #003aff">i</span><span style="color: #0035ff">c</span><span style="color: #0030ff">o</span><span style="color: #002bff">D</span><span style="color: #0025ff">e</span><span style="color: #0020ff">t</span><span style="color: #001bff">模</span><span style="color: #0015ff">型</span><span style="color: #0010ff">网</span><span style="color: #000bff">络</span><span style="color: #0005ff">结</span><span style="color: #0000ff">构</span></div> 
<!-- - 内置集成 YOLOv5 模型网络结构
- 内置集成 YOLOR 模型网络结构
- 内置集成 YOLOX 模型网络结构
- 内置集成 YOLOv7 模型网络结构
- 内置集成 Scaled_YOLOv4 模型网络结构
- 内置集成 YOLOv4 模型网络结构
- 内置集成 YOLOv3 模型网络结构
- 以及优秀的部分改进模型
- YOLO-FaceV2模型网络结构
- TPH-YOLOv5模型网络结构
- YOLOv5-Lite模型网络结构
- PPYOLO模型网络结构
- PicoDet模型网络结构 -->
...

以上多种检测算法使用统一模型代码框架，**集成在 YOLOAir 库中，统一任务形式、统一应用方式**。🌟便于科研者用于论文算法模型改进，模型对比，实现网络组合多样化。🌟工程算法部署落地更便捷，包含轻量化模型和精度更高的模型，根据场景合理选择，在精度和速度俩个方面取得平衡。同时该库支持解耦不同的结构和模块组件，让模块组件化，通过组合不同的模块组件，用户可以根据不同数据集或不同业务场景自行定制化构建不同检测模型。

🚀模型支持导出ONNX进行TensorRT推理，落地部署。

🚀支持加载YOLOv3、YOLOv4、YOLOv5、YOLOv7、YOLOR等网络的官方预训练权重进行迁移学习

🚀支持更多Backbone

- `CSPDarkNet系列`、(多种)
`ResNet系列`、(多种)
`ShuffleNet系列`、(多种)
`Ghost系列`、(多种)
`MobileNet系列`、(多种)
`ConvNext系列`、
`RepLKNet系列`、
`RepBlock系列`、(多种)
`自注意力Transformer系列`、(多种)
持续更新中🎈

🚀支持更多Neck

- neck包含FPN、PANet、BiFPN等主流结构。
 持续更新中🎈

🚀支持更多检测头Head  
-  YOLOv4、YOLOv5 Head检测头、
-  YOLOvR 隐式学习Head检测头、
-  YOLOX的解耦合检测头Decoupled Head、DetectX Head
-  自适应空间特征融合 检测头ASFF Head、
-  YOLOv7检测头IAuxDetect Head, IDetect Head等；

🚀支持更多即插即用的注意力机制
- 在网络任何部分即插即用式使用注意力机制，例如SE、CBAM、CA、GAM、ECA...等多种主流注意力机制  
[详情](https://github.com/iscyy/yoloair/blob/main/docs/document/attention.md)

🚀支持更多IoU损失函数
- CIoU、DIoU、GIoU、EIoU、SIoU、alpha IOU等损失函数；  
[详情](https://blog.csdn.net/qq_38668236?type=blog)

🚀支持更多NMS  
- NMS、Merge-NMS、DIoU-NMS、Soft-NMS、CIoU_NMS、DIoU_NMS、GIoU_NMS、EIoU_NMS、SIoU_NMS等;  
[详情](https://blog.csdn.net/qq_38668236?type=blog)

🚀支持更多数据增强
- Mosaic、Copy paste、Random affine(Rotation, Scale, Translation and Shear)、MixUp、Augment HSV(Hue, Saturation, Value、Random horizontal flip

🚀支持更多Loss
- ComputeLoss、ComputeNWDLoss、ComputeXLoss、ComputeLossAuxOTA(v7)、ComputeLossOTA(v7)等
[详情](https://blog.csdn.net/qq_38668236?type=blog)

🚀支持加权框融合(WBF)

🚀 内置多种网络模型模块化组件
- Conv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, GhostConv, 等
详细代码 **./models/common.py文件** 内搜索🔍👉[对应模块链接](https://github.com/iscyy/yoloair/blob/main/models/common.py)

- 👉[网络模型结构图](https://github.com/iscyy/yoloair/blob/main/docs/document/model_.md) 

以上组件模块使用统一模型代码框架、统一任务形式、统一应用方式，**模块组件化**🚀 可以帮助用户自定义快速组合Backbone、Neck、Head，使得网络模型多样化，助力科研改进检测算法，构建更强大的网络模型。

### 内置网络模型配置支持✨

🚀包括YOLOv3、YOLOv4、Scaled_YOLOv4、YOLOv5、YOLOv6、YOLOv7、YOLOX、YOLOR、Transformer、YOLO-FaceV2、PicoDet、YOLOv5-Lite、PPYOLO、TPH-YOLOv5、**其他多种改进网络结构等算法模型**的yaml配置文件汇总

[多种内置yaml网络模型配置(推荐🌟🌟🌟🌟🌟)](https://blog.csdn.net/qq_38668236/article/details/126237396)

🚀用户可自行改进网络

YOLOv7官方仓库目前一直在更新

## 使用🍉

**About the code.** Follow the design principle of [YOLOv5](https://github.com/ultralytics/yolov5).  
The original version was created based on YOLOv5(v6.1)

### 安装

在**Python>=3.7.0** 的环境中克隆版本仓并安装 requirements.txt，包括**PyTorch>=1.7**。

```bash
$ git clone https://github.com/iscyy/yoloair.git  # 克隆
$ cd YOLOAir
$ pip install -r requirements.txt  # 安装
```

### 训练

```bash
$ python train.py --data coco128.yaml --cfg configs/yolov5/yolov5s.yaml #默认为yolo
```

### 推理

`detect.py` 在各种数据源上运行推理, 并将检测结果保存到 `runs/detect` 目录。

```bash
$ python detect.py --source 0  # 网络摄像头
                          img.jpg  # 图像
                          vid.mp4  # 视频
                          path/  # 文件夹
                          path/*.jpg  # glob
```

### 融合
如果您使用不同模型来推理数据集，则可以使用 wbf.py文件 通过加权框融合来集成结果。
您只需要在 wbf.py文件 中设置 img 路径和 txt 路径。
```bash
$ python wbf.py
```

### Benchmark
Updating...

### YOLO网络模型具体改进方式教程及原理参考

- 1.[改进YOLOv5系列：1.YOLOv5_CBAM注意力机制修改(其他注意力机制同理)](https://blog.csdn.net/qq_38668236/article/details/126086716)

- 2.[改进YOLOv5系列：2.PicoDet结构的修改](https://blog.csdn.net/qq_38668236/article/details/126087343?spm=1001.2014.3001.5502)

- 3.[改进YOLOv5系列：3.Swin Transformer结构的修改](https://blog.csdn.net/qq_38668236/article/details/126122888?spm=1001.2014.3001.5502)

- 4.[改进YOLOv5系列：4.YOLOv5_最新MobileOne结构换Backbone修改](https://blog.csdn.net/qq_38668236/article/details/126157859)

- 5.[改进YOLOv5系列：5.CotNet Transformer结构的修改](https://blog.csdn.net/qq_38668236/article/details/126226726)

- 6.[改进YOLOv5系列：6.修改Soft-NMS,Soft-CIoUNMS,Soft-SIoUNMS](https://blog.csdn.net/qq_38668236/article/details/126245080)

- 7.[改进YOLOv5系列：7.修改DIoU-NMS,SIoU-NMS,EIoU-NMS,CIoU-NMS,GIoU-NMS](https://blog.csdn.net/qq_38668236/article/details/126243834)

- 8.[改进YOLOv5系列：8.增加ACmix结构的修改,自注意力和卷积集成](https://blog.csdn.net/qq_38668236/article/details/126302599)

- 9.[改进YOLOv5系列：9.BoTNet Transformer结构的修改](https://blog.csdn.net/qq_38668236/article/details/126333061)

更多模块详细解释教程持续更新中。CSDN博客搜索🔍【芒果汁没有芒果】🥭

### YOLOv5官方教程✨
与YOLOv5框架同步

- [训练自定义数据](https://github.com/ultralytics/yolov5/wiki/Train-Custom-Data)  🚀 推荐
- [获得最佳训练效果的技巧](https://github.com/ultralytics/yolov5/wiki/Tips-for-Best-Training-Results)  ☘️ 推荐
- [使用 Weights & Biases 记录实验](https://github.com/ultralytics/yolov5/issues/1289)  🌟 新
- [Roboflow：数据集、标签和主动学习](https://github.com/ultralytics/yolov5/issues/4975)  🌟 新
- [多GPU训练](https://github.com/ultralytics/yolov5/issues/475)
- [PyTorch Hub](https://github.com/ultralytics/yolov5/issues/36)  ⭐ 新
- [TFLite, ONNX, CoreML, TensorRT 导出](https://github.com/ultralytics/yolov5/issues/251) 🚀
- [测试时数据增强 (TTA)](https://github.com/ultralytics/yolov5/issues/303)
- [模型集成](https://github.com/ultralytics/yolov5/issues/318)
- [模型剪枝/稀疏性](https://github.com/ultralytics/yolov5/issues/304)
- [超参数进化](https://github.com/ultralytics/yolov5/issues/607)
- [带有冻结层的迁移学习](https://github.com/ultralytics/yolov5/issues/1314) ⭐ 新
- [架构概要](https://github.com/ultralytics/yolov5/issues/6998) ⭐ 新

</details>

### 未来增强✨
后续会持续建设和完善 YOLOAir 生态  
完善集成更多 YOLO 系列模型，持续结合不同模块，构建更多不同网络模型  
横向拓展和引入关联技术，如半监督学习等等  
跟进：YOLO-mask & YOLO-pose  

______________________________________________________________________

## Statement
<details><summary> <b>Expand</b> </summary>

* The content of this site is only for sharing notes. If some content is infringing, please sending email.

* If you have any question, please discuss with me by sending email.
</details>

## Acknowledgements

<details><summary> <b>Expand</b> </summary>
[https://github.com/ultralytics/yolov5](https://github.com/ultralytics/yolov5)  
[https://github.com/AlexeyAB/darknet](https://github.com/AlexeyAB/darknet)  
[https://github.com/ultralytics/yolov3](https://github.com/ultralytics/yolov3)  
[https://github.com/WongKinYiu/PyTorch_YOLOv4](https://github.com/WongKinYiu/PyTorch_YOLOv4)  
[https://github.com/WongKinYiu/ScaledYOLOv4](https://github.com/WongKinYiu/ScaledYOLOv4)   
[https://github.com/meituan/YOLOv6](https://github.com/meituan/YOLOv6)  
[https://github.com/WongKinYiu/yolov7](https://github.com/WongKinYiu/yolov7)  
[https://github.com/WongKinYiu/yolor](https://github.com/WongKinYiu/yolor)   
[https://github.com/xmu-xiaoma666/External-Attention-pytorch](https://github.com/xmu-xiaoma666/External-Attention-pytorch)  
[https://gitee.com/SearchSource/yolov5_yolox](https://gitee.com/SearchSource/yolov5_yolox)  
[https://github.com/Krasjet-Yu/YOLO-FaceV2](https://github.com/Krasjet-Yu/YOLO-FaceV2)  
[https://github.com/positive666/yolov5_research/](https://github.com/positive666/yolov5_research)  
[https://github.com/ppogg/YOLOv5-Lite](https://github.com/ppogg/YOLOv5-Lite)  
[https://github.com/Gumpest/YOLOv5-Multibackbone-Compression](https://github.com/Gumpest/YOLOv5-Multibackbone-Compression)  
[https://github.com/cv516Buaa/tph-yolov5](https://github.com/cv516Buaa/tph-yolov5)
</details>
