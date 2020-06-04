# VSCode Remote 云端开发指南

## 🤔写在前面
- 本地系统： Mac OS
- 云端系统： centos
- 云端用户：root
 

## 🚶Steps

- 绑定本地ssh公钥到云端实例，[查看步骤](https://cloud.tencent.com/document/product/213/35700#.E4.BD.BF.E7.94.A8.E5.AF.86.E9.92.A5.E7.99.BB.E5.BD.95)
- 本地 VScode 上安装 remote development
- 点击左侧小电视，点击 + 号，在命令行输入ssh [name]@[hostIp]
- 打开 VSCode 命令行(shift+command+p), 输入open config, 选择Remote SSH: Open Configuration File, 选择 /Users/hong/.ssh/config, 输入配置 
  
    Host Tcloud
    
    HostName [hostIp]

    User root

    ForwardAgent yes
-  连接到远端，根据提示打开文件夹



### 📖参考

[Visual Studio Code 远程开发探秘](https://cloud.tencent.com/developer/article/1476533)

[使用 SSH 登录 Linux 实例](https://cloud.tencent.com/document/product/213/35700#.E4.BD.BF.E7.94.A8.E5.AF.86.E9.92.A5.E7.99.BB.E5.BD.95)
