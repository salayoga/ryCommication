# ryCommication
融云通讯web端对接代码

自己对接融云通讯web端的代码,包括发送文字图片和文件功能,历史消息和小视屏语音由于后台权限
这里没有添加，自己可以参照文档进行对接。

20200518.md  这是我的appkey和自己模拟生成的token,项目中由后台传输。

rongcloud-web-im-upload-master 这个文件夹是融云提供的图片上传的参考,图片保存在七牛云,我在代码已经实现，也可以上传到自己的服务器。

test.html是图片上传测试文件

除了上面结果文件外，其余全部导入就可以看到效果了。

说一下主要代码：
html和css部分是我实现的样式，具体的自己修改。
前面的6个create文件是用于消息展示的,自己看情况修改（非必须）
cutImageBase64 文件压缩和转base64方法,由于融云只支持80kb以下的图片文件,这里就用的自己的压缩代码,在发送消息的时候把他的base64路径替换成自己的就行了。
下面的基本都是融云官方代码,可以参考注释,个人较懒就不写太多了,代码有什么不理解的可以咨询.

融云开发者文档：https://docs.rongcloud.cn/v3/views/im/noui/guide/private/msgmanage/msgsend/web3.html
token获取:https://developer.rongcloud.cn/apitool/-fAhAh2XeCJoygEf5Cpj2w
