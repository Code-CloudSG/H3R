# Heatmap Regression via Randomized Rounding
----

**[2020/07/27]**: the paper is available on [ArXiv]().


## Introduction

This repo contains the facial landmark detection code for "Heatmap Regression via Randomized Rounding".

![demo image](data/selfie.jpg.png)

## Get Started

````bash
pip install -r requirements.txt
````

## Demo
````bash
export PYTHONPATH=./:$PYTHONPATH
python examples/demo.py --image data/demo.jpg --model models/wflw/p1/hrnet18/256x256/
````

## Test on WFLW

```bash
ln -s path/to/WFLW_images/ data/WFLW/images
```

````bash
python examples/test.py --model models/wflw/hrnet18_256x256_p1/
````

| Backbone | BBox | Resolution | #Params | GFLOPs | NME (%)| 
|:--:|:--:|:--:|:--:|:--:|:--:|
| HRNet-W18 | P1 | 256x256 | 9.69M | 4.84G | 3.81 |
| HRNet-W18 | P2 | 256x256 | 9.69M | 4.84G | 3.95 |
| MobileNetV2 | P2 | 256x256 | 0.60M | 0.51G | 4.45 |

## Citation

```
@article{yu2020heatmap,
  title   = {Heatmap Regression via Randomized Rounding},
  author  = {Yu, Baosheng and Tao, Dacheng},
  journal= {arXiv preprint arXiv:},
  year={2020}
}
```


## Contact

Baosheng Yu, baosheng.yu.usyd@gmail.com.


## Acknowledgement

[https://github.com/HRNet](https://github.com/HRNet)

