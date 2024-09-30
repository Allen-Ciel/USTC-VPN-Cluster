# USTC-VPN-Cluster
记录一下MacOS配置的流程


## vpn账号开通
1. 需要填写一份文件盖章提交，开通vpn账号。找HJT老师（学院负责老师）盖章，然后扫描发给网络信息中心nic@ustc.edu.cn。

   ![image](https://github.com/user-attachments/assets/38189222-df00-486b-a6d4-67f90581cdb7)


3. 在设置中配置vpn。
   
   2.1 L2TP配置方法。（挂🪜也无法访问外网）

   具体参数和视频见https://ustcnet.ustc.edu.cn/2015/0127/c33586a592091/page.htm
   和
   https://ustcnet.ustc.edu.cn/2020/0107/c33586a592095/page.htm
 
  
  步骤见以下截图：

  
<img width="400" alt="image" src="https://github.com/user-attachments/assets/6f623fff-c025-466d-a07c-3ae31c280032">

<img width="400" alt="image" src="https://github.com/user-attachments/assets/75e985e0-4113-465b-83f6-b10a638bc598">

   2.2 Tunnelblick配置方法。（挂🪜可以访问外网）
   
   1）在 https://tunnelblick.net/index.html 网站下载软件

<img width="600" alt="image" src="https://github.com/user-attachments/assets/58465322-a3f0-4425-801f-8e99b0e005fb">

   2）在 http://openvpn.ustc.edu.cn/index.php 下载配置文件

   <img width="400" alt="image" src="https://github.com/user-attachments/assets/e9235e12-cafa-45b8-a831-7994868241f2">

   3）选择一个.ovpn文件拖拽到Tunnelblick左侧栏目

<img width="600" alt="image" src="https://github.com/user-attachments/assets/eb3daeff-6bca-4506-89f1-7d9647f8d999">

   4）会出现一些报错，和安全性提示。“设置”-“隐私与安全性”-下滑找到“启用系统扩展”
   
   <img width="600" alt="image" src="https://github.com/user-attachments/assets/bec86de1-a070-4ac6-901e-0a42bc67969c">

   5）会出现如下提示，需要开启系统权限，具体操作见网站教程 https://www.52mac.com/soft/13613-1-1.html
   或 [教程](./M1_M2_M3芯片%20Mac%20在“恢复”模式中启用系统扩展教程.pdf) 。
   
   <img width="400" alt="image" src="https://github.com/user-attachments/assets/ea05361e-2f6e-46eb-a388-93eb5a1e799e">

   6）重启之后返回“设置”-“隐私与安全性”-下滑找到“启用系统扩展”，应该还需要重启一次或两次电脑，直到没有“启用系统扩展”按钮。

   7）返回Tunnelblick软件，点击右下角的”连接“，输入 用户名 与 密码 即可。

   <img width="600" alt="image" src="https://github.com/user-attachments/assets/6a3982e8-70b0-4967-abfd-21e9456f7729">

## 集群连接
1. 申请开通账号
2. 校外需要连接vpn
3. 启动“终端”，选择“Shell”-“新建远程连接”
   
   <img width="358" alt="image" src="https://github.com/user-attachments/assets/d590ce13-8960-4f81-9004-1555c313c9d2">
   
<img width="500" alt="image" src="https://github.com/user-attachments/assets/01eb0b13-589e-4cd5-b01f-5b22a71a7698">



## 集群配置
1. module配置，每次启动都需要手动module load 模块，我基本只需要anaconda，所以在~/.bashrc添加module load anaconda3
2. 


