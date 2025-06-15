# LHATA-Net
<details open>
<summary>Install</summary>
  
Pip install the ultralytics package including all [requirements](https://github.com/ultralytics/ultralytics/blob/main/pyproject.toml) in a [**Python>=3.8**](https://www.python.org/) environment with [**PyTorch>=1.8**](https://pytorch.org/get-started/locally/).

Pip install the other pakage.
```bash
pip install -r requirements.txt
=======
pip install -U openmim
mim install mmengine
mim install "mmcv>=2.0.0"
```

<details open>
<summary>Run</summary>

Train with LHATA-Net:
```bash
cd ultralytics-8.1.9
```
```bash
yolo cfg=<path_to_your_cfg> model=LHATA-Net.yaml imgsz=640 epoch=300 batch=64 device=0,1,2,3,4,5,6,7 optimizer=SGD deterministic=False amp=False 
```
