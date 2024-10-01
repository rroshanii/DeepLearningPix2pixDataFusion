# DeepLearningPix2pixDataFusion

!git clone https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix
%cd /content/drive/MyDrive/DL/pytorch-CycleGAN-and-pix2pix-master/pytorch-CycleGAN-and-pix2pix-master
!pip install -r requirements.txt 
!pip install dominate
!pip install wandb
من توی کلب کار کردم
!bash /content/drive/MyDrive/DL/pytorch-CycleGAN-and-pix2pix-master/pytorch-CycleGAN-and-pix2pix-master/datasets/download_pix2pix_dataset.sh facades
!python /content/drive/MyDrive/DL/pytorch-CycleGAN-and-pix2pix-master/pytorch-CycleGAN-and-pix2pix-master/datasets/facades/ --dataroot /content/drive/MyDrive/DL/pytorch-CycleGAN-and-pix2pix-master/pytorch-CycleGAN-and-pix2pix-master/datasets/facades --name facades_pix2pix --model pix2pix --n_epochs 100 --n_epochs_decay 50
!ln -s /content/drive/MyDrive/DL/pytorch-CycleGAN-and-pix2pix-master/pytorch-CycleGAN-and-pix2pix-master/checkpoints/facades_pix2pix/latest_net_G.pth ./checkpoints/facades_pix2pix/latest_net_G.pth
!python /content/drive/MyDrive/DL/pytorch-CycleGAN-and-pix2pix-master/pytorch-CycleGAN-and-pix2pix-master/test.py --results_dir /content/drive/MyDrive/result --dataroot /content/drive/MyDrive/DL/pytorch-CycleGAN-and-pix2pix-master/pytorch-CycleGAN-and-pix2pix-master/datasets/facades/ --name facades_pix2pix --model pix2pix

