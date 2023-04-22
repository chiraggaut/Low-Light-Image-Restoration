# Low-Light-Image-Restoration


1)Change directory to ./LLFlow/code

2)Create 3 folders here: the input folder, the output folder(where ouputs will be stored) and the high-res folder, which contains the high resolution images (to calculate PSNR)

3)Run eval.py with 3 input arguments: python eval.py --inputdir input --outputdir output --highdir high. PSNR for each example and time taken will be displayed.

4)For training (fine-tuning), run the script python train.py. (No input arguments required). The pretrained LLFlow model is finetuned for 6 epochs on the custom dataset named collective_dataset. The scriptlogs the training results and saves the best model. Results can be visualised through tensorboard

5)Dataset paths, model weights can be set in the config file (./code/confs/LOL_smallNet.yml)
