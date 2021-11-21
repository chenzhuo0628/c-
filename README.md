# c-
学习的点点滴滴
2. 第一个C语言程序
3. 数据类型
为什么出现这么的类型？
每种类型的大小是多少？
注意：存在这么多的类型，其实是为了更加丰富的表达生活中的各种值。
类型的使用：
3. 变量、常量
生活中的有些值是不变的（比如：圆周率，性别，身份证号码，血型等等）
有些值是可变的（比如：年龄，体重，薪资）。
#include <stdio.h>
int main()
{
    printf("hello bit\n");
    printf("he he\n");
    return 0;
}
//解释：
//main函数是程序的入口
//一个工程中main函数有且仅有一个
char        //字符数据类型
short       //短整型
int         //整形
long        //长整型
long long   //更长的整形
float       //单精度浮点数
double      //双精度浮点数
//C语言有没有字符串类型？
#include <stdio.h>
int main()
{
    printf("%d\n", sizeof(char));
    printf("%d\n", sizeof(short));
    printf("%d\n", sizeof(int));
    printf("%d\n", sizeof(long));
    printf("%d\n", sizeof(long long));
    printf("%d\n", sizeof(float));
    printf("%d\n", sizeof(double));
    printf("%d\n", sizeof(long double));
    return 0;
}
char ch = 'w';
int weight = 120;
int salary = 20000;
不变的值，C语言中用常量的概念来表示，变得值C语言中用变量来表示。
3.1 定义变量的方法
3.2 变量的分类
局部变量
全局变量
总结：
上面的局部变量global变量的定义其实没有什么问题的！
当局部变量和全局变量同名的时候，局部变量优先使用。
3.3 变量的使用
int age = 150;
float weight = 45.5f;
char ch = 'w';
#include <stdio.h>
int global = 2019;//全局变量
int main()
{
    int local = 2018;//局部变量
    //下面定义的global会不会有问题？
    int global = 2020;//局部变量
    printf("global = %d\n", global);
    return 0;
}
#include <stdio.h>
int main()
{
    int num1 = 0;
   int num2 = 0;
    int sum = 0;
    printf("输入两个操作数:>");
    scanf("%d %d", &num1, &num2);
    sum = num1 + num2;
    printf("sum = %d\n", sum);
    return 0;
}
//这里介绍一下输入，输出语句
//scanf
//printf
