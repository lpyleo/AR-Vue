## 概述
本项目采用ar.js＋vite Vue3的框架进行编写
Vue3在这里的作用主要是用来启动https服务
如果后续大家有需要，可在本代码的基础上编写相应vue组件

## 案例展示
我在本仓库中放了相应的代码演示视频，这个比使用说明来的简单多了。演示视频为video.mp4。

## 代码下载即运行方法
1. git clone 本项目
2. 进入该项目文件夹
3. npm install下载相应node_moudle
4. npm run dev -- --https（启动项目以https的方式）
5. 等待项目加载完成，注意要联网

## 小结
我们对这个项目从0到实现，很多技术都是生搬硬套，所以存在许多不足之处，它包括

1. 放大缩小是直接用css对dom元素属性进行操作，而没有用到vue组件，因为我们在vue组件中导入不了相应的ar.js包。
2. 本案例采用nft方式进行图像识别，所展示的模型并不稳定，会有闪烁的情况出现。
3. 由于原因1，所以我们的放大缩小只能针对一个模型，想要多个模型需要另外自己编码。

以上就是这个项目的全部概述，如果有帮到你的话，希望点一个star谢啦!!☆⌒(*＾-゜)v。

