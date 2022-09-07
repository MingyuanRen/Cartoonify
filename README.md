
# Cartoonify

Cartoonify: a Serverless Machine Learning App

## CartoonGAN



If you're interested in the training procedure, have a look at the [CartoonGAN](https://openaccess.thecvf.com/content_cvpr_2018/papers/Chen_CartoonGAN_Generative_Adversarial_CVPR_2018_paper.pdf) paper

Download the four pretrained models first. These weights will be loaded inside the Generator model defined in cartoongan/network/Transformer.py
```
cd cartoongan
bash download_pth.sh
```


To test one of the four models, head over the notebook cartoongan/notebooks/CartoonGAN.ipynb and change the input image path to your test image. This notebook calls cartoongan/test_from_code.py script to make the transformation.
```
cd cartoongan/notebooks
jupyter notebook
```
## serverless API using AWS Lambda