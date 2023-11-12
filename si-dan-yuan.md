# 第四单元

## 条件语句

### 例1   输入两个整数，输出两个数中的最大数

```
#include<stdio.h>
int main()
{    
     int a,b;
     scanf("%d%d",a,b);
     if(a>b)
         printf("最大数是：%d",a);
     if(a<=b)
         printf("最大数是：%d",b);   
     return 0;
}
```

### 做一次比较，实现同样的功能：

```
#include <stdio.h>
int main()
{ 
     int a,b,max;
     scanf("%d%d",&a,&b);
     if(b>max)
        max=b;
     printf("%d和%d的最大值是%d",a,b,max);
     return 0;
}
```

### 例2  输入两个整数，按照从小到大的顺序输出

```c
#include <stdio.h>
int main()
{    
     int a,b,max,t;
     scanf("%d%d",&a,&b);
     if(a>b)
     {       t=a;    //将a的值给t
             a=b;     //将b的值给a（可以这样理解，此时a的值空了）
             b=t;     //将t的值（刚才a的值给b）   最后结果就是a和b互调了
     } 
     printf("FROM MIN TO MAX：%d， %d",a,b);
     return 0;
 }
```

### 例3 输入一个整数，判断该数是正数，还是负数

```c
#include <stdio.h>    
int main()
{    
     int x;
     scanf("%d",&x);    

     return 0;
}
```

### 例4  编写程序，判断某一年是否是闰年

当输入2023，2024，2000，1900的时候，输出为？

| 序号 | （同时）闰年的条件1 | （同时）闰年的条件2 | （或）闰年的条件3 |
| :--- | :--- | :--- | :--- |
| 1 | year%4==0 | year%4！=100 | 或者year%400==0 |

```
#include <stdio.h>
int main()
{    
     int year;    
     scanf("%d",&year); 
     if(                            )
         printf("the year is leapyear");
     else
         printf("the year is not leapyear");
     return 0;
}
```

## 条件嵌套

### 例5 如果x为正数，输出1，如果x为负数，输出为-1，如果x为0，输出为0

```c
#include<stdio.h>
int main()
{   int x,y;
     printf("PLS enter the value of x：\n");
     scanf("%d",&x);
     if(x>=0)
          if(x>0)
               y=1;
          else
               y=0;
     else
          y=-1;
     printf("y=%d\n",y);
     return 0;
}
```

### 例6 输入分数，判断优良差

\(当输入78，87，65，23时，输出为？\)

```c
#include <stdio.h>
int main()
{    float s;
     scanf("%f",&s);	
     if(s>=0&&s<=100)
     {
          if(s>=90)
               printf("youxiu");
          else if(s>=80)
                    printf("lianghao");
                else if(s>=70)
                      printf("zhongdeng");
                      else if(s>=60)
                                 printf("jige");
                             else
                                    printf("bujige");
     }
     else
          printf("buhefa");	
     return 0;
}

```



