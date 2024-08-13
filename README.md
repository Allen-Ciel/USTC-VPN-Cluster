# USTC-VPN-Cluster
记录一下MacOS配置的流程


## vpn账号开通
1. 需要填写一份文件盖章提交，开通vpn账号。具体待确认。
2. 在设置中配置vpn。具体参数和视频见https://ustcnet.ustc.edu.cn/2015/0127/c33586a592091/page.htm和https://ustcnet.ustc.edu.cn/2020/0107/c33586a592095/page.htm
  步骤见以下截图：
<img width="400" alt="image" src="https://github.com/user-attachments/assets/ef0a6dce-90bd-458b-a56c-5f04b76a519f">

<img width="400" alt="image" src="https://github.com/user-attachments/assets/75e985e0-4113-465b-83f6-b10a638bc598">

## 集群连接
1. 申请开通账号
2. 校外需要连接vpn
3. 启动“终端”，选择“Shell”-“新建远程连接”
   
   <img width="358" alt="image" src="https://github.com/user-attachments/assets/d590ce13-8960-4f81-9004-1555c313c9d2">
   
<img width="500" alt="image" src="https://github.com/user-attachments/assets/90866bed-c2a2-4deb-868d-aee9ec26e2b9">

## 集群配置
1. module配置，每次启动都需要手动module load 模块，我基本只需要anaconda，所以在~/.bashrc添加module load anaconda3
2. 


