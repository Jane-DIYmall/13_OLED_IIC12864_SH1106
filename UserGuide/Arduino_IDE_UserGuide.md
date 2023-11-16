# 【1.3INCH_OLED_IIC_SH1106】在Arduino UNO开发板上的运用
本教程目的是指导如何通过Arduino UNO开发板对1.3英寸SH1106的OLED进行显示图像操作。
资料包下载：[1.3inch_BULE_OLED_IIC12864_SH1106.zip](https://pan.baidu.com/s/1JV9Z0a2VLDOwMUmUkQ3qJA?pwd=6e24)

# 1. 硬件需求
>* OLED：1.3inch IIC接口 SH1106
![](../vx_images/353592220237356.png)
 
>* Arduino开发板：Arduino UNO Rev3 开发板一块及对应的USB数据线一条
![143013723257415](../vx_images/541982320250191.png)

>* 杜邦线：一公一母的2.54mm杜邦线一排
![](../vx_images/342562620242500.png)

>* 电脑：Windows/Mac 电脑一台（本教程使用Windows 11 64位系统）
![6434523242393](../vx_images/285032420246746.png)


# 2. 软件需求
>* 编程软件：Arduino IDE 1.8.19 （仅代表本教程测试版本，可以使用其他版本）
如果还未安装，请在Arduino官网链接进行Arduino IDE下载安装：[Arduino software](https://www.arduino.cc/en/software)
>* Arduino库：U8glib（Adafruit或u8glib的标准库形式可能不太适合此OLED设备。请确保您正在使用上方提供的资料包（里面更改了I2C地址和一些定义部分）。如果这些文件已经在库中，需要进行替换）

U8glib库安装说明：

1. 在Arduino IDE中，转到 **File** >  **Preferences**  
![](../vx_images/386341623249493.png)

2. 转到红色框中所指向的文件夹 
![](../vx_images/532191423231067.png)

3. 解压缩上方资料包，把路径 **1.3inch_BULE_OLED_IIC12864_SH1106\Arduino Example\heltec1.3OLED-master** 文件夹里的“U8glib”文件夹步骤2中的位置
![](../vx_images/205401823237360.png)


# 3. 硬件接线说明
13inch OLED同Arduino UNO接线示意图
![](../vx_images/43662323260380.png)

# 4. 例程测试
按如上接好线后打开一个例程进行测试。

1. 打开一个**Logo_DIYmall**例程，在Arduino IDE中，转到 **File** >  **Examples** >  **U8glib** >  **Logo_DIYmall**。
![](../vx_images/277082823257984.png)

2. 选择对应的开发板**Arduino UNO**以及对应的COM口。
![](../vx_images/478754123255486.png)

3. 进行编译烧录
![](../vx_images/497474423236727.png)

# 5. 测试
此次例程会在OLED屏幕上显示一个LOGO。
![](../vx_images/281764623259167.png)