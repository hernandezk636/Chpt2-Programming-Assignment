# Chpt2-Programming-Assignment

//Kevin Henrnandez
// CHPT2 PA

#include <stdio.h>
#include <math.h>
int main() {
double volumeCylinder;  // all variables are double since we are dealing with decimal values in our calculations// 
double areaCylinder;
double radius;
double height;

printf("please input the radius of the cylinder:\n"); // prompts the user to input a value for the radius//
scanf("%lf", &radius); // gets input and assignes it to radius//

printf("please input the height of the the cylinder:\n");  //same scenerio as previous statement//
scanf("%lf", &height);

volumeCylinder = (M_PI * pow(radius, 2) * height); // M_PI is the value of pi with a limit of 4 decimal values i believe,//
 //                                                   pow calculates radius to the power of 2, then multiply by height at the end//
                                               
areaCylinder = (2 * M_PI * radius * height) + (2 * M_PI * pow(radius, 2)); // i put "()" just to ensure that calculations are done //
//                                                                          the way i want even if i dont have to before adding//

printf("volume (cubic inches): %0.2lf\n", volumeCylinder);// outputs the prompt "volume (cubic inches):" followed by the value of the cylinder 
//                                                           ending in a new line to make it look more clean and less cluttered// 

printf("surface area (square inches) %0.2lf\n", areaCylinder);   // lf since we are dealing with a double type variable to display,
//                                                               and the 0.2 before lf is to set the the maximum numbers after the decimal//
 
 return 0; 
}
