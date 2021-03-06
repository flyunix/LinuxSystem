# README

以前记录的Linux内核相关的内容都是以博客的形式存在，并没有组织成体系，在阅读的时候没有先后的连续性，所以打算一点一点集成到一个仓库中，这样方便以后查阅。

## 参考

* [The Linux Kernel’s documentation](https://www.kernel.org/doc/html/latest/)
* 书籍：Linux设备驱动开发详解 基于最新的Linux 4.0内核
* [The Linux Kernel Archives](https://www.kernel.org/)
* [Linux Kernel GitHub](https://github.com/torvalds/linux)

## 文档索引

文档名称(docs目录下) | 简述
:------|:-----
[0031_FPGA.md](docs/0031_FPGA.md)                                             | FPGA PCIe驱动开发笔记（私有，非公开仓库）
[0030_Ending_Align.md](docs/0030_Ending_Align.md)                             | 将文件每行填充空格到一定列数，个人分析代码调用流程最喜欢的工具；
[0029_Modbus_Protocol.md](docs/0029_Modbus_Protocol.md)                       | 目前百度IoT除了支持MQTT以外，Modbus TCP也是支持的；
[0028_MQTT_Protocol.md](docs/0028_MQTT_Protocol.md)                           | MQTT通信协议貌似已经成为标准的物联网通信协议了，测试使用了百度MQTT通信；
[0027_Easy_Image_Identification.md](docs/0027_Easy_Image_Identification.md)   | 树莓派采集USB摄像头的图片，并和预置图片的相似度对比并控制继电器；
[0026_I2C_Bus_Java_Access_Lib.md](docs/0026_I2C_Bus_Java_Access_Lib.md)       | Android直接访问I2C总线获取I2C从设备数据；
[0025_UART_Tool.md](docs/0025_UART_Tool.md)：                                   | 支持Linux/Android的命令行串口调试工具；
[0024_EtherCAT_Protocol.md](docs/0024_EtherCAT_Protocol.md)                   | 工业自动化数据实时性要求相对比较高，了解EtherCAT通信协议原理；
[0023_Bluetooth_Protocol.md](docs/0023_Bluetooth_Protocol.md)                 | 当你的蓝牙手环，除了手环功能既能连接你的笔记本，同时能连接你的手机，那它到底是怎么工作的呢？
[0022_USB_Protocol.md](docs/0022_USB_Protocol.md)                             | 不久笔记本电脑也许只剩下USB Type-C接口，那为什么不看看USB是怎么工作呢？
[0021_Edge_Computing.md](docs/0021_Edge_Computing.md)                         | 边缘计算可以认为是小区域的数据统筹处理；
[0020_Talk_To_IoT.md](docs/0020_Talk_To_IoT.md)                               | 其实我们已经开始进入*对话式物联网*：亚马逊Echo、百度小度等等音箱；
[0019_Bootstrap.md](docs/0019_Bootstrap.md)                                   | 如果你真的想为你的设备做网站，Bootstrap可以让你更快一点；
[0018_Website_For_Board.md](docs/0018_Website_For_Board.md)                   | 设备具有联网功能，那么为什么不尝试建个网站，用动态网站去控制你的设备呢，路由器不就是这么干的吗，当然人家用的是OpenWRT来处理整套系统，不过也不妨碍理解；
[0017_SD_Card_Image.md](docs/0017_SD_Card_Image.md)                           | SD/EMMC tar解包部署文件系统太慢，SD卡image文件直接dd更高效；
[0016_Ubuntu_Debian_For_ARM.md](docs/0016_Ubuntu_Debian_For_ARM.md)           | 学会基于Ubuntu/Debian ARM版发行自己的Linux ARM发行版；
[0015_Repo.md](docs/0015_Repo.md)                                             | Git是基本技能，多仓库管理的就轮到Repo出马，Anroid使用Repo管理；
[0014_Yocto.md](docs/0014_Yocto.md)                                           | 能做的事情和Buildroot类似，不过更重要的是芯片大厂都参与维护，知名度更高；
[0013_Buildroot.md](docs/0013_Buildroot.md)                                   | 也许Busybox是很不错的学习文件系统的工具，不过Buildroot会让你惊讶于不止于Busybox；
[0012_Raspberry_Pi.md](docs/0012_Raspberry_Pi.md)                             | 从事嵌入式Linux开发，树莓派还是可以知道一下，预研工作在上面进行还是挺不错的；
[0011_QEMU.md](docs/0011_QEMU.md)                                             | QEMU模拟硬件开发板，虽然现在的开源硬件已经很便宜了，不过QEMU还是可以了解一下的；
[0010_KGDB.md](docs/0010_KGDB.md)                                             | 实时调试内核；
[0009_Device_Tree.md](docs/0009_Device_Tree.md)                               | 外设控制器、外设与驱动的衔接——设备树；
[0008_Memory_Access.md](docs/0008_Memory_Access.md)                           | I2C/SPI/USB/GPIO等各种控制器寄存器如何访问；
[0007_Interrupt.md](docs/0007_Interrupt.md)                                   | 驱动是为了操作硬件，硬件和软件之间的神经——中断；
[0006_bootargs_Module_Param.md](./docs/0006_bootargs_Module_Param.md)         | bootargs参数中那么多，到底是给谁的；
[0005_devfs_udev.md](docs/0005_devfs_udev.md)                                 | 设备节点自动生成到底是谁在维护；
[0004_GPL.md](docs/0004_GPL.md)                                               | 开源不代表免费，免费的不一定开源，用了有Linux内核的系统，也许就可以要求要内核源代码，不过能不能看懂是另外一回事；
[0003_Cross_Compiler_Tools.md](docs/0003_Cross_Compiler_Tools.md)             | 怎么生成交叉工具链；
[0002_define.md](docs/0002_define.md)                                         | 常用宏定义使用，看不懂宏怎么窥视内核；
[0001_Coding_Style.md](docs/0001_Coding_Style.md)                             | 代码格式太蓝看的话，可能不会有人来帮你看Bug；
