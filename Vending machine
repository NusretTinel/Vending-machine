#include<stdio.h>
#include<stdlib.h>
#define COFFEE 5.50
#define TEA 2.50
#define ESPRESSO 8.45
#define AMERICANO 9.45

void transaction(float money);
int repeat(void);

int main(void)
{
    int a;
    float money;
    char ID;

    do {
        printf("Welcome to vending machine\n");
        printf("C: $5.50 coffee\nT: $2.50 tea\nE: $8.45 espresso\nA: $9.45 americano\n");
        printf("Please choose your option\n");
        scanf(" %c", &ID); 
        switch (ID)
        {
        case 'C':
            money = COFFEE;
            transaction(money);
            a = repeat();
            break;
        case 'T':
            money = TEA;
            transaction(money);
            a = repeat();
            break;
        case 'E':
            money = ESPRESSO;
            transaction(money);
            a = repeat();
            break;
        case 'A':
            money = AMERICANO;
            transaction(money);
            a = repeat();
            break;
        default:
            printf("Please choose one of the characters in table.\n");
            a = 1;
        }
    } while (a == 1);

    return 0;
}

void transaction(float money) // The function should return void, not int
{
    float input, res;
    printf("Please give your money: ");
    scanf("%f", &input);

    res = input - money;
    if (res < 0) {
        printf("Your money is not enough.\n");
    }
    else {
        printf("Here is your money: $%.2f\n", res);
        printf("Please take your drink.\n");
    }
}

int repeat( void)
{
    int a;
    printf("To continue press 1  ");
    scanf("%d", &a);
    return a;
}
