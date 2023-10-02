# Note for Introduction of Conmputer Science
<div align = right>By Grantley-W in CEO of NKU.</div align = right>

```
写在前面：
本笔记标号统一采用以下顺序：一、1.  (1)
考试会考的知识点以引用方式总结 使用> 进行标注
重点全部以==高亮==形式标注
所有示例代码均使用python编写
```
## 零 导论
计算机的两套结构：冯诺依曼结构、图灵结构
- 图灵结构：![图灵结构示意图](\Photos/1696131596567.png)
- 冯诺依曼结构：![冯诺依曼结构](\Photos/fnymstructure.png)

==二者根本区别：冯结构可以将程序储存在计算机的存储器中，图灵结构不行==

硬件三大子系统：中央处理器、主存储器、输入输出子系统

## 一 数据结构

### 1 数据与结构

> 考点：二、八、十、十六进制转换（整数和小数都要熟练）

位：bit 一个0/1 8个bit组成一个byte，是计算机处理数据的最小单位

常考汇编指令：
- load R1, address ：把address里的数值读取到R1寄存器里
- mov R1, constant / mov R2, R1
- add/sub R2, R1, constant ：R2 = R1 +- constant
- add/sub R3, R1, R2 : R3 = R1 +- R2
- shiftl/shiftr R3, R1, R2 :左右移指令 R3 = R1 左/右移动R2位

### 2 数组
 二维数组的行主序存储：对于 object[i][j], 有：y = x + cols * (i-1) + (j-1)

 数组的增改删查：
 - 增：所有数据从后往前依次后移一位，再插入元素
 - 改：根据数组索引直接修改
 - 删：数据依次往前一位覆盖
 - 查：下标索引
  ```
    例：删去30个数的数组中第6个元素
    i = 5
    while i< 30 - 1:
        arr[i] = arr[i+1]
    end while
  ```

