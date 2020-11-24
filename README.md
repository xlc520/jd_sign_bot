<p align="center">
    <img src="https://cdn.jsdelivr.net/gh/ruicky/ruicky.github.io/2020/06/05/jd-sign/0.png">
</p>

<p align="center">
    <img alt="Version" src="https://img.shields.io/badge/release-0.0.1-blue"/>
    <a href="https://github.com/ruicky">
        <img alt="Author" src="https://img.shields.io/badge/author-ruicky-blueviolet"/>
    </a>
</p>

# 京东自动签到
功能：
1. 获取签到最新代码
2. 替换参数值
3. 签到并发送通知

详情参考文章:[京东定时签到-GitHub 实现](https://ruicky.me/2020/06/05/jd-sign/)

# 步骤
- 1.Fork
- 2.设置secret
  - Name: **JD_COOKIE**
  - Value: 你自己的 京东 cookie 值
  - 填写完成后 点击 Add secret 按钮
  
  - Name: **PUSH_KEY**
  - Value: 你自己的 server key 值
  - 填写完成后 点击 Add secret 按钮
- 3.任意提交一次

## 注意过一段时间cookie会失效，需要及时更新

- 获取cookie
  - 1. 电脑上打开 Chrome 浏览器，按 F12 打开开发者工具，并点击工具栏的左上角选择*手机模式*。
  - 2. 输入地址  https://plogin.m.jd.com/login/login  并打开网页，输入手机号验证码，点击登录。
  - 3. 选择右侧工具栏中的 console 控制台，然后在下放输入  copy(document.cookie)  回车，它会拷贝当前的 cookie， 然后在一个文本编辑器中或其他可编辑的窗口中复制出内容，并保存好，下方要用。
   - 注意： 1. 用手机号验证码登陆时间长一点，cookie一般会在24-28天左右失效，需要重新登陆获取，用  copy(document.cookie)  获取比较方便。
           2. 每次更新cookie需要重新更新一次 code ,随便提交一次就可以。
           3. 另外，可以进入个人中心 home.action 获取cookie

