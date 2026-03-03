****FEA自动化工具使用SOP****

****一、使用****

1.连接公共电脑，计算机名和用户名如下，密码Csisolar@2025C

  

2.开始界面中选中如下求解器，出现下右图的APDL求解界面时说明许可证连接成功。

3\. 双击打开路径下的exe文件，出现如下界面。此时最好检查D盘空间，若可用空间小于20GB，建议删除个人文件夹内的结果文件（rst及其他文件），保留计算文件（cdb文件）

****路径：D:\\00-Personal folder\\FEA\_Automation\_Tool****

  

4.按需求选择版型及安装方式，输入安装距离（注：所有模型初始位置均为100mm，因此输入150mm，则表示实际模型为100+150=250mm），模型中仅计算该部分载荷。

5.计算过程中界面处于未响应状态，****此时不要随意点击窗口****，后面黑色窗口显示此时正在进行Ansys计算。

  

6.计算过程中文件说明：

  

ü  200+2400：文件夹，存放结果文件，计算进度可查看.out文件

ü  ansys.msg: 导入hypermesh生成的额外文件，无实际作用

ü  command.tcl: hypermesh日志记录文件

ü  CS6.2-66TB-……\_P5400pa.cdb: 源文件

ü  CS6.2-66TB-……\_P2400pa.cdb: 位置挪完后的新文件，****可通过查看两个文件大小来检查是否导出存在问题****

ü  cs6.msg：ansys计算过程的日志文件

ü  FEA Report：导出报告

ü  Hw\_command.tcl: hyperview操作记录文件

ü  Read\_result.tcl: hyperview读取结果的脚本

ü  result.png: 云图截图

ü  result.txt：云图最大值数据

ü  Run\_Ansys.bat: 用于执行ansys的系统文件

ü  Run\_hypermesh.bat: 用于执行hypermesh的系统文件

ü  Run\_hyperview.bat: 用于执行hyperview的系统文件

ü  Write\_to\_file2.tcl文件：hypermesh操作

****二、维护****

1.模型文件位置D:\\00-Personal folder\\09\_YB\\Model\_ui\\ModelTemplate，若有新的文件加入或需修改模型，可按如下规则进行文件名和模型内部修改。

l  长边railless

示例：CS6.2-48TD\_longrailless\_A100mm\_P3000pa

          4部分（版型名称\_安装方式\_位置\_载荷值），使用下划线"\_"分割

          版型名称较长时用"-"连接

          P表示positive，正压，N表示negative，为负压

          安装方式：固定为longrailless，暂不支持其他

l  垂直长边压块

示例：CS6.2-48TD\_4perpclamps\_A100mm\_P6000pa

l  ID规则（****ID号必须连续，否则后处理无法与component对应****）

1：压块

2：cerig单元

3：mass单元

4：导轨

5：边框（包含长短边框）

6：玻璃（包含正背面玻璃）

7：硅胶（包含长短边硅胶）

8：EVA

****三、解决方法****

3.1  Hypermesh许可证问题

  

****任务管理器—服务—Altair License Server—右键重新启动即可****
