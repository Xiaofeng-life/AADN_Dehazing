# The document of code for AADN

The code is for the paper, ''Adversarial Attack and Defense for Dehazing Networks''. The arxiv link is, ''https://arxiv.org/pdf/2303.17255.pdf''.

If you have any suggestions, feel free to contact me (Email: cxf_svip@163.com). Thanks.

## 1. The structure of this code 
attack_utils： codes for attack

defense_utils: codes for defense

methods: network define and config

demo_dataset: datasets

results_attack: store the attack results (both before and after defense training)

results_train: store the original training checkpoints and defense training checkpoints

AADN_4KDehazing_defense.py/sh: defense training of 4Kdehazing

AADN_attack.py/sh: attack codes, can be used for 4KDehazing/GCANet

AADN_GCANet_defense.py/sh: defense training of GCANet

## 2. Some details
(1) The final dehazing results (displayed in paper) are all calculated by skimage. Therefore, the metrics during training process is just for analyzing the training process (will not be displayed in paper). 
Since all dehazing models set to the same epochs during training process. It is fine to delete the eval code
during process (epochs is fixed).