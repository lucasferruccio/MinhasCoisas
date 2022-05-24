#include <stdio.h>
#include <math.h>

int main()
{
    long position1, position2, aux1, aux2, aux3, aux4, aux5, actualnumber, sumdouble = 0, sumone = 0, sumall, validation, creditnumber;
    printf("Credit Card Number: ");
    scanf("%li", &creditnumber);
    //Sum of the double numbers
    for (int i = 1; i <= 16; i += 2)
    {
        //1,3,5,7,9,11,13,15
        aux1 = pow(10, i);
        aux2 = pow(10, i + 1);
        position1 = creditnumber / aux1;
        position2 = creditnumber / aux2;
        actualnumber = position1 - (position2 * 10);
        aux3 = actualnumber * 2;
        if (aux3 >= 10)
        {
            aux4 = aux3 / 10;
            aux5 = aux4 + (aux3 - aux4 * 10);
            actualnumber = aux5;
        }
        else
        {
            actualnumber *= 2;
        }
        sumdouble = sumdouble + actualnumber;
    }
    //Sum of the multiplied by one
    for (int i = 0; i <= 16; i += 2)
    {
        //0,2,4,6,8,10,,12,14
        aux1 = pow(10, i);
        aux2 = pow(10, i + 1);
        position1 = creditnumber / aux1;
        position2 = creditnumber / aux2;
        actualnumber = position1 - (position2 * 10);
        sumone = sumone + actualnumber;
    }
    sumall = sumdouble + sumone;
    validation = sumall % 10;
    //if validation equal to 0 the sum of the numbers ends with 0
    if (validation == 0)
    {
        printf("Validated");
    }
    else
    {
        printf("Invalidated");
    }
}
