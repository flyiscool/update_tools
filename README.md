### 软件升级工具

本工具为 px4 的 firmware 剥离出的脚本文件。用于延续用户的升级习惯，作为非开发者可以使用本工具对 coolfly 模组进行固件升级。

#### 环境说明
- window系统下如需使用，请预先安装windows下的开发环境。下载地址如下：   
```
    https://github.com/PX4/windows-toolchain
```
- ubuntu系统下可直接使用  

#### 天空端固件升级

将天空端编译出的 coolfly-f1_default.px4 文件拷贝到当前目录下，执行脚本 ./upgrade.sh ，给天空端上电即可进入升级界面。

#### 地面段固件升级
将地面端编译出的 app.px4 文件拷贝到当前目录下，按住地面端 reset 按键，执行脚本 ./upgrade.sh，放下 reset 键即可进入升级界面。

#### 备注
1. ./upgrade.sh 脚本会查找存在当前目录下的 px4 文件作为升级的文件，所以 UpgradeTool 目录下只能存在一个 .px4 文件，烧写天空端时只放天空端的 px4 文件，烧写地面端只放地面端的 px4 文件。