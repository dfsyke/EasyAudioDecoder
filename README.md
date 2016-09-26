## EasyAudioDecoder ##

**EasyAudioDecoder** 是EasyDarwin开源流媒体服务团队整理、开发的一款音频转码到Linear PCM的工具库，目前支持G.711A/PCMA、G.711U/PCMU、G726、AAC音频格式的转码，跨平台，支持Android & iOS；

### Android AudioCodec库说明

 1. 该工程（Android目录下的工程）为Android的NDK工程；
 2. ffmpeg静态库已经编译ok，其中.h、.a文件位于ffmpeg/armeabi-v7a目录下；
 3. 该工程实际上是对于ffmpeg库的封装，具体实现见AACDecode.cpp文件；
 4. 库工程仅编译了armeabi-v7a版本，如需其他abi版本，可自己编译ffmpeg（参考http://blog.csdn.net/jyt0551/article/details/52519096#0-qzone-1-94593-d020d2d2a4e8d1a374a433f596ad1440），把对应abi的版本拷贝至ffmpeg目录下面，在Application.mk里增加改abi，再编译;
 5.  对应的java文件为AudioCodec.java

## 调用示例 ##

- **testEasyAudioDecoderr**：通过EasyAudioDecoderAPI对G711A/G711U/G726/AAC进行转码；

- **ARM版本的EasyAudioDecoder库可自行编译**；

## 调用过程 ##
![](http://www.easydarwin.org/skin/easydarwin/images/easyaudiodecoder20160910.png)

## 获取更多信息 ##

邮件：[support@easydarwin.org](mailto:support@easydarwin.org) 

WEB：[www.EasyDarwin.org](http://www.easydarwin.org)

Copyright &copy; EasyDarwin.org 2012-2016

![EasyDarwin](http://www.easydarwin.org/skin/easydarwin/images/wx_qrcode.jpg)
