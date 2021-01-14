# 机器学习实验

小组成员：汤韬（组长）、张洪鑫、李炜煜


操作系统 windows 10

python 版本 3.7，需要额外安装 matplotlib、pandas、numpy、 seaborn

c++ 编译环境 gcc 9.2.0 使用c++17，编译命令 `g++ main.cpp -std=c++1z -m64 -o main.exe`

### 实验一、 多源数据集成、清洗和统计

合并两个数据源，去重并且去除一些部分信息缺失的数据

- ID 统一为 202XXX
- 身高统一为 cm 作为单位
- 性别用 'male' 和 'female' 表示

- 具体的实现方法是通过对 ID 排序，那么 ID 相同的数据就会在相邻，然后比较去重合并

  如果两个ID相同的数据有某一项不同并且不为空，说明数据冲突，那么要将数据删除

  如果两个ID相同数据有一项为空，那么用另一个数据补充



### 实验二、 数据统计和可视化

本实验的所有画图通过 matplotlib 实现

按公式实现即可

### 实验三、 k-means聚类算法

本实验的所有画图通过 matplotlib 实现

k-means 算法实现在 k-means.cpp 中，代码有注释

产生的聚类结果会输出为txt文件保存

draw.py 画出散点图
