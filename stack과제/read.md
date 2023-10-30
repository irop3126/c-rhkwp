스택과 자료구조

자료구조는 데이터를 구성하고 저장하는 방식을 나타내는 것이며, 스택은 그 중 하나입니다. 스택은 데이터를 일렬로 쌓아두는 구조로, 데이터의 삽입과 삭제가 한쪽 끝에서만 이루어지는 선형 자료구조입니다. 스택은 후입선출(LIFO, Last-In-First-Out) 원칙을 따릅니다. 가장 최근에 삽입된 데이터가 가장 먼저 삭제됩니다.

스택의 연산방식은 다음과 같습니다.

Push: 스택에 데이터를 삽입하는 연산입니다.
Pop: 스택에서 데이터를 삭제하고 반환하는 연산입니다.
Top/Peek: 스택의 맨 위에 있는 데이터를 조회하는 연산입니다. 삭제하지 않습니다.

스택의 활용분야는 다음과 같습니다.

스택은 컴퓨터 과학 및 소프트웨어 개발에서 다양한 분야에서 활용됩니다. 예를 들면 함수 호출 스택, 뒤로 가기 버튼의 기록, 괄호 검사, 계산기 등 다양한 애플리케이션에서 사용됩니다.

코드
```c
#include <stdio.h>
#define MAX_SIZE 3
int stack[MAX_SIZE];
int top = -1;

void push(int value) {
    if (top < MAX_SIZE - 1) {
        stack[++top] = value;
    } else {
        printf("스택이 꽉 찼습니다. 더 이상 푸시할 수 없습니다.\n");
    }
}

int pop() {
    if (top >= 0) {
        return stack[top--];
    } else {
        printf("스택이 비어있습니다. 팝할 데이터가 없습니다.\n");
        return -1;
    }
}

int main() {
    push(1);
    push(2);
    push(3);

    int poppedValue1 = pop();
    int poppedValue2 = pop();
    int poppedValue3 = pop();

    printf("팝한 값: %d %d %d\n", poppedValue1, poppedValue2, poppedValue3);

    return 0;
}
```
소감
202230945 김범석

자료구조에서 스택에 대해 공부하고 그것을 어디에서 활용하는지, 스택을 통해 어떠한 프로그램을 만들 수 있는지 알게되었으며, 스택의 데이터 저장등의 방식과 원리에 대해 알게되어서 나름 재미있는 시간이였습니다.
