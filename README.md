# News_Pro
这是一个仿网易新闻客户端的项目，正在进行中，持续更新......

| 首页        |      新闻详情           |  视频列表  |
| :-------------: |:-------------:| :------------:|
| ![首页](https://github.com/manofit/ScreenPics/blob/master/News_Pro_Pics/%E9%A6%96%E9%A1%B5.gif)     | ![图文详情](https://github.com/manofit/ScreenPics/blob/master/News_Pro_Pics/%E5%9B%BE%E6%96%87%E8%AF%A6%E6%83%85.gif) | ![视频列表](https://github.com/manofit/ScreenPics/blob/master/News_Pro_Pics/%E8%A7%86%E9%A2%91%E5%88%97%E8%A1%A8.gif) |
| 视频详情        |      搜索           |  我的  |
| ![视频详情](https://github.com/manofit/ScreenPics/blob/master/News_Pro_Pics/%E8%A7%86%E9%A2%91%E8%AF%A6%E6%83%85.gif)     | ![搜索](https://github.com/manofit/ScreenPics/blob/master/News_Pro_Pics/%E6%90%9C%E7%B4%A2.gif) | ![我的](https://github.com/manofit/ScreenPics/blob/master/News_Pro_Pics/%E4%B8%AA%E4%BA%BA%E4%B8%AD%E5%BF%83.gif) |

# Meituan
| ios01        |      ios02           |  ios03  |
| :-------------: |:-------------:| :------------:|
| ![ios01](https://github.com/manofit/ScreenPics/blob/master/MeiTuan/iOS_0.png)     | ![ios02](https://github.com/manofit/ScreenPics/blob/master/MeiTuan/iOS_1.png) | ![ios03](https://github.com/manofit/ScreenPics/blob/master/MeiTuan/iOS_2.png) |

# GoodList && PicShow
|   GoodList      |      PicShow           |
| :-------------: |:-------------:|
|![goodsList](https://github.com/manofit/ScreenPics/blob/master/PicShow%26GoodsLIst/goodsList.png)|![PicShow](https://github.com/manofit/ScreenPics/blob/master/PicShow%26GoodsLIst/pic_show.gif)|



# 常见错误记录。 
 从GitHub上下载的demo，运行之后报``'config.h' file not found``  
解决方法:  
1. 切换到项目的根目录下，然后执行: `cd node_modules/react-native/third-party/glog-0.3.5/`。  
	再执行`../../scripts/ios-configure-glog.sh`。这个方法试过不行。
2. 切换到项目的根目录下，然后执行: `cd node_modules/react-native/third-party/glog-0.3.5/`  
	再执行`./configure`。这个方法可以
⚠️注意：如果不知道`glog-0.3.5`的版本，可以先切换到`third-party`的目录下，然后`ls`查看文件，再跳转到相对应的目录，之后执行`./configure`

执行了上面的操作之后还会报一个错误，错误如下：`error: Build input file cannot be found: '/Users/xxx/xxx/xxx/node_modules/react-native/Libraries/WebSocket/libfishhook.a'`  
解决办法：打开Xcode，找到`Libraries`->`RCTWebSocket.xcodeproj`，点击Build Phases，再点击Link Binary With Libraries，找到`libfishhook.a`，点击之后点击减号`-`，把这个依赖项删除掉，然后点击加号，找到`libfishhook.a`依赖项再添加回来，然后build就好了。  
[参考网址1](https://blog.csdn.net/u010379595/article/details/82965506)
[参考网址2](https://blog.csdn.net/lzm150/article/details/84565365)
