
1.math.lib 만들기 & 22와 33더하기 구현
![diq](https://github.com/irop3126/c-rhkwp/assets/127822814/e4e0f541-a134-4245-97ff-aecb964b8375)


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
