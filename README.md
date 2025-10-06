# RK3588-Based-Multi-Channel-Physical-Test-Counting-System
This repository contains a multi-channel fitness rep counter system implemented on Orange Pi (RK3588) using YOLOv11-pose and QT. The UI is straightforward, as the author has no prior QT experience and used the most basic implementations.



演示视频：
https://github.com/user-attachments/assets/b6fbceb8-f247-4e49-8748-1a7d1db5948d



<img width="865" height="648" alt="image" src="https://github.com/user-attachments/assets/c017c6ed-d0a3-4261-be20-15042f781b07" />  


Usage Instructions:  
一、Flashing the OS Image  
Prerequisites: TF card (8GB or larger), TF card reader, official Ubuntu image.  
  ① Download the official OS image from the manufacturer's website：http://www.orangepi.cn/html/hardWare/computerAndMicrocontrollers/service-and-support/Orange-pi-5.html  
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


四、Code Compilation and Execution  
  To compile the code:bash build-linux_RK3588.sh  
  To run the application: ./rknn_yolov11pose_demo  



#########################################################################################################################
按照上述流程不行的，参考文档：

[rk3588多路体测系统文档.docx](https://github.com/user-attachments/files/22723281/rk3588.docx)
