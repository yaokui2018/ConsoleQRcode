# ConsoleQRcode
![visitor badge](https://thread-erratic-podium.glitch.me/badge?page_id=yaokui2018.ConsoleQRcode)

在终端/控制台里输出二维码，打印二维码字符（非图片），Java实现

## 依赖项
Zxing
- Jar包：https://pan.baidu.com/s/1ZKb8DwsBNIcE_kBQmjHASg?pwd=i4pj
- Maven
  ``` maven
  <dependency>
      <groupId>com.google.zxing</groupId>
      <artifactId>core</artifactId>
      <version>3.5.1</version>
  </dependency>
  ```
## 使用
``` java
ConsoleQRcode.printQRcode("需要生成二维码的内容");
```
## 效果
![image](https://user-images.githubusercontent.com/41621936/232272385-9ad841b5-218b-4697-be96-ec2a587593dc.png)

## 存在缺陷
1. 仅在终端/命令行窗口有效，像 IDEA 的 console 不太好使，因为 IDEA 输出的文字行高比较大，导致输出内容宽高不一致。

    ![image](https://user-images.githubusercontent.com/41621936/232272775-98716825-31d4-4c29-9da5-cf426c97b409.png)

2. 当二维码内容较为复杂（生成二维码尺寸会变大）或者 CMD 运行窗口较小时，会出现文字换行情况，导致排版错乱。
