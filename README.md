# avarage-calculator
The exercise of average.

#include <stdio.h>
#include <time.h>

int main(){

    double x, y, z;
    int choiceCalculation;

    printf("Type three numbers: ");
    scanf("%lf %lf %lf", &x, &y, &z);

    printf("Which calculation do you want perform?");
    printf("\n1. Geometric average\n2. Weighted average\n3. Harmonic Average\n4. Arithmetic Average\n");
    scanf("%d", &choiceCalculation);

    if(choiceCalculation == 1) printf("The Geometric Average is: %lf", x*y*z);

    else if(choiceCalculation == 2) printf("The Weighted Average is: %lf", (x + 2*y + 3*y)/6);

    else if(choiceCalculation == 3){
        double harmonic;
        harmonic = 1/(1/x + 1/y + 1/z);
        printf("The Harmonic Average is: %lf", harmonic);
    }

    else if(choiceCalculation == 4) printf("The Arithmetic Average is: %lf", (x + y + z)/3);

    else printf("Calculation not valid");

    
    return 0;
}
