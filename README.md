```
________                  ___________.__            .___            
\_____  \_______   ____   \_   _____/|__| ____    __| _/___________ 
 /   |   \_  __ \_/ __ \   |    __)  |  |/    \  / __ |/ __ \_  __ \
/    |    \  | \/\  ___/   |     \   |  |   |  \/ /_/ \  ___/|  | \/
\_______  /__|    \___  >  \___  /   |__|___|  /\____ |\___  >__|   
        \/            \/       \/            \/      \/    \/      
```
# INFO8010 Project : OreFinder
Implementation of YOLOv5 to detect ores in Minecraft, for the INFO8010 course.

## Project files
- model.py : YOLOv5 model implementation.
- study_reference_model.py: Notebook used to study the YOLOv5 official model.
- train_reference_model: Notebook used to train the YOLOv5 official model on our dataset and study the feasability of the project.

## Dev environment
### Conda installation
```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh # Accept everything, say 'yes'...
conda init # Run it in a new terminal
conda create -n info8010
conda activate info8010
conda info --envs #check your conda envs
which python3 # check that the python version is the one from conda (something like /home/username/miniconda3/envs/info8010/bin/python3) 
conda install ipykernel
sudo apt install graphviz
```
When running the notebook, make sure to select the kernel info8010.

### Model download
- Dlownload the model .pth file from: https://drive.google.com/file/d/1DAsTbonuAwgIGh83tqrq6XZwUol1-57Y/view?usp=drive_link
- Place it at the root of the project folder.

## Model links
Official Implementation : https://github.com/ultralytics/yolov5/tree/master/models

YOLOV5 explained: 
- https://iq.opengenus.org/yolov5/
- https://towardsai.net/p/l/yolov5m-implementation-from-scratch-with-pytorch
- https://sh-tsang.medium.com/brief-review-yolov5-for-object-detection-84cc6c6a0e3a
- https://github.com/ultralytics/yolov5/discussions/3181

## Dataset
- YOLOv5: https://universe.roboflow.com/yolo-minecraft/minecraft-ogpjp/dataset/10

## Training supervision
- https://wandb.ai/s-gardier-work?product=models

## Project links
- Course page: https://github.com/glouppe/info8010-deep-learning
