# 第四单元

## 例1   输入两个整数，输出两个数中的最大数

```c
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

```c
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



