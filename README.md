# note
字符串String：
Definition:以'\0'或者0结尾的一串字符
     But  0或者'\0'（整数0）是一样的，但是和'0'（字符，人可以读到的0，0x30 十六进制，十进制的48）不同.
0的作用？表示字符串结束了，但它本身不在里面-->so 我们计算字符串长度的时候是不会包含这个0的
Format:在内存里存在的形式只有数组(字符串是数组)，但是访问时是数组或者指针-->给我滚回去想想指针和数组的联系！
头文件：#include <string.h>
 
                string是数组
string variable：----->字符数组的变量，just表现形式不同
  char *str="Hello"；
  char word[]="Hello"；
  char line[10]="Hello"；  在line里头只占5个字符？No 6个字节  why?还有个结尾的0，注意：虽然0占据了内存当中的字节，数组长度要+1，但是它并不在字符串长度之内
""-->字符串的常量，会被编译器变成一个字符数组放在某处，数组长度要+1
两个相邻的字符串常量会被自动连接起来。



一些零碎的knowledge points:
1.整数（char ,short,int,long,long long）的输入输出：但是只有两种输入输出形式 int,long long
%d:char,short,int(所有小于int)
%ld:long,long long(所有大于int )
%u:unsigned
%lu:unsigned long long

二.矩阵
1.矩阵在C语言中如何表示？
  数组
2.矩阵加法：多维数组，遍历，for嵌套
3.矩阵乘法：注意行列数的变化，引入中间值idx
   本质：两个线性变化的复合
4.矩阵的转置：注意行列交换，for循环时的赋值
