#include<stdio.h>
#include<conio.h>
#include<stdlib.h>

#define MAX_SIZE 3

void push(int i);
void pop(void);

int choice, i;
int *tos, *p1, arr_stack[MAX_SIZE];
int exit_p = 1;

int main() {

    int value;

    tos = arr_stack; /* tos points to the top of stack */
    p1 = arr_stack; /* initialize p1 */
    printf("\n Simple Stack Example - Pointers");

    do {
        printf("\nStack Pointer : Main Menu");

        printf("\n1.Push \t2.Pop \tOthers to exit : Your Choice : ");
        scanf("%d", &choice);
        switch (choice) {
            case 1:
                printf("Enter value: ");
                scanf("%d", &value);
                push(value);
                break;
            case 2:
                pop();
                break;
            default:
                exit_p = 0;
                break;
        }
    } while (exit_p);

    return 0;
}

void push(int i) {
    if (p1 == (tos + MAX_SIZE)) {
        printf("\nStatus : Stack Overflow.\n");
    } else {
        *p1 = i;
        printf("\nPush Value : %d ", *(p1));
        p1++;
    }
}

void pop(void) {
    if (p1 == tos) {
        printf("\nStatus : Stack Underflow.\n");
        //return 0;
    } else {
        p1--;
        printf("\nPop Value : %d ", *(p1));
    }
}
