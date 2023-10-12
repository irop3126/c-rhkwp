1.mymath.lib 만들기 & 22와 33더하기 구현

![image](https://github.com/irop3126/c-rhkwp/assets/127822814/c501a237-8daf-4a00-920d-73cb94d1fc08)


2.코드

test.c
```c
#include <stdio.h>
int main()
{
printf("%d", add(22,33));
}
```

math.c (math.lib)
```c
#include<stdio.h>
int add(int a, int b)
{return a+b;}
int min(int a, int b)
{return a-b;}
int mul(int a, int b)
{return a*b;}
int div(int a, int b)
{return a/b;}
int mod(int a, int b)
{return a%b;}
```
