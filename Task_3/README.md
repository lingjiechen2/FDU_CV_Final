## 环境配置

```
pip install -r requirements.txt
```

<details>
  <summary> Dependencies (click to expand) </summary>
  
  ## Dependencies
  - PyTorch 1.4
  - matplotlib
  - numpy
  - imageio
  - imageio-ffmpeg
  - configargparse
  
The LLFF data loader requires ImageMagick.

You will also need the [LLFF code](http://github.com/fyusion/llff) (and COLMAP) set up to compute poses if you want to run on your own real data.

</details>

### 使用范例

Download data for two example datasets: `lego` and `fern`

```
bash download_example_data.sh
```

To train a low-res `lego` NeRF:

```
python run_nerf.py --config configs/lego.txt
```
