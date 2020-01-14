# subpackage

#### 介绍
1.生成母包信息：包含ios ipa包 ，安卓 apk包  2.根据母包自动生成渠道包

#### 软件架构
subPackage 用到的库文件  
sub.php    入口文件

#### 安装教程

1.  下载zip文件，解压即可使用 

#### 使用说明

1.  根据自己项目，设置DOWNLOAD_DIR,PLIST_TMP_PATH 保证目录读写权限.项目读取info.plist信息时 会产生info.plist 到临时目录PLIST_TMP_PATH 
2.  参数$p 母包名 $a 渠道包名 如果$p=$a 是生成母包参数，写入数据库 如果$p!=$a则在母包基础上，打入渠道信息
3.  项目区分安卓，ios 包方式可以自行定义。目前支持ipa，apk两种包信息读取以及打入渠道信息。如有其它需求请自行扩展
4.  apk母包必须使用v1签名方式打包，不然可能出现渠道包安装不上的问题

![包目录结构说明](https://gitee.com/tongyh/subpackage/blob/master/dir-tmplate.png "tongyh")

### 问题反馈
使用中遇到任何问题，欢迎及时反馈！

#### 参与贡献

1.  Fork 本仓库
2.  新建 Feat_xxx 分支
3.  提交代码
4.  新建 Pull Request
