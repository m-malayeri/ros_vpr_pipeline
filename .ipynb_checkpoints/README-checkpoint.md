# LW Dataset Pipeline
This repository is a collection of ROS integrated functions that is used to process the bag files of the LW dataset. This pipeline provides functionalities such as extraction, merging, filtering, visualization, place ID generation, frame transformation, dataset split, and integrity check. The output of this flexible pipeline is then used to evaluate the performance of deep learning methods such as NetVLAD and Patch-NetVLAD. The LW dataset is a large-scale indoor industrial VPR dataset featuring images from four RGB-D cameras (mounted around a logistic robot) and their corresponding pose and IMU data. This dataset will be published soon after receiving approvals.

## Installing Dependencies
We suggest creating a separate conda environment for this repository. In your terminal, execute:

1. ``` conda create -n vpr_pipeline python numpy==1.26.4 ipykernel pycryptodomex pyyaml python-gnupg rospkg opencv matplotlib scikit-learn ```
2. ``` conda activate vpr_pipeline ```
3. ``` python -m ipykernel install --user --name=vpr_pipeline --display-name "Python (vpr_pipeline)" ```
4. ``` pip install rosbags-image ```

## Before Use
Adjust the path parameters to point to the dataset.