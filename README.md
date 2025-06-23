#include<stdio.h>

int main()
{
    int real_price;
    int off;


    printf("enter the real price\n");
    scanf("%d",&real_price);

    if(real_price<=100) {
        printf("your off is 5%%\n");
        off=5;
    }

    else if(real_price<=300) {
        printf("your off is 10%%\n");
        off=10;
    }

    else if(real_price<=500) {
        printf("your off is 20%%\n");
        off=20;
    }

    else if(real_price<=800) {
        printf("your off is 25%%\n");
        off= 25;
    }

    else if(real_price>=1000) {
        printf("your off is 30%%\n");
        off = 30;
    }

    else {
        printf("sorry nothing offer\n");
        off = 0;
    }

    int discount;

    discount = real_price*off/100;


    int price;

    price = real_price - discount;
    printf("your product price is %d\n",price);

    return 0;
}
