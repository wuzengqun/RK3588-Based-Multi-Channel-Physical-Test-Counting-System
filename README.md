# RK3588-Based-Multi-Channel-Physical-Test-Counting-System
This repository contains a multi-channel fitness rep counter system implemented on Orange Pi (RK3588) using YOLOv11-pose and QT. The UI is straightforward, as the author has no prior QT experience and used the most basic implementations.



演示视频：
https://github.com/user-attachments/assets/b6fbceb8-f247-4e49-8748-1a7d1db5948d



<img width="865" height="648" alt="image" src="https://github.com/user-attachments/assets/c017c6ed-d0a3-4261-be20-15042f781b07" />
Usage Instructions:
一、Flashing the OS Image
Prerequisites: TF card (8GB or larger), TF card reader, official Ubuntu image.
  ① Download the official OS image from the manufacturer's website：http://www.orangepi.cn/html/hardWare/computerAndMicrocontrollers/service-and-support/Orange-pi-5.html
  <img width="256" height="193" alt="image" src="https://github.com/user-attachments/assets/46854c88-c350-471a-818f-7f86f33fa189" />
  <img width="307" height="353" alt="image" src="https://github.com/user-attachments/assets/431867da-eacc-4897-8d88-b921123e2728" />
  
  ② After the download is complete, use the image flashing tool included in the official package to flash the image onto the TF card.


二、Transferring This Repository Code to the Development Board
Prerequisites: One Ethernet cable, MobaXterm software.
    ①Connect the development board directly to your computer using the Ethernet cable. Configure the network settings on both sides to ensure they are on the same subnet and can ping each other successfully.
    ② Open the MobaXterm software, establish an SSH connection to the development board, and transfer the project to it.


三、Essential Environment Setup
Execute the following commands in the terminal:
①sudo apt-get update
②sudo apt-get install -y cmake
③sudo apt-get install -y qtbase5-dev qtdeclarative5-dev qttools5-dev


四、代码编译及运行
  编译代码：bash build-linux_RK3588.sh，等待编译完成即可
  代码运行： ./rknn_yolov11pose_demo

