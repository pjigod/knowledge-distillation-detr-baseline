# knowledge-distillation-detr-baseline

知识蒸馏实验使用的 RT-DETR 基线代码，作为后续改进方法的对照组。基于 [RT-DETR](https://github.com/lyuwenyu/RT-DETR)。

## 本仓库包含

- RT-DETR 和 RT-DETRv2 的代码与模型配置。
- PyTorch 和 Paddle 实现。
- 训练、评估等工具。

## 基线训练

先准备 COCO 数据集，并在 `RT-DETR-main/rtdetr_pytorch/configs/dataset/coco_detection.yml` 中设置数据路径。然后运行：

```powershell
cd RT-DETR-main/rtdetr_pytorch
pip install -r requirements.txt
python tools/train.py -c configs/rtdetr/rtdetr_r50vd_6x_coco.yml
```

## 来源

- 上游代码：[lyuwenyu/RT-DETR](https://github.com/lyuwenyu/RT-DETR)
- 许可证：[Apache-2.0](RT-DETR-main/LICENSE)
