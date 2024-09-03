We build our code for FLoD on top of the open-source code of 3D Gaussian Splatting.
In accordance with the licensing requirements, we have not deleted any license information from the base code. 

Our code was tested on conda environment installed with environment.yml and the submodules written below.

For submodule installation, run the following commands at /path/to/flod_code:
git clone https://github.com/graphdeco-inria/diff-gaussian-rasterization submodules/diff-gaussian-rasterization
git clone https://gitlab.inria.fr/bkerbl/simple-knn.git submodules/simple-knn
sudo apt install libglm-dev
pip install submodules/diff-gaussian-rasterization
pip install submodules/simple-knn

To reproduce, run...
train_{dataset_name}.sh to train 3DGS-FLoD
render_single.sh for individual level rendering of 3DGS-FLoD
render_selective.sh for selective rendering of 3DGS-FLoD

To run viewer (as the demo in our project page)
run convert4viewer.sh and run ./SIBR_viewers/install/bin/SIBR_flodViewer_app /path/to/your/model
