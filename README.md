```
________                  ___________.__            .___            
\_____  \_______   ____   \_   _____/|__| ____    __| _/___________ 
 /   |   \_  __ \_/ __ \   |    __)  |  |/    \  / __ |/ __ \_  __ \
/    |    \  | \/\  ___/   |     \   |  |   |  \/ /_/ \  ___/|  | \/
\_______  /__|    \___  >  \___  /   |__|___|  /\____ |\___  >__|   
        \/            \/       \/            \/      \/    \/      
```
Implementation of YOLOv5 to detect ores in Minecraft, for the INFO8010 course.

## Project links
- Course page: https://github.com/glouppe/info8010-deep-learning
- Project page: https://github.com/glouppe/info8010-deep-learning/blob/master/project.md
- Project proposal: https://www.overleaf.com/7518417627ycrxkdktsnjc#f5cae5
- Project report: https://www.overleaf.com/3124452873pyhrsqkzqtpd#3ed97c

## Official model links
Official Implementation : https://github.com/ultralytics/yolov5/tree/master/models

YOLOV5 explained:
- https://iq.opengenus.org/yolov5/
- https://towardsai.net/p/l/yolov5m-implementation-from-scratch-with-pytorch
- https://sh-tsang.medium.com/brief-review-yolov5-for-object-detection-84cc6c6a0e3a
- https://github.com/ultralytics/yolov5/discussions/3181
- https://docs.ultralytics.com/fr/yolov5/tutorials/architecture_description/

## Dataset
- YOLOv5: https://universe.roboflow.com/yolo-minecraft/minecraft-ogpjp/dataset/10

## Wandb project
- https://wandb.ai/s-gardier-work?product=models

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
When running the notebook, make sure to select the kernel info8010).

### Wandb
Ref doc: https://docs.wandb.ai/quickstart/ (We use "W&B Models")

- First, activate from the terminal your conda env (the same you use in the notebook, i.e. info8010) and install wandb: `pip install wandb`
- Then, login with your wandb token: `wandb login <you_token>`
- You can find your token in your wandb account settings: https://wandb.ai/authorize
- Should be good :) Test with the wandb-test notebook, it should run fine and you should see a new run (takes a few seconds to appear) in the wandb workspace: https://wandb.ai/s-gardier-work/wandb-test/.
