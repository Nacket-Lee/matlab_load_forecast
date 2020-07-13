# matlab_load_forecast
    这个文档用于记录与matlab负荷预测算法相关的一些函数的使用和预测的过程
   
```
[num,txt,raw] = xlsread('myExample.xlsx')
```
    这个函数是matlab中常见的用来读取excel表格数据的函数，但有个缺点就是耗时较长，因此通常的做法就是读进来数据之后将数据格式另存为.mat格式，下次使用的时候就比较快
    上面这种用法读出来的数据格式除了num是double之外，txt和raw都是cell格式，顾名思义num就是保存纯数字格式的数据，txt保存纯文字的数据，raw保存所有

    导入数据之后要输入神经网络之前应该先通过矩阵变形将输入变成行输入
    
