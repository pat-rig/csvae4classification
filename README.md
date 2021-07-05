# 1) How to Run the Code?
## You need to set up a particular environment before running the notebooks:

`cd repo_path`

`conda env create -f environment.yml`

`source activate pDL`


## The model code as well as evaluation is stored in the jupyter notebooks

`vae.ipynb`contains a vanilla VAE based on
https://github.com/Atcold/pytorch-Deep-Learning/blob/master/11-VAE.ipynb

`conv_vae.ipynb` contains the superior extension of `vae.ipynb` which produces better generations through convolving z.

Hyper parameters, such as `beta`, number of layers and convolutional parameters need to be manipulated in-line.

# 2) Repo Structure

2.1) Executing either of the notebooks for the first time will create a data directory with the MNIST `/data` automatically.
Do not use other preprocessed versions of MNIST.

2.2) `/models` contains checkpoints of small training runs on a local machine. Parameter settings can be found in the file name.

2.3) fig_src contains samples and reconstructions for different models which are specified by the filename of the respective images.
