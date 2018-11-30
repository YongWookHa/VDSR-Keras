
# VDSR-Keras

### Overview

VDSR(Very Deep Super-Resolution) implemented in Keras.
You can find further information in [the author's page](https://cv.snu.ac.kr/research/VDSR/)

This VDSR code is based on [GeorgeSeif's VDSR-Keras](https://github.com/GeorgeSeif/VDSR-Keras).

I modified the original code for using.
This code is intended to be simpler and more convinient to use than the original one.

### Files
* `vdsr.py` : Contains model.
* `predict.py` : Use the trained model for super-resolution.

### Usage

#### vdsr.py
* Put your dataset folder into `data` directory. (recommend to use jpg)
*  > You need to prepare 2 sets of data.
`x` : Low resolution image data. 
`y` : High resolution image data which have `TARGET_IMG_SIZE`.

* Set parameters to your data [here](https://github.com/YongWookHa/VDSR-Keras/blob/f810543f700717a2e1ae884c2f409ac0265e88a5/vdsr.py#L16)
* Run `vdsr.py` to train the model.

#### predict.py
* > `predict.py` has four parameters to set.
`json_path` : Path of model architecture.
`w_path` : Path of model weights.
`img_path` : Path of images to be up-scaled.
`dst_path` : Path to save the up-scaled images.

* `target_size` has to be set according to size of output image.

* Run `predict.py` with console prompt.

Enjoy.
