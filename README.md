# Fish Tools

Note: Only for Intel CPUs at present.

注意事项:仅限Intel CPU使用目前

More radical Hacking Tools / Anti-Cheating Tools

更激进的黑客工具 / 反作弊工具

-
Usage: Open Water.exe=>Click Start=>Click Init PDB (waiting for loading to end)=>Click Init Start=>Green text appears=>Normal use (red text at the beginning doesn't matter)
-

使用方法:打开Water.exe=>点击Start=>点击Init PDB(等待加载结束)=>点击Init Start=>出现绿色字样=>正常使用 (刚开始都是红色字样不用在意).
-

In the introduction: Chinese is at the bottom, English is at the top, just read one!
-
介绍中:中文在下,英文在上,只需要读一个即可!
------------------------------------------------------------------------------------------------------------------------------------------------------
-
Copy memory: It can be written to read-only memory without modifying the properties of the target process, and the properties remain unchanged after writing,This is not about changing attributes=>writing=>changing back, the entire process will not be modified!

拷贝内存:可以在不修改目标进程属性的情况下,写入只读内存,写完之后属性依旧不变,这里并不是改属性=>写入=>改回,全程不修改!

![image](https://github.com/user-attachments/assets/694e9a12-2e4b-443a-84d1-269c56ae12b3)
-
-
Loading drivers (not captured by all ARK tools) can be tested using Test.sys driver, which will load ten "ez"/monitoring drivers, including manual mapping such as Kdmap loading

加载驱动(所有ARK工具都无法捕捉) 可以使用Test.sys驱动测试加载,会加载十个"ez" / 监控驱动加载,包括手动映射,诸如Kdmap加载

![image](https://github.com/user-attachments/assets/1e2a6539-12f1-4e2d-b700-d10fd78d2ab6)
-
-
Hidden memory class: It can hide specified memory, and no driver can read the memory!

隐藏内存类:可以隐藏指定内存,任何驱动都读取不到内存!

![image](https://github.com/user-attachments/assets/0d06d8c3-a9cc-422a-9594-21e8c301aa1d)
-
Traverse system windows: It can traverse any hidden window information. The printed information includes (window style, window rectangle, window name, window class name, window thread ETHREAD, window process ID, window process name...)

遍历系统窗口:可以遍历出任意隐藏的窗口信息 打印的信息包括(窗口样式,窗口矩形,窗口名字,窗口类名,窗口的线程ETHREAD,窗口的进程ID,窗口的进程名字...)

![image](https://github.com/user-attachments/assets/7ad1ace7-4b1b-408b-9a53-67abd3a9024d)
-

The above printed content can be checked using MongoDB or DbgView. Currently, it is compatible with Win10 21H2 version and is good because it is not well made compatible (too tiring)

以上打印的内容均可以用WinDbg 或者 DbgView 检查,目前兼容Win10 21H2版本良好
-

BUG:
[1] After loading all functions, it is temporarily impossible to open the driver selection list with three points. Manually enter the driver path to load: \?? \C:\Users\Administrator\Deskto\test.sys

漏洞:
[1]在加载完全部功能暂时无法用三个点打开选择驱动列表,手动输入要加载的驱动路径:\??\C:\Users\Administrator\Deskto\test.sys

