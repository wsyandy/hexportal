hexportal
=========

和谐数据 阿里云代理平台 控制台开源项目


和谐数据是我在2012年开发者大赛获奖后的准备着手做的一个项目，最初没准备开源，所以代码写得非常粗糙，即使中途改写过一些核心代码，依然很乱。

先来简单介绍下功能：

  阿里云主机代理平台，顾名思义就是代理阿里云主机ECS业务，本平台集主机管理、用户管理、账单系统于一身，功能齐全，且UI界面参照了业界著名的“青
  云”（北京优帆技术有限公司）的samantha大师的简洁风格影响，所有界面组件均使用FlatUI的元件完成，且兼容到了IE6（图标功能尚有些许BUG，若有精
  力请使用者自行完善）。

  
免责与法律声明：

  1.本项目开源所释出源代码仅供参照者用作学习研究之用途，未经本项目系统研发者及其所引用框架底层代码研发者授权，不允许商业用途。
  2.本项目所有研发者不对代码安全性做保证，用户使用其用于生产环境、二次开发的，因本项目系统BUG、漏洞等导致经济损失，本项目研发者不承担任何责任。
  3.开源是一种精神，不是义务。


使用教程：

    1.使用git clone git@gitshell.com:hexdata/hexpanel.git
    2.进入console/source/plugin/host/core，编辑api.php和api2.php中的access key和secret.
    3.将sql备份导入到数据库中
    4.编辑下述文件中的数据库配置信息：
        console/config/config_global.php
        console/config/config_ucenter.php
        console/uc_server/data/config.inc.php
    5.后台登录入口为console/ultraadmin.php，用户名为admin，密码为123456
    6.将ucenter与discuz的key配置成一致
    7.因为阿里云ECS接口限制，普通用户申请不到ECS自动开发接口，开通主机需要手工审核，而且需要在阿里云平台申请开通，然后在后台开通时补填主机编号（如“AY1302241021447dc7307”）、VMID（可以用谷歌浏览器抓包获取）、公网IP、内网IP
    8.代理折扣什么的，需要你自行与阿里云谈


演示:

  https://i.hexdata.cn/console/

赞助与支持：

  本作品正在参加阿里云开发者大赛（http://dasai.aliyun.com/signup/works2013/?search=11），您的一票就是对我最大的支持！

Some other tips:

    hexData console is an open source & business running project, All functions were based on Discuz!X2.5,
    UI Framework from @QingCloud( Beijing Yunify Technology LTD ). License Snapshot: http://t.cn/z85zacu

    Github:    https://github.com/hexdata/hexportal , Open License: Discuz License & GNU.
    36kr+:     http://www.36kr.net/hexieshuju
    17Startup: http://17startup.com/startup/view/21124

    This project work is being shown on Alibaba Cloud Start-up Competition, If you wanna small upon me, please vote +1 for No.11 on http://dasai.aliyun.com/signup/works2013/
    If you are an investors, and interested in this project, please contact hackes#outlook.com

    Thanks to everyone who helped hexData.
