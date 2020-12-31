### 【一个理论上能正常使用的钉钉打卡脚本】

【解锁屏幕】【打卡结果反馈】【多时段打卡】【随机时间】【钉钉自动登录】

------

开源地址：https://github.com/fangyk-rel/DingDing-SayNo

该脚本用于Hamibot，你可以修改后用于Auto.js

### 更新日志

------

V3.2：  

- 新增 解锁方式，解锁成功率更高
- 新增 申请截图权限时自动确定

#### 安装脚本后你需要干什么？

------

#### 开启必要权限

- 无障碍权限

- 后台弹出界面，用于打开钉钉

- 后台锁定及电池优化白名单，保证Hamibot常驻后台

- 如果在配置中输入了百度OCR url或者勾选了上传截图，会申请截图权限  

  Tips：注意在权限弹出框中有一个隐藏的勾选框，瞎点几下勾选上，以后就不用重复弹出了

- 可能还有其他的.......

#### 脚本配置详解

- **【非必填】【公司名】：**  

  如果钉钉加入了多个公司，请输入公司名称，可以填写部分（例：改革春风吹满地，可以填改革、春风等等）,否则请置空

- **【必填】【上班打卡时间范围】：**  

  格式（08:00-09:00）支持多个打卡时间，以英文分号分隔(08:00-09:00;11:00-12:00)

- **【必填】【下班打卡时间范围】：**  

  同上

- **【非必填】【钉钉登录账号】**

  用于登录

- **【非必填】【钉钉登录密码】**

  同上

- **【必填】【打卡随机时间】：**  

  进入打卡页面后，会从10s~输入的时间内，随机选择一个时间并等待后，开始打卡（避免每天打卡时间相同）

- **【非必填】【解锁密码】：**  

  请填写数字密码，目前支持这个，不填表示上滑即解锁（没测试过所有机型，小米手机解锁失败的可以更换"MIUI11"这个主题试试）

- **【必填】【停顿时间】：**  

  默认3s，打不开钉钉的话，请调大该数字

- **【非必填】【server酱Url】：**  

  http://sc.ftqq.com/?c=wechat&a=bind 前往绑定，绑定后在“发送消息”中的SCKEY复制到此处输入框。用于推送打卡结果到微信

- **【非必填】【百度OCR】：**  

  填写百度OCR获取token的url，一般不用管这个

- **【非必选】【上传截图至图床】：**  

  勾选后，会将打卡截图上传至SM·MS图床，以及图片删除链接发送至server酱，你可以在微信中预览该图片，同时通过删除链接删除该图片（若不使用server酱，请勿勾选）
