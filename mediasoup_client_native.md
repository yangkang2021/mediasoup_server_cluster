# mediasoup_client_native
mediasoup客户端原生c++开发项目.

## 目标
1. 主要支持平台：Windows，Mac，Ubuntu/Centos。会考虑到Android和ios的通用性。
2. 支持任意音视频的输入发布：
    - camera和mic
    - yuv帧
    - 屏幕录制
    - 音视频文件
    - IPC网络摄像头采集
    - ffmpeg获取的数据
    - 后续支持海思sdk的采集...
    - ...
3. 扩展编码器：
    - 支持intel sdk硬件编解码
    - 支持英伟达 video sdk的硬件解码
    - 支持ffmpeg的编解码器调用。
    - 后续支持海思sdk的硬件编解码...
4. 扩展音频设备
    - 支持动态的切换设备
    - 支持混入额外的音频流
    - 支持获取每一路音频流的实时音量
5. 扩展图像处理
    - 支持采集和渲染的数据回调进行预处理
    - 支持简单的图像处理算法
    - 支持美颜算法
    - 支持核心的深度学习算法：检测，分割，识别，跟踪，OCR文字提取。
6. 应用扩展
    - 虚拟主播
    - 全息投影
    - 三维重建
    - 全景直播

## C++接口规范
1. 参数传入传出不包含c++标注库的类
    - 列表采用数组。
    - string采用const char *。
2. export导出




## 客户软件开发：
1. 工具4分天下：pc，web，ios，android。
2. 得到6个软件：web，ios，android，pc-windows，pc-linux，pc-mac。
##### PC端
![图 1](images/aab8401acd79683dd9b8ad979ddd413cca33bf0e0d9d198739ab8be8f77f3971.png)  

##### Android端
![图 2](images/295290790f56996424d267c4311279fb9c21957bdb973fe12746f4340a1bf150.png)  

##### ios端
![图 1](images/c9dee87b216297b77b8b6ca263476c6270012304fb90699c701a3686afaccc6f.png)  

##### Web端
![图 3](images/f2431c3e5734cef3803c001636476066a66d55c0f1bc3cdf51746d3ecfba076c.png)  
