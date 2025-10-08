# RK3588-Based-Multi-Channel-Physical-Test-Counting-System  
---
This repository contains a multi-channel fitness rep counter system implemented on Orange Pi (RK3588) using YOLOv11-pose and QT. The UI is straightforward, as the author has no prior QT experience and used the most basic implementations.Welcome everyone to join in optimizing this project.




Usage Instructions
---
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







演示视频:  
---
<video src="https://github.com/user-attachments/assets/e71c0e9c-5271-4e9c-b2fb-d95266a63476" controls width="800">
  Your browser does not support the video tag.
</video>  







<img width="865" height="648" alt="展示" src="https://github.com/user-attachments/assets/07361ca2-8807-49b0-8b96-7c25d30a1d3f" />  


<img width="865" height="648" alt="image" src="https://github.com/user-attachments/assets/e7ebf89f-1819-4100-a079-b6bc3dcceeb7" />  







#########################################################################################################  
If the above procedure does not work, please consult the documentation:  

[rk3588多路体测系统文档.docx](https://github.com/user-attachments/files/22723281/rk3588.docx)
