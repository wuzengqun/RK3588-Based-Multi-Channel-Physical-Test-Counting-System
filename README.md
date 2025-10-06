# RK3588-Based-Multi-Channel-Physical-Test-Counting-System
This repository contains a multi-channel fitness rep counter system implemented on Orange Pi (RK3588) using YOLOv11-pose and QT. The UI is straightforward, as the author has no prior QT experience and used the most basic implementations.



演示视频：
https://github.com/user-attachments/assets/b6fbceb8-f247-4e49-8748-1a7d1db5948d



<img width="865" height="648" alt="image" src="https://github.com/user-attachments/assets/c017c6ed-d0a3-4261-be20-15042f781b07" />
使用方法：
一、镜像烧录
准备：tf卡（8g以上）、tf卡烧录器、官方ubuntu镜像
  ①进入官网下载镜像：http://www.orangepi.cn/html/hardWare/computerAndMicrocontrollers/service-and-support/Orange-pi-5.html
  <img width="256" height="193" alt="image" src="https://github.com/user-attachments/assets/46854c88-c350-471a-818f-7f86f33fa189" />
  <img width="307" height="353" alt="image" src="https://github.com/user-attachments/assets/431867da-eacc-4897-8d88-b921123e2728" />
  
  ②下载完成后使用官方提供的镜像烧录工具，将镜像烧录到tf卡中
  <img width="433" height="259" alt="image" src="https://github.com/user-attachments/assets/a6c06a5b-fded-489d-a10b-a0afcbddd2d9" />


二、将此仓库代码移动到开发板端
准备：网线一根、mobaxterm软件
    ①使用网线直接连接开发板和电脑，分别配置俩边的网络，确保处于同一网段并且可以ping通。
    ②打开mobaxterm软件，ssh连接上开发板，将项目移动到开发板中


三、必要环境安装
终端执行以下命令：
①sudo apt-get update
②sudo apt-get install -y cmake
③sudo apt-get install -y qtbase5-dev qtdeclarative5-dev qttools5-dev


四、代码编译及运行
  编译代码：bash build-linux_RK3588.sh，等待编译完成即可
  代码运行： ./rknn_yolov11pose_demo

