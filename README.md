# 中兴光猫系列配置解密工具

解密操作：
```
 .\ztecfg.exe -d AESCBC -i .\db_user_cfg.xml -o 1.cfg
```
其中：
```
-d AESCBC：指定解密算法为AESCBC。
-i .\（要解密的文件名）db_user_cfg.xml：指定要解密的文件路径及文件名。
-o （解密后文件名）123.cfg：指定解密后的文件名及保存路径。
```

加密操作：
```
 .\ztecfg.exe -e AESCBC -i .\1.cfg -o db_user_cfg.xml
```
其中：
```
-e AESCBC：指定加密算法为AESCBC。
-i .\（要加密的文件名）123.cfg：指定要加密的文件路径及文件名。
-o （加密后文件名）db_user_cfg.xml：指定加密后的文件名及保存路径。
```
```
crc xor aescbc
```


![zte](https://raw.githubusercontent.com/wx1183618058/ZET-Optical-Network-Terminal-Decoder/master/src.png)

**本软件**是一款专为解密中兴光猫配置的工具，使用QT开发。
- **具体功能** ：如图基本所有加解密都支持。
- 用 Qt creator 打开编译即可， 在zteont.pro中设置好依赖 zlib

> $ cd ZET-Optical-Network-Terminal-Decoder
> 
> $ qmake
> 
> $ ./zteont
