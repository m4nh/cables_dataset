# Cables Dataset


The cable dataset, used for [Ariadne](https://github.com/m4nh/ariadne).

<p float="left">
<img  width=200 src='https://raw.githubusercontent.com/m4nh/cables_dataset/master/cable_dataset_simple/00000.jpg'/>
<img  width=200 src='https://raw.githubusercontent.com/m4nh/cables_dataset/master/cable_dataset_simple/00020.jpg'/>
<img  width=200 src='https://raw.githubusercontent.com/m4nh/cables_dataset/master/cable_dataset_simple/00050.jpg'/>
<img  width=200 src='https://raw.githubusercontent.com/m4nh/cables_dataset/master/cable_dataset_hard/00009.jpg'/>
<br>
<img  width=200 src='https://raw.githubusercontent.com/m4nh/cables_dataset/master/cable_dataset_simple/00000_mask_all.png'/>
<img  width=200 src='https://raw.githubusercontent.com/m4nh/cables_dataset/master/cable_dataset_simple/00020_mask_all.png'/>
<img  width=200 src='https://raw.githubusercontent.com/m4nh/cables_dataset/master/cable_dataset_simple/00050_mask_all.png'/>
<img  width=200 src='https://raw.githubusercontent.com/m4nh/cables_dataset/master/cable_dataset_hard/00009_mask_all.png'/>
</p>
<p >
First row depicts four samples of rgb source images; Second row represents corresponding binary masks.
</p>

## Format

The dataset is split in two parts: **cable_dataset_simple** and **cable_dataset_hard** (the **cable_dataset_reduced** part is just a reduced mix of both). Each folder 
contains a list of source images with corresponding labels with the following convention:

* **00000.jpg**: Source image
  * **00000_mask_N.png**: is the binary mask for the N-th cable.
  * **00000_mask_all.png**: is the binary mask for all cables in the image.
* **00000.txt**: the M-th row of this file contains coordinates for the M-th cable in the image. Each row is in the following format: ```K x0 y0 x1 y1 ... xk yk```: it is the 
list for the ```K``` coordinates of the simplified representation (spline control points) of the corresponding cable. (first numeber ```K``` si the number of coordinates pairs)

## Citation

If you use this dataset for your research, please cite our paper <a href="https://arxiv.org/abs/1810.04461">Let's take a Walk on Superpixels Graphs: Deformable Linear Objects Segmentation and Model Estimation</a>:

```
@article{degregorio2018,
  title={
Let's take a Walk on Superpixels Graphs: Deformable Linear Objects Segmentation and Model Estimation},
  author={De Gregorio, Daniele and Palli, Gianluca and Di Stefano, Luigi},
  journal={arXiv preprint arXiv:1810.04461},
  year={2018}
}
```
