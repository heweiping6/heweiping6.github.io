
### how to install gt730 driver on ubuntu 18.04.4(only driver)

[ref link](https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html)

Pick up usefull info:

```bash
###########################part 1
lspci | grep nvi -i 
#01:00.0 VGA compatible controller: NVIDIA Corporation GK208B [GeForce GT 730] (rev a1)

sudo apt-get update
sudo apt-get upgrade
reboot #reboot the system

###########################part 2
sudo apt-get install build-essential
sudo apt-get install linux-headers-$(uname -r)
#install dkms
sudo apt-get install dkms
sudo apt-get update
sudo apt-get upgrade
reboot #reboot the system

###########################part 3
# check nouveau
lsmod | grep nouveau

#disable nouveau
sudo vim /etc/modprobe.d/blacklist-nouveau.conf # with the following contents:
blacklist nouveau
options nouveau modeset=0

#update initramfs
sudo update-initramfs -u
reboot #reboot the system

###########################part 4
#enter  F8
#append runlevel 3 under grub, F10, boot with text mode.
ubuntu-drivers  devices
apt-get  install  nvidia-driver-435
reboot #reboot the system

#NOTE: ENTER A NEW SECURITY BOOT KEY AND REMEMBER IT, AFTER REBOOT BEFORE STARTUP, WE NEED ENTER AND VERIFY. OTHERWISE, NEW DRIVER WILL NOT ENABLE.

###########################part 5
lsmod  | grep nvi -i
#nvidia_uvm            876544  0
#nvidia_drm             49152  3
#nvidia_modeset       1122304  5 nvidia_drm
#nvidia              19517440  175 nvidia_uvm,nvidia_modeset
#.....

nvidia-smi
#Mon Mar  2 09:59:42 2020       
#+-----------------------------------------------------------------------------+
#| NVIDIA-SMI 435.21       Driver Version: 435.21       CUDA Version: 10.1     |
#|-------------------------------+----------------------+----------------------+
#| GPU  Name        Persistence-M| Bus-Id        Disp.A | Volatile Uncorr. ECC |
#| Fan  Temp  Perf  Pwr:Usage/Cap|         Memory-Usage | GPU-Util  Compute M. |
#|===============================+======================+======================|
#|   0  GeForce GT 730      Off  | 00000000:01:00.0 N/A |                  N/A |
#| 30%   33C    P8    N/A /  N/A |     37MiB /  2002MiB |     N/A      Default |
#+-------------------------------+----------------------+----------------------+
#                                                                               
#+-----------------------------------------------------------------------------+
#| Processes:                                                       GPU Memory |
#|  GPU       PID   Type   Process name                             Usage      |
#|=============================================================================|
#|    0                    Not Supported                                       |
#+-----------------------------------------------------------------------------+

```


