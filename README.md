注：本插件 fork 自 kaiye/workflows-youdao,主要做了两点修改：
1. 修复登录有道账号失败异常，导致无法存储在本地
2. 增加了一个配置项，用于将查询过的单词存储为本地txt/markdown文件，方便随时以日为单位复习单词。效果如下：
3. 稍微改了一下本文件...

![image.png](http://ata2-img.cn-hangzhou.img-pub.aliyun-inc.com/a176c6358f3456756ac5da93170d9b5b.png)
![image.png](http://ata2-img.cn-hangzhou.img-pub.aliyun-inc.com/931c240369662f4216874ee3d06aba7d.png)

# kaiye/workflows-youdao

使用方法，选中需要翻译的文本，按两下 `command` 键即可。选中结果后，配合以下功能键可实现不同功能：

* `enter` 同步单词到有道在线单词本（若未配置有道账号则保存至本地单词本）
* `alt + enter` 翻译至剪切板
* `shift + enter` 直接发音
* `control + enter` 打开有道翻译页面
* `command + enter` 直接在光标处打出翻译结果

## 安装

### 1、[点击下载](https://github.com/k42jc/workflows-youdao/raw/master/youdao.alfredworkflow)

### 2、安装后设置双击快捷键

![按两下 command 设置快捷键](https://cloud.githubusercontent.com/assets/344283/12189204/b0d21524-b5f6-11e5-9cc8-33c17561f9ee.gif)

**建议设置为【alt+d】**

### 3、配置有道词典账号信息

![image.png](http://ata2-img.cn-hangzhou.img-pub.aliyun-inc.com/7fe87188c4cca058d5b7425bd78119d9.png)

![image.png](http://ata2-img.cn-hangzhou.img-pub.aliyun-inc.com/3a0721c724ddec2c69baed82c66cc6bd.png)

如上图所示，双击 alt 相关的 Run Script，在弹出的 Script 框中参照以上格式配置相关参数：

* `-filepath` 指定本地单词本的绝对路径，若不设置则默认为当前用户 Documents/Alfred-youdao-wordbook.xml 路径
* `-textpath` 指定本地txt/markdown绝对路径，以日为维度分隔存储
* `-username` 有道词典用户邮箱，用于模拟登录、同步单词信息
* `-password` 有道词典用户密码



## 演示

### 英译中

![](http://ww2.sinaimg.cn/large/48910e01gw1erucr05z85g213p0kbqhn.gif)

### 中译英

![](http://ww2.sinaimg.cn/large/48910e01gw1erucrd5tnmg213p0kbk6q.gif)

### 翻译短语

![](http://ww2.sinaimg.cn/large/48910e01gw1erucrvb9a8g213p0kbqhn.gif)

### 使用浏览器搜索

![](http://ww4.sinaimg.cn/large/48910e01gw1erucsmvtkgg213l0kaqq2.gif)

### 输出结果到光标所在应用程序

![](http://ww3.sinaimg.cn/large/48910e01gw1eructbvt9rg213p0jh0wi.gif)

